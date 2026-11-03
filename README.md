<img src="banner.svg" alt="Nikolas Sapalidis" width="622">

17 · Greece · self-taught since January 2026.

I build tools for AI agents and fix bugs in the tools I use.
Sometimes the bug is in the benchmark. That gets published too.

<img src="assets/field-notes.svg" alt="Field notes: a folded graphite wave, rendered in ordered dither with a blue seam." width="100%">

[Builds](#things-ive-shipped) · [Merged fixes](#fixes-that-landed-upstream) · [Research](#experiments-with-the-receipts) · [Numbers](#by-the-numbers) · [Contact](#say-hello)

`TypeScript` · `Python` · `Swift` · `React / Next.js`

## Things I've shipped

<img src="assets/builds.svg" alt="Selected builds: ns-ui, components you keep; Grip, less DOM, more context; branch-ai, a debugger for the reasoning tree." width="100%">

### ns-ui

A shadcn-compatible registry of 542 React components, installed as source you own.
Includes a CLI and MCP server so coding agents can find and install components.

[Browse components](https://design.helpmarq.com) · [Source](https://github.com/nikolas-sapa/ns-ui)

<details>
<summary>Install a component · stack</summary>

```bash
npx shadcn add https://design.helpmarq.com/r/gallery-coverflow-caustic.json
```

Tailwind v4 · Motion · react-three-fiber · agent-readable via `/llms.txt`.

</details>

### Grip

A Python browser SDK built directly on Chrome DevTools Protocol. It gives agents
compact semantic snapshots, stable element references, shadow-DOM traversal,
and typed error recovery. No Playwright or Puppeteer dependency.

[PyPI](https://pypi.org/project/grip-browser/) · [Site](https://grip-browser.vercel.app) · [Source](https://github.com/nikolas-sapa/grip-browser)

<details>
<summary>Install · eight-page benchmark · the comparison I lost</summary>

```bash
pip install grip-browser
```

In the published eight-page benchmark (August 10, 2026), snapshots used a median
1,998 tokens. The median per-page reduction was 16× versus raw HTML and 5× versus
Playwright MCP. These measure snapshot size, not task success or end-to-end cost.

[Benchmark data](https://github.com/nikolas-sapa/grip-browser/blob/main/benchmarks/RESULTS_COMPETITORS.md) ·
[The comparison where browser-use is smaller](https://github.com/nikolas-sapa/grip-browser/blob/main/benchmarks/RESULTS_BROWSERUSE.md)
(different page coverage, explained in the report).

</details>

### branch-ai

Capture extended thinking from AI coding CLIs as a navigable, forkable tree.
Rewind to a node, fork it, and explore another direction. Local-first, with an MCP server.

[Demo](https://branchai-fawn.vercel.app) · [Source](https://github.com/nikolas-sapa/branch-ai) · `npm i -g branch-ai`

## Fixes that landed upstream

35 merged PRs across 14 other projects, covering fixes, features, tests, and docs.
Including two directory-listing PRs: [37 merges across 16 repositories](https://github.com/search?q=is%3Apr+author%3Anikolas-sapa+is%3Amerged+-user%3Anikolas-sapa&type=pullrequests).

| Project | What changed |
|---|---|
| WebdriverIO | [A signal-terminated worker must fail the run, not pass it (#15595)](https://github.com/webdriverio/webdriverio/pull/15595) |
| sktime | [`BaggingClassifier.fit()` must not reseed NumPy's process-global RNG (#11307)](https://github.com/sktime/sktime/pull/11307) |
| Astro | [Vercel redirects must respect `trailingSlash: always/never` (#18085)](https://github.com/withastro/astro/pull/18085) |
| Traefik | [Add a global default for `aliasHeadersStrategy` (#13919)](https://github.com/traefik/traefik/pull/13919) |
| ESLint Stylistic | [Align parenthesized type values from the opening parenthesis (#1283)](https://github.com/eslint-stylistic/eslint-stylistic/pull/1283) |
| Cap | [Optimize screenshot alpha checks, flattening, and premultiplication (#2673)](https://github.com/CapSoftware/Cap/pull/2673) |
| CapyMOA | [Add the EDDM drift detector (#422)](https://github.com/adaptive-machine-learning/CapyMOA/pull/422) |
| Presidio | [Preserve partial results when requested entities are unsupported (#2259)](https://github.com/data-privacy-stack/presidio/pull/2259) |

Also the credited reporter of [GHSA-c3rg-jwq9-3233](https://github.com/get-convex/convex-auth/security/advisories/GHSA-c3rg-jwq9-3233):
a high-severity sign-in rate-limiting bypass in Convex Auth, patched in `0.0.95`.

## Experiments, with the receipts

[Resumed-agent staleness](https://github.com/nikolas-sapa/resumed-agent-staleness):
a pre-registered, 2,631-run study of agents acting on stale checkpoint summaries
after checking live data. Includes transcripts, analysis, and reproduction instructions.

In the tested setup, templated provenance summaries reduced stale writes;
provenance instructions for model-written compaction did not.
The report documents the failed approaches and scorer corrections too.

## By the numbers

<img src="assets/activity.svg" alt="2026 GitHub snapshot, November 3: 3,923 contributions, 432 PR contributions, 85 repositories with PR contributions. Includes my own repositories." width="100%">

Snapshot: **November 3, 2026**. Since January 1: **3,923 contributions**, **432 PR contributions**,
**85 repositories with PR contributions**, including my own repositories.
[GitHub contribution history](https://github.com/nikolas-sapa?tab=overview&from=2026-01-01&to=2026-11-03).

Three npm tools, **2,803 downloads** from **November 3, 2025 through November 3, 2026**:
[branch-ai: 1,090](https://api.npmjs.org/downloads/point/2025-11-03:2026-11-03/branch-ai) ·
[skillswitch: 1,160](https://api.npmjs.org/downloads/point/2025-11-03:2026-11-03/skillswitch) ·
[clientcast: 553](https://api.npmjs.org/downloads/point/2025-11-03:2026-11-03/clientcast).
Registry downloads include CI and automated installs; they are not unique users.

<details>
<summary>Counting method</summary>

GitHub source: GraphQL `user(login: "nikolas-sapa")` →
[`contributionsCollection(from: "2026-01-01T00:00:00Z")`](https://docs.github.com/en/graphql/reference/objects#contributionscollection),
queried November 3, 2026. Fields: `contributionCalendar.totalContributions`,
`totalPullRequestContributions`, `totalRepositoriesWithContributedPullRequests`.
These are contribution counts, not an upstream-only total.

Upstream merges are counted separately above, excluding my own repositories.
The 35-PR / 14-repository figure also excludes two directory-listing PRs;
the full figure is 37 / 16. npm links return the stated rolling-period download counts.

</details>

---

<details>
<summary><code>ls ~/projects</code> · more developer tools</summary>

| Project | What it does | Try it |
|---|---|---|
| [skillswitch](https://github.com/nikolas-sapa/skillswitch) | Toggle coding-agent skills and save per-project profiles | `npm i -g skillswitch` |
| [clientcast](https://github.com/nikolas-sapa/clientcast) | Draft client updates from commits; classify replies and flag scope creep | `npm i -g clientcast` |
| [toolfence](https://github.com/nikolas-sapa/toolfence) | Scan MCP servers for tool poisoning, prompt injection, drift, and scope risks | `npx toolfence <url>` |
| [sigeval](https://github.com/nikolas-sapa/sigeval) | LLM evaluation gates with confidence intervals: PASS / FAIL / INCONCLUSIVE | [Docs](https://nikolas-sapa.github.io/sigeval/) |
| [helm](https://github.com/nikolas-sapa/helm) | Deployment and governance for internal agents, with tool scopes and spend limits | [Site](https://helm-internal-agent-platform.vercel.app) |
| [agentic-pipeline](https://github.com/nikolas-sapa/agentic-pipeline) | Postgres-backed LLM request queue with retries, dead letters, and replay | [Source](https://github.com/nikolas-sapa/agentic-pipeline) |
| [x402-bounty-radar](https://github.com/nikolas-sapa/x402-bounty-radar) | Funded GitHub bounties ranked by competition and freshness | [API](https://x402-bounty-radar.nikolas-sapalidis.workers.dev) |

</details>

<details>
<summary><code>ls ~/experiments</code> · web products, consumer apps, and on-chain work</summary>

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

</details>

<details>
<summary><code>git log --reverse</code> · before the open-source PRs</summary>

| When | What I was building |
|---|---|
| 2024–2025 | SCAT Advanced Quantitative; CTY Greece courses in Probability & Game Theory and Economics & Entrepreneurship. |
| April 2025 | Foodsave, a near-expiry food marketplace concept. Solo entry, top 5 of 100+ teams in the Crazy Business Ideas entrepreneurship contest. |
| January 2026 | Started teaching myself to code. |
| February 2026 | First paying website client. Four paying clients and about €2,000 earned by September. |
| July 2026 | Launched PadelUp, my own AI padel-coaching iOS app, on the App Store. |
| September 2026 | First merged upstream PR: making WebdriverIO report crashed workers as failures. |

</details>

<details>
<summary><code>cat .debug/notes</code></summary>

```diff
- The test is green. Ship it.
+ Break the target. Does the test turn red?
```

WebdriverIO's crashed workers used to pass.
My browser benchmarks include a comparison I lost.
You can probably guess why this is here.

```text
418 I'm a teapot
200 You found the bottom of the README
```

</details>

## Say hello

[Website](https://nikolassapalidis.tech) · [X @NikolasSapa](https://x.com/NikolasSapa)

<!-- Reading the raw Markdown? The ASCII banner is a protected species. -->
