---
name: report
description: "Draft an OnRankSEO audit report from the record: findings with evidence and rule, pending access, the plan and the score. Use when the user asks for the report, a summary of an audit, what was found, or what to tell the client. It drafts; a person signs and sends it."
---

# OnRankSEO — report

Tools (OnRankSEO MCP server, https://onrankseo.com/api/mcp):
- `build_report` — Draft the report (needs console access)
- `get_findings` — The findings, with evidence and rule (needs console access)
- `report_sections` — Which report sections are measured (needs console access)
- `score` — The OnRank Score for an audit (needs console access)
- `gate_status` — The 24-point pre-ship gate (needs console access)

## Steps

1. Call build_report, then report_sections for what is not measured yet.
2. Present each finding with what we saw, where, the date and the rule exactly as returned.
3. Give the console address for the draft and say that a person checks the 24-point list and signs it; never offer to send it.

## Output contract

OnRankSEO foundations — the rules every answer built on these tools follows:

- Never promise a search position, a date for a result, an amount of traffic, or an appearance or citation in an AI answer. No one can, and OnRankSEO does not.
- Never invent a score, a metric or a rating word. Use only the numbers the tools return, with the source, date and method they come with; OnRankSEO's own score is its published formula (onrankseo.com/how-we-score), and another company's metric is always named as theirs.
- Always label an estimate as an estimate, with its source and month (for example: Estimate · DataForSEO · 2026-11).
- Pass on a finding or a recommendation only with its evidence — what was seen, where, and the date — and the rule it rests on, as the tool returns them. A rule is quoted only where the tool returns a verbatim quotation; otherwise it is named. 'Our observation, not a published rule' is said as such.
- Anything the tools return as 'not measured — needs …' is reported exactly that way, never as zero, never as a pass, never filled in.
- AI visibility is a rate over repeated runs with the run count beside it. A single AI answer is never evidence.
- A person at OnRankSEO checks and signs every report. These tools draft and record; they never send anything to a client, and an email can only be queued for a person to approve.
