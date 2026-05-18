<p align="center">
  <a href="https://orbitkit.io">
    <img src="https://orbitkit.io/assets/brand/orbitkit-icon-512.png" alt="OrbitKit" width="96">
  </a>
</p>

<h1 align="center">OrbitKit</h1>

<p align="center"><strong>The web layer for Apple platform apps.</strong></p>

<p align="center">
  <a href="https://orbitkit.io">Website</a> &nbsp;·&nbsp;
  <a href="https://orbitkit.io/api">API Docs</a> &nbsp;·&nbsp;
  <a href="https://orbitkit.io/dashboard">Dashboard</a> &nbsp;·&nbsp;
  <a href="https://orbitkit.io/blog">Blog</a>
</p>

---

Apple's App Store Review requires a surprising number of **web URLs** before your app can ship — a privacy policy page, a support page, a data‑deletion page, an Apple App Site Association (AASA) file for Universal Links, a privacy manifest, and more. OrbitKit generates every one of them, hosts them on your own domain, and keeps them in sync with your app.

- **Privacy policy** — an Apple‑compliant policy from a guided wizard
- **Support & data‑deletion pages** — the URLs App Review asks for
- **AASA / well‑known files** — Universal Links, App Clips, Sign in with Apple
- **Privacy manifest** — generated from your policy answers
- **Custom domains** — host it all under your own domain with managed SSL

## Open source

| Project | What it is | Install |
|---|---|---|
| [**OrbitKit CLI**](https://github.com/OrbitKit-io/OrbitKit-CLI) | Manage apps, policies & deploys from the terminal or CI | `npm i -g @orbitkit-io/cli` |
| [**OrbitKit Deploy**](https://github.com/OrbitKit-io/OrbitKit-Deploy) | GitHub Action to deploy your app site from CI/CD | `uses: OrbitKit-io/OrbitKit-Deploy@v1` |

Both are [Apache‑2.0](https://www.apache.org/licenses/LICENSE-2.0) licensed.

## AI agents (MCP)

OrbitKit runs a **hosted MCP server** so Claude, Cursor, and other [Model Context Protocol](https://modelcontextprotocol.io) clients can manage your App Store compliance pages directly. Add it in one line:

```bash
claude mcp add --transport http orbitkit https://mcp.orbitkit.io/mcp \
  --header "Authorization: Bearer ok_YOUR_API_KEY"
```

Or point any MCP client at `https://mcp.orbitkit.io/mcp` with an `Authorization: Bearer ok_…` header. Full setup & tool reference: **[orbitkit.io/api/mcp-server](https://orbitkit.io/api/mcp-server/)**.

## Get started

The first app is free for 30 days — set it up at **[orbitkit.io](https://orbitkit.io)**.

<p align="center"><sub>© OrbitKit, Inc. &nbsp;·&nbsp; <a href="mailto:help@orbitkit.io">help@orbitkit.io</a></sub></p>
