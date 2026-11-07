---
name: audit
description: "Start or continue an OnRankSEO audit for a client: open it, crawl the site with the 38 audit checks, gather the market data and observe competitors. Use when the user asks to audit a client's site, run an audit, or see where an audit stands. Needs an OnRankSEO console account."
---

# OnRankSEO — audit

Tools (OnRankSEO MCP server, https://onrankseo.com/api/mcp):
- `run_audit` — Start an audit for a client (needs console access)
- `audit_status` — Where an audit stands (needs console access)
- `gather_market` — Gather the market data (needs console access)
- `observe_competitors` — Observe the client and up to three competitors (needs console access)
- `link_check` — Broken and blocked links, counted properly (needs console access)
- `pending_access` — What is waiting on the client's access (needs console access)

## Steps

1. Call run_audit with the client (or audit_status if the audit exists).
2. Call observe_competitors with up to three competitor addresses the user names.
3. Call link_check and pending_access, and report what is measured, what is not measured and what each needs.
4. Record findings only with add_finding, each with its evidence, date and rule.

## Output contract

OnRankSEO foundations — the rules every answer built on these tools follows:

- Never promise a search position, a date for a result, an amount of traffic, or an appearance or citation in an AI answer. No one can, and OnRankSEO does not.
- Never invent a score, a metric or a rating word. Use only the numbers the tools return, with the source, date and method they come with; OnRankSEO's own score is its published formula (onrankseo.com/how-we-score), and another company's metric is always named as theirs.
- Always label an estimate as an estimate, with its source and month (for example: Estimate · DataForSEO · 2026-11).
- Pass on a finding or a recommendation only with its evidence — what was seen, where, and the date — and the rule it rests on, as the tool returns them. A rule is quoted only where the tool returns a verbatim quotation; otherwise it is named. 'Our observation, not a published rule' is said as such.
- Anything the tools return as 'not measured — needs …' is reported exactly that way, never as zero, never as a pass, never filled in.
- AI visibility is a rate over repeated runs with the run count beside it. A single AI answer is never evidence.
- A person at OnRankSEO checks and signs every report. These tools draft and record; they never send anything to a client, and an email can only be queued for a person to approve.
