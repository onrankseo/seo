# OnRankSEO for Claude

This is the plugin marketplace for OnRankSEO. It holds one Claude plugin, `onrank`, which connects Claude to OnRankSEO's audit tools: it runs a real SEO audit of a website, returns each finding with what was seen, where and when, and the published rule it rests on, and drafts a report that a person at OnRankSEO checks and signs.

**You need an OnRankSEO account.** The plugin signs in with the account you already have — no API key. It sees exactly what that account sees, and refuses whatever that account could not do in OnRankSEO. Three tools (the first look at one page, the checks catalogue and the score formula) work for any account; the audit tools need console access.

## Install in Claude Code

```
/plugin marketplace add onrankseo/seo
/plugin install onrank@onrankseo
```

Then run `/mcp`, choose `onrankseo`, and sign in.

Skills: `/onrank:foundations`, `/onrank:first-look`, `/onrank:audit`, `/onrank:report`, `/onrank:link-plan`, `/onrank:local-grid`, `/onrank:ai-visibility`, `/onrank:evidence`. `foundations` loads by itself and carries the rules below. The subagent `onrank-auditor` runs long audits.

In Claude on the web or desktop, add a custom connector with the address https://onrankseo.com/api/mcp and sign in; ask in plain words, for example "give me a first look at example.com" or "draft the report for my client's audit".

## What it deliberately cannot do

- Send a report to a client, or sign one. A person at OnRankSEO checks every report against a 24-point list and signs it in the console.
- Send an email. It can only queue a draft in the Approvals queue for a person to read, approve and send.
- Invent a metric, a score or a rating word. Every number returns with its source, date and method; anything unmeasured returns as 'not measured — needs <KEY>'.
- Promise a position, a date, traffic or an AI citation.
- Pass on a finding without its evidence and the rule it rests on.
- Do anything the signed-in account could not do in the OnRankSEO console.

These limits are the point: an assistant connected to OnRankSEO can only pass on what OnRankSEO can stand behind.

## The tools

| Tool | What it does | Who can use it |
|---|---|---|
| `first_look` | Free first look at one page | any account |
| `checks_catalogue` | The 38 audit checks | any account |
| `score_formula` | The OnRank Score formula | any account |
| `run_audit` | Start an audit for a client | console account |
| `audit_status` | Where an audit stands | console account |
| `get_findings` | The findings, with evidence and rule | console account |
| `add_finding` | Record a finding | console account |
| `evidence` | One finding's evidence | console account |
| `pending_access` | What is waiting on the client's access | console account |
| `observe_competitors` | Observe the client and up to three competitors | console account |
| `gather_market` | Gather the market data | console account |
| `map_grid` | Where the client shows on the map | console account |
| `link_check` | Broken and blocked links, counted properly | console account |
| `build_report` | Draft the report | console account |
| `report_sections` | Which report sections are measured | console account |
| `gate_status` | The 24-point pre-ship gate | console account |
| `link_plan` | The link plan | console account |
| `dealer_pack` | What would put a local business ahead | console account |
| `score` | The OnRank Score for an audit | console account |
| `lab_readings` | The Lab's weekly readings for a site | console account |
| `lab_tactics` | What the Lab has tried | console account |
| `queue_email` | Queue an email for approval | console account |

Documentation, how to connect, and how to end a connection: https://onrankseo.com/mcp
