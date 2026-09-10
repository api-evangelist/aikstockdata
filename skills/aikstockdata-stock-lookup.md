---
name: korean-stock-lookup
description: Look up one Korean listed company by name or ticker and return its confirmed close, quarterly earnings and 1-year price context.
api: 한국주식데이터 공개 데이터 API
method: generated
source: mcp/aikstockdata-mcp-tools.json (probed) + openapi/aikstockdata-openapi.json
tools:
  - search_stock
  - get_stock
  - get_history
endpoints:
  - GET /data/public/search_index.json
  - GET /data/public/s/{code}.json
  - GET /data/public/s/{code}_history.json
---

# Korean stock lookup

Resolve a Korean company to its 6-digit KRX code, then pull its snapshot and price history. All calls are keyless GETs (or the equivalent MCP tools); data is the T+1 confirmed close, not real-time.

## Steps
1. **Resolve the code.** If you only have a name, call `search_stock(query)` (or GET `/data/public/search_index.json` / `search_index_aliases.json`) and take the 6-digit `code`. Codes match `^[0-9A-Z]{6}$` (e.g. `005930` = 삼성전자).
2. **Get the snapshot.** Call `get_stock(code)` (or GET `/data/public/s/{code}.json`, ~5KB). Returns confirmed close, change, market cap, latest incl. preliminary quarterly earnings, and ranking signals.
3. **Add price context (optional).** Call `get_history(code, days)` (or GET `/data/public/s/{code}_history.json`, ~250 trading days of `[date, close, volume]`). Use the `columns` field for order; do not assume dates are contiguous — holidays have no row.

## Rules
- A missing/invalid code returns **HTTP 404** ("없는 종목코드/날짜"); resolve valid codes first (see errors/aikstockdata-problem-types.yml).
- No auth, no quota — fair use only (rate-limits/aikstockdata-rate-limits.yml).
- Data refreshes once per trading day at 18:10 KST; repeated calls in a day return identical values.
