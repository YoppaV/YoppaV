<h1 align="center">Juan Rodríguez</h1>

<p align="center">
  <em>Read-only interfaces between the web and Claude.</em>
</p>

<p align="center">
  <sub>Madrid · 2026</sub>
</p>

---

### What I'm building

```mermaid
flowchart LR
    classDef public stroke:#2ea043,stroke-width:2px,color:#2ea043
    classDef private stroke:#888,stroke-dasharray:3 3,color:#888

    twitter[twitter-mcp]:::public
    polymarket[polymarket-mcp]:::public
    linkedin[linkedin-mcp]:::private
    instagram[instagram-mcp]:::private
    reddit[reddit-mcp]:::private

    twitter    --> claude{{Claude}}
    polymarket --> claude
    linkedin   --> claude
    instagram  --> claude
    reddit     --> claude

    twitter   --> ingest[social-ingest]
    instagram --> ingest
    ingest    --> vault[(Obsidian)]
```

### Public

- **[twitter-mcp](https://github.com/YoppaV/twitter-mcp)** — read-only Twitter/X for Claude. 17 tools, Playwright + GraphQL interception.
- **[polymarket-mcp](https://github.com/YoppaV/polymarket-mcp)** — Polymarket research MCP. 21 tools across 4 tiers: wallet forensics, market metadata, cross-wallet correlation.

### /now

Wiring agent workflows that read from social platforms and prediction markets, then route the interesting bits into a personal knowledge graph. Quietly figuring out which of these are worth open-sourcing next.

<sub><code>Python</code> · <code>Playwright</code> · <code>FastMCP</code> · <code>TypeScript</code> · <code>Go</code> · <code>Postgres</code></sub>
