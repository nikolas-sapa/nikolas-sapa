# Nikolas Sapalidis

Builder + marketer. I ship precise, fast products across developer tools, AI infrastructure, and web apps — and market them the same day. Greece.

![TypeScript](https://img.shields.io/badge/TypeScript-0B0B0D?style=flat-square&logo=typescript&logoColor=F3F2EE)
![Python](https://img.shields.io/badge/Python-0B0B0D?style=flat-square&logo=python&logoColor=F3F2EE)
![Swift](https://img.shields.io/badge/Swift-0B0B0D?style=flat-square&logo=swift&logoColor=F3F2EE)
![Next.js](https://img.shields.io/badge/Next.js-0B0B0D?style=flat-square&logo=nextdotjs&logoColor=F3F2EE)
![React](https://img.shields.io/badge/React-0B0B0D?style=flat-square&logo=react&logoColor=F3F2EE)
![Node.js](https://img.shields.io/badge/Node.js-0B0B0D?style=flat-square&logo=nodedotjs&logoColor=F3F2EE)
![Solidity](https://img.shields.io/badge/Solidity-0B0B0D?style=flat-square&logo=solidity&logoColor=F3F2EE)
![Vercel](https://img.shields.io/badge/Vercel-0B0B0D?style=flat-square&logo=vercel&logoColor=F3F2EE)

**Now:** distributing [ns-ui](https://design.helpmarq.com) · growing [Grip](https://pypi.org/project/grip-browser/) · shipping with `/workflow` agent teams — five agents on one repo, in parallel.

---

### ns-ui — React components, installed as source

[![registry](https://img.shields.io/badge/registry-design.helpmarq.com-006bff?style=flat-square&labelColor=0B0B0D)](https://design.helpmarq.com)
[![license](https://img.shields.io/badge/license-MIT-0B0B0D?style=flat-square&labelColor=0B0B0D)](https://github.com/nikolas-sapa/ns-ui/blob/main/LICENSE)
[![components](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fnikolas-sapa%2Fns-ui%2Fmain%2Fregistry.json&query=%24.items.length&label=components&style=flat-square&labelColor=0B0B0D&color=0B0B0D)](https://github.com/nikolas-sapa/ns-ui)

The project I keep coming back to. Every component is built one at a time around a
single interaction, gated by a Playwright suite that refuses regressions — and it
installs as plain source you own, not a package you depend on.

```bash
npx shadcn add https://design.helpmarq.com/r/gallery-coverflow-caustic.json
```

Tailwind v4 · Motion · react-three-fiber · 542 components across `core` and `loud` ·
CLI + MCP server for agent-driven installs, agent-readable via `/llms.txt`.

**[Browse the registry](https://design.helpmarq.com)** · **[Source](https://github.com/nikolas-sapa/ns-ui)**

---

### Grip — the browser layer for AI agents

[![PyPI](https://img.shields.io/pypi/v/grip-browser?style=flat-square&labelColor=0B0B0D&color=006bff)](https://pypi.org/project/grip-browser/)
[![downloads](https://img.shields.io/pypi/dm/grip-browser?style=flat-square&labelColor=0B0B0D&color=0B0B0D)](https://pypi.org/project/grip-browser/)
[![python](https://img.shields.io/pypi/pyversions/grip-browser?style=flat-square&labelColor=0B0B0D&color=0B0B0D)](https://pypi.org/project/grip-browser/)
[![license](https://img.shields.io/pypi/l/grip-browser?style=flat-square&labelColor=0B0B0D&color=0B0B0D)](https://github.com/nikolas-sapa/grip-browser/blob/main/LICENSE)

A CDP-native browser SDK for AI agents: turns a live page into a semantic snapshot
your agent can act on — median ~2k tokens instead of ~59k of raw HTML (16× smaller),
and 5× smaller than Playwright MCP. No Playwright, no Puppeteer — raw Chrome DevTools
Protocol with stable element refs, shadow-DOM traversal, a prompt-injection guard,
and typed error recovery.

```bash
pip install grip-browser
```

The [benchmark page](https://grip-browser.vercel.app) publishes the full run,
including the round Grip lost, the structural cause behind it, and the 30/30 re-run.

**[PyPI](https://pypi.org/project/grip-browser/)** · **[Site + benchmarks](https://grip-browser.vercel.app)** · **[Source](https://github.com/nikolas-sapa/grip-browser)**

---

### Developer tools & AI infrastructure

| Project | What it does | Try it |
|---|---|---|
| [**branch-ai**](https://github.com/nikolas-sapa/branch-ai) | Reasoning canvas for AI CLIs — capture Claude Code / Codex / Gemini extended thinking as a navigable, forkable tree | `npm i -g branch-ai` · [demo](https://branchai-fawn.vercel.app) |
| [**skillswitch**](https://github.com/nikolas-sapa/skillswitch) | Manage AI-coding skills across Claude Code, Gemini CLI, Codex, Aider, Amp & Droid — stop 100 skills bloating your context window | `npm i -g skillswitch` · [site](https://skillswitch-landing.vercel.app) |
| [**clientcast**](https://github.com/nikolas-sapa/clientcast) | Turn Git commits into AI-drafted client updates; classify replies, flag scope creep, invoice flagged work via Stripe | `npm i -g clientcast` · [site](https://clientcast-landing.vercel.app) |
| [**toolfence**](https://github.com/nikolas-sapa/toolfence) | Security scanner for MCP servers — flags tool poisoning, prompt injection, drift, scope & cost before your agents connect | `npx toolfence <url>` · [site](https://mcpguard-site.vercel.app) |
| [**sigeval**](https://github.com/nikolas-sapa/sigeval) | pytest for LLMs that isn't flaky — significance-tested eval regression gates so you don't ship on noise | [docs](https://nikolas-sapa.github.io/sigeval/) |
| [**helm**](https://github.com/nikolas-sapa/helm) | Deploy + governance control plane for internal AI agents — ship an agent in one command; IT scopes its tools, caps token spend, kills it on demand | [site](https://helm-internal-agent-platform.vercel.app) |
| [**agentic-pipeline**](https://github.com/nikolas-sapa/agentic-pipeline) | Event-driven LLM request pipeline (Postgres queue, idempotent ingress, retry/DLQ/replay) — plus the benchmark that killed its own cost-routing feature | [repo](https://github.com/nikolas-sapa/agentic-pipeline) |
| [**x402-bounty-radar**](https://x402-bounty-radar.nikolas-sapalidis.workers.dev) | Paid API for real, funded GitHub bounties — scam-filtered, competition-scored, $0.01/call in USDC via x402, no key, no KYC | [live](https://x402-bounty-radar.nikolas-sapalidis.workers.dev) |

### SaaS & web products

| Project | What it does | Live |
|---|---|---|
| [**neurolens**](https://github.com/nikolas-sapa/neurolens) (NeuroPulse) | Score any ad — image, video, or copy — across 8 brain regions before you spend a dollar promoting it. Open-source, self-hostable | [neurolens-nine.vercel.app](https://neurolens-nine.vercel.app) |
| **marketmyapp** | Marketing health score for indie founders — find out what's broken before your launch does | [marketmyapp.vercel.app](https://marketmyapp.vercel.app) |
| **creator-roast** | AI profile audit — scores, grades, and a ranked fix list to get brand-deal ready | [creator-roast.vercel.app](https://creator-roast.vercel.app) |
| **helpmarq** | Honest, structured project feedback from real users in 48 hours. Free tier | [helpmarq.com](https://helpmarq.com) |

### Consumer apps

| Project | What it does | Live |
|---|---|---|
| **noctiq** | AI sleep coach — reads HealthKit + Oura / WHOOP / Garmin and tells you exactly what to change | [noctiq-site.vercel.app](https://noctiq-site.vercel.app) |
| **padelup** | AI padel coaching — video analysis, training plans, court finder | [trypadelup.com](https://trypadelup.com) |
| **ugc-engine** | AI-UGC system — generate, score, and improve short-form video + carousels that learn from every post | [ugc-engine-site.vercel.app](https://ugc-engine-site.vercel.app) |

### On-chain

| Project | What it does | |
|---|---|---|
| [**sac-capital**](https://github.com/nikolas-sapa/sac-capital) | Verifiable AI trading agent — multi-stage LLM equity research with on-chain bytes32 commitments on Mantle, paper execution, full audit trail | [sapa-fund.vercel.app](https://sapa-fund.vercel.app) |
| [**curb**](https://github.com/nikolas-sapa/curb) | Your bank card has a daily limit, your wallet doesn't — a Monad vault that caps daily outflow: lowering is instant, raising is timelocked | [curb-pink.vercel.app](https://curb-pink.vercel.app) |

---

### Open source

| Contribution | Repo | Status |
|---|---|---|
| Reported [GHSA-c3rg-jwq9-3233](https://github.com/get-convex/convex-auth/security/advisories/GHSA-c3rg-jwq9-3233) — sign-in rate limiting bypass in `@convex-dev/auth` allowing verification-code brute force. CVSS 7.4 (High), patched in 0.0.95, credited reporter | Convex | published |
| Warn about unsupported requested entities in `/analyze` while preserving partial results ([#2259](https://github.com/data-privacy-stack/presidio/pull/2259)) | Microsoft Presidio | merged |
| Document `RECOGNIZER_REGISTRY_CONF_FILE` override for the analyzer server ([#2311](https://github.com/data-privacy-stack/presidio/pull/2311)) | presidio | merged |

Active in issues and PRs across `oven-sh/bun`, `traefik/traefik`, `mastra-ai/mastra`,
`withastro/astro`, `modelcontextprotocol/typescript-sdk`, `dottxt-ai/outlines`,
`adaptive-machine-learning/CapyMOA`, `gofr-dev/gofr`, and the `unjs` ecosystem.

---

### Links

[nikolas.helpmarq.com](https://nikolas.helpmarq.com) · [X @NikolasSapa](https://x.com/NikolasSapa)
