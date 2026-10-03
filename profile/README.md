<p align="center"><img src="mark.svg" width="88" alt="ProspectAPIs compass-star logo"></p>

# ProspectAPIs

**Funding signals and cited prospect research over one REST API**, for sales teams and the AI agents that work for them. Every fact comes back with the source link that states it.

[Create a free account](https://prospectapis.com/signup) · [Docs](https://prospectapis.com/docs) · [Pricing](https://prospectapis.com/pricing) · [MCP server](https://github.com/ProspectAPIs/prospectapis-mcp)

## What you can do

- **Find companies that just raised.** Search funding rounds by date, round, amount, company, domain, investor and country, newest first.
- **Watch for new rounds.** Save a search as a watchlist and get each new matching round delivered to your webhook.
- **Research an account or a person.** Send one identifier (a domain, a work email, a LinkedIn URL, or a name with a company) and get a structured brief in about 20 to 90 seconds, each field with its sources and a confidence score.
- **Call it from an agent.** Run the MCP server in Claude, Cursor, Windsurf or VS Code with the same key, credits and prices as the REST API.

## Pricing

| What | Price |
|---|---|
| Funding records (`GET /v1/funding`) | $0.02 per record returned, after 100 free records a month; a search that matches nothing is free |
| Watchlist deliveries | $0.02 per delivered record, from the same 100 free records a month; creating and managing watchlists is free |
| Research briefs (`POST /v1/research`) | $0.15 per completed brief; a failed brief is refunded |

Prepaid credits, 1:1 with dollars, no seats and no subscription. The live price list is always at `GET https://api.prospectapis.com/pricing`.

## Start here

| Resource | Link |
|---|---|
| Create a free account | https://prospectapis.com/signup |
| Quickstart | https://prospectapis.com/docs |
| Funding signals API | https://prospectapis.com/docs/funding |
| Watchlists API | https://prospectapis.com/docs/watchlists |
| Prospect research API | https://prospectapis.com/docs/research |
| MCP server | https://github.com/ProspectAPIs/prospectapis-mcp |
| Blog | https://prospectapis.com/blog |

## FAQ

**Is there a free tier?** Every account gets 100 funding records free each month. After that you pay per record from prepaid credits.

**Which MCP clients work?** Claude Desktop, Claude Code, Cursor, Windsurf and VS Code, or any client that speaks the Model Context Protocol. Install with `npx -y prospectapis-mcp` and set `PROSPECTAPIS_API_KEY`.

**Where do the facts come from?** Public sources. Each field in a research brief carries the links that state it, and a field the sources do not support comes back empty rather than guessed.
