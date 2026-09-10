---
name: korean-market-digest-and-disclosures
description: Summarize the Korean market for a trading day and surface the important DART disclosures with their typical post-filing price impact.
api: 한국주식데이터 공개 데이터 API
method: generated
source: mcp/aikstockdata-mcp-tools.json (probed) + openapi/aikstockdata-openapi.json
tools:
  - get_today
  - get_market_summary
  - get_disclosures
  - get_disclosure_impact
endpoints:
  - GET /data/public/today.json
  - GET /data/public/disclosures.json
  - GET /data/public/disclosures_top100.json
  - GET /data/public/disclosure_impact.json
---

# Korean market digest and disclosures

Answer "how was the Korean market today, and what was filed that matters?"

## Steps
1. **Digest.** Call `get_today()` (or GET `/data/public/today.json`) for index levels, breadth, 52-week high/low counts, top-3 disclosures and growth top-3. For just index + breadth, `get_market_summary()`.
2. **Disclosures.** Call `get_disclosures(date?, session?, label?, min_score?, limit?)` (or GET `/data/public/disclosures.json`; for the ranked shortlist GET `/data/public/disclosures_top100.json`). Each row carries receipt time (HH:MM), session, a plain-language summary and an importance score.
3. **Impact (optional).** For a disclosure type, call `get_disclosure_impact(label)` (or GET `/data/public/disclosure_impact.json`) for the median market-adjusted price path after that filing type.

## Rules
- Large files truncate in agents at ~50-150KB; prefer `disclosures_top100.json` and check `index.json.file_bytes` before pulling a full dataset.
- These are facts and signals, not investment advice; quotes are prior-session confirmed closes.
- No auth; once-per-trading-day refresh at 18:10 KST.
