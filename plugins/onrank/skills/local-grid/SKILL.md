---
name: local-grid
description: "Where a local business shows on Google Maps around its address, point by point, and what would put it ahead locally (structured data, Business Profile, name-address-phone consistency). Use when the user asks about local rankings, the map pack, Google Maps or a dealership's local visibility."
---

# OnRankSEO — local grid

Tools (OnRankSEO MCP server, https://onrankseo.com/api/mcp):
- `map_grid` — Where the client shows on the map (needs console access)
- `dealer_pack` — What would put a local business ahead (needs console access)

## Steps

1. Call dealer_pack.
2. Call map_grid with the search the user names; if it returns 'not measured — needs GOOGLE_MAPS_API_KEY', say exactly that.

## Output contract

OnRankSEO foundations — the rules every answer built on these tools follows:

- Never promise a search position, a date for a result, an amount of traffic, or an appearance or citation in an AI answer. No one can, and OnRankSEO does not.
- Never invent a score, a metric or a rating word. Use only the numbers the tools return, with the source, date and method they come with; OnRankSEO's own score is its published formula (onrankseo.com/how-we-score), and another company's metric is always named as theirs.
- Always label an estimate as an estimate, with its source and month (for example: Estimate · DataForSEO · 2026-11).
- Pass on a finding or a recommendation only with its evidence — what was seen, where, and the date — and the rule it rests on, as the tool returns them. A rule is quoted only where the tool returns a verbatim quotation; otherwise it is named. 'Our observation, not a published rule' is said as such.
- Anything the tools return as 'not measured — needs …' is reported exactly that way, never as zero, never as a pass, never filled in.
- AI visibility is a rate over repeated runs with the run count beside it. A single AI answer is never evidence.
- A person at OnRankSEO checks and signs every report. These tools draft and record; they never send anything to a client, and an email can only be queued for a person to approve.
