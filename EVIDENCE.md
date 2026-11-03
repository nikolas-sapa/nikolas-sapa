# Nikolas Sapalidis: full text and sources

Profile snapshot: November 3, 2026. Counts are dated snapshots, not live counters.

## About

17. Greece. Self-taught since January 2026.

I build tools for AI agents and fix bugs in the tools I use.

## Selected builds

### ns-ui

542 React components. Install the source. Make it yours.

A shadcn-compatible registry with a CLI and MCP server. Components are installed as source you can edit.

- [Source and documentation](https://github.com/nikolas-sapa/ns-ui)
- [Live component registry](https://design.helpmarq.com)

The live registry contained 542 components when checked on November 3, 2026. This is a component count, not an install or user count.

### Grip

A CDP-native browser SDK for AI agents. Compact page snapshots. Typed error recovery.

Python SDK built directly on Chrome DevTools Protocol. Published on PyPI.

- [Source and documentation](https://github.com/nikolas-sapa/grip-browser)
- [PyPI package](https://pypi.org/project/grip-browser/)
- [Website](https://grip-browser.vercel.app)
- [Published competitor benchmark](https://github.com/nikolas-sapa/grip-browser/blob/main/benchmarks/RESULTS_COMPETITORS.md)
- [Comparison where browser-use produces smaller snapshots](https://github.com/nikolas-sapa/grip-browser/blob/main/benchmarks/RESULTS_BROWSERUSE.md)

The published eight-page benchmark, dated August 10, 2026, reports a median of 1,998 snapshot tokens. Median per-page reductions were 16× versus raw HTML and 5× versus Playwright MCP. These measure snapshot payload size. They do not measure actual cost, task success or end-to-end agent performance.

The browser-use comparison uses different page coverage, explained in that report. Its unfavorable result is retained alongside the larger benchmark.

### branch-ai

Turn surfaced AI reasoning into a tree you can revisit and fork.

Published CLI version 1.1.0 was verified on npm for this snapshot.

- [Source and documentation](https://github.com/nikolas-sapa/branch-ai)
- [npm package](https://www.npmjs.com/package/branch-ai)
- [Hosted demo](https://branchai-fawn.vercel.app)

The tree contains reasoning surfaced by supported tools. It does not expose hidden cognition. Revisit and fork describe the captured tree and available workflows, not exact restoration of a model's internal state. The hosted demo is read-only; local viewer and integration capabilities require the local setup described in the repository.

### skillswitch

Switch coding-agent skill sets without deleting them.

Published CLI version 0.2.0 was verified on npm for this snapshot.

- [Source and documentation](https://github.com/nikolas-sapa/skillswitch)
- [npm package](https://www.npmjs.com/package/skillswitch)

Basic skill management supports six CLI targets. Profiles, catalog and audit features are Claude-only. No measured context-saving claim is made.

These four projects were selected after a review of 12 current project READMEs. The selection emphasizes a tangible component registry, browser tooling, captured reasoning and skill management. It is a documentation-based curation, not a full code audit.

## Merged fixes upstream

35 merged pull requests across 14 external repositories, excluding two directory-listing PRs. Including those listings: 37 merged PRs across 16 external repositories. Snapshot: November 3, 2026. Own repositories are excluded from both upstream totals.

- [Full merged external PR history](https://github.com/search?q=is%3Apr+author%3Anikolas-sapa+is%3Amerged+-user%3Anikolas-sapa&type=pullrequests)

Featured fixes:

- [WebdriverIO #15595](https://github.com/webdriverio/webdriverio/pull/15595): Crashed test workers must fail the run.
- [sktime #11307](https://github.com/sktime/sktime/pull/11307): Stop `fit()` reseeding NumPy's global RNG.
- [Astro #18085](https://github.com/withastro/astro/pull/18085): Make Vercel redirects respect `trailingSlash`.

The aggregate includes fixes, features, tests and documentation. It is separate from the GitHub contribution totals below.

## Security advisory

Credited reporter. Convex Auth. High severity. Patched in 0.0.95.

- [GHSA-c3rg-jwq9-3233](https://github.com/get-convex/convex-auth/security/advisories/GHSA-c3rg-jwq9-3233)

The advisory is the source for the credit, severity and patched version. No broader impact claim is made here.

## Research

### When summaries go stale

2,631 runs studying when stale summaries overrule fresh evidence.

Templated provenance helped. Model-written compaction remained unresolved.

- [Resumed-agent staleness: report, public transcripts and reproduction material](https://github.com/nikolas-sapa/resumed-agent-staleness)

The study examines resumed agents acting on stale checkpoint summaries after checking live data. The repository includes preregistrations, transcripts, analysis, corrections and limits.

In the tested setup, templated provenance summaries reduced stale writes. Provenance instructions for model-written compaction did not resolve the problem. The report retains failed approaches and scorer corrections. This is not an externally replicated result or a demonstrated production fix.

## A short history

- April 2025: Foodsave, a near-expiry food marketplace concept. Solo entry, top 5 of 100+ teams in the Crazy Business Ideas entrepreneurship contest.
- January 2026: Started teaching myself to code.
- February 2026: First paying website client.
- September 2026: Four paying clients and about €2,000 earned.

Earlier study: SCAT Advanced Quantitative in 2024; CTY Greece Probability & Game Theory in June 2024; Economics & Entrepreneurship in January 2025.

Personal chronology and client totals are self-reported. No client identities or private supporting material are published here.

## Counting notes

### GitHub: January 1 through November 3, 2026

- 3,926 contributions.
- 433 pull-request contributions.
- 85 repositories with pull-request contributions.
- Includes own repositories.

[Contribution history](https://github.com/nikolas-sapa?tab=overview&from=2026-01-01&to=2026-11-03)

Source: GitHub GraphQL `user(login: "nikolas-sapa")`, queried November 3, 2026, using `contributionsCollection(from: "2026-01-01T00:00:00Z")`.

Fields: `contributionCalendar.totalContributions`, `totalPullRequestContributions`, `totalRepositoriesWithContributedPullRequests`.

[GitHub contributions collection documentation](https://docs.github.com/en/graphql/reference/objects#contributionscollection)

433 PR contributions is not an upstream merge count. The separate external merged-PR total is 35/14, or 37/16 including the two directory listings.

### npm: November 3, 2025 through November 3, 2026

- [branch-ai: 1,090 downloads](https://api.npmjs.org/downloads/point/2025-11-03:2026-11-03/branch-ai)
- [skillswitch: 1,160 downloads](https://api.npmjs.org/downloads/point/2025-11-03:2026-11-03/skillswitch)
- [clientcast: 553 downloads](https://api.npmjs.org/downloads/point/2025-11-03:2026-11-03/clientcast)
- Total: 2,803 downloads across those three packages.

Registry downloads include CI and automated installs. They are not unique users. These links query the stated date range; the profile records the counts checked on November 3, 2026.

## Contact

- [Website](https://nikolassapalidis.tech)
- [X: @NikolasSapa](https://x.com/NikolasSapa)

## Reading and motion

This page provides the image profile's text as selectable, searchable Markdown. Each project, PR, advisory, research panel and contact strip has its own outer link in the profile.

Every animated profile image has a separate static SVG selected by an outer `picture` source for `prefers-reduced-motion: reduce`. SVGs also contain a CSS reduced-motion fallback. Name geometry comes from the original banner, retained unchanged as `banner.svg`. All artwork is self-contained vector SVG, without scripts or external font requests.
