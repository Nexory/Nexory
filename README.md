# Hi, I'm Andre ✌🏻

[![GitHub Contribution Stats](https://raw.githubusercontent.com/Nexory/Nexory/main/card.svg)](https://github.com/Nexory/BugMergeStats)

I'm a developer from Germany. By day I do quantitative research on prediction markets (mostly Polymarket microstructure and orderbook stuff). On the side I read a lot of open-source code and file the bugs I find, which is what most of the activity on this profile is about.

## Background

My path was not the standard "CS undergrad straight into a SWE job" one:

- Three-year vocational programme in business IT (German qualification: *Kaufmännischer Assistent zur Informationsverarbeitung*)
- Higher-education entrance qualification (German: *Fachhochschulreife*)
- Started a Bachelor in Informatics out of curiosity, dropped out without finishing because I learned more building real systems than working through the curriculum

I'm self-taught in everything that matters for what I do now. Reading unfamiliar codebases carefully is a big part of how I learn, and the contribution sprints on this profile are mostly that practice spilling outwards.

## What I work on here

The card above counts what's actually visible: issues filed in public repos and PRs maintainers wrote to fix them. I try to write each report well enough that the maintainer can ship the fix without follow-up questions.

A few categories I keep coming back to:

- TypeScript / Python / Rust / Solidity SDK code-correctness: async race conditions, lifecycle bugs, decimal precision, type-binding drift between SDK declarations and runtime behaviour
- OpenAPI generator artefacts (missing enum cases, schema validation gaps)
- Auth callback routing failures and token-lifecycle issues
- HackerOne reports and coordinated GHSA disclosure for security findings

## A few recent ones that landed

- [ProjectOpenSea/tool-sdk#9](https://github.com/ProjectOpenSea/tool-sdk/issues/9) -> [PR #10](https://github.com/ProjectOpenSea/tool-sdk/pull/10): a predicate auth-gate accepted an unbounded, non-expiring payment proof because `validBefore` was optional; reported with a matching fix and a failing-then-passing test, recreated by the maintainers and shipped in `@opensea/tool-sdk@0.16.1` with credit in the release notes
- [ProjectOpenSea/opensea-js#1976](https://github.com/ProjectOpenSea/opensea-js/pull/1976): a `cancelOrders` batch spanning two Seaport protocol addresses silently left half the orders fillable; recreated by the maintainers and shipped in v11.2.0
- [opencart/opencart#15540](https://github.com/opencart/opencart/pull/15540): switched API signature validation to constant-time `hash_equals()`, merged into master
- [dojo/dojo#461](https://github.com/dojo/dojo/pull/461): guarded the final `setObject` path segment against prototype pollution, merged into master
- [web2py/web2py#2650](https://github.com/web2py/web2py/pull/2650): timing-safe compare for the CSRF formkey check, merged into master
- [vercel/ai#15708](https://github.com/vercel/ai/issues/15708) -> [PR #15734](https://github.com/vercel/ai/pull/15734): `safeValidateTypes` was discarding validated elements in array output, fixed by a maintainer-merged PR
- [vercel/turborepo#12975](https://github.com/vercel/turborepo/issues/12975) -> [PR #12976](https://github.com/vercel/turborepo/pull/12976): the auth flow used a reqwest client with no timeouts and could hang the CLI, fixed and shipped in a same-day canary

The full list lives in the issues and PRs tabs on this account.

## A note on AI

Yes, I use Claude Opus for a lot of my issue and PR drafting and for the verification passes that run before I file anything. It's a tool I rely on the same way I rely on an IDE or a linter.

If you maintain a project I've reported on and you'd rather not receive AI-assisted reports, just say so on any of my issues or PRs and I'll stop on your repo. I'd rather lose a finding than burn a maintainer relationship over disclosure style.

I sign every commit with my SSH key (`ED25519 SHA256:CWX60WPoOQcianliIELliGtEftFs9vEnkLmywphAUP8`) and read everything I push. AI does the heavy code reading and drafting; the call to file and the responsibility for what gets filed are mine.

## Reach out

- HackerOne: [hackerone.com/nexory](https://hackerone.com/nexory)
- Email for coordinated disclosure: visible on my GitHub profile sidebar

## If you want to sponsor research time

Sometimes useful for a maintainer who'd like to send a thank-you for a finding, or just if something here helped you.

| Chain | Address |
|---|---|
| ETH / EVM (Mainnet, Base, Arbitrum, Optimism, Polygon) | `0xc70d9CAbe1d11Edb126E6be7793D1E09cf5C7F89` |
| Solana | `FqDxFXK21qsFamTrFgDAqYXd3L5MNshArf4RD2pbpTt` |
| Bitcoin (native SegWit) | `bc1qeepx83cenkjv29q0gvs8g74u7ujfexcgfsn9wc` |
