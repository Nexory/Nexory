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

The card above counts what's actually visible: issues filed in public repos and PRs maintainers wrote to fix them. It undercounts on purpose, because a good part of the work never becomes a public artefact at all. Where a project asks for private reporting, the finding goes to that channel and stays there until they say otherwise.

The areas I keep coming back to:

- **Memory safety in C parsers**: image and archive formats, where a length field is trusted one line before it is validated. Box parsing in AVIF, TIFF and PNG decoders, cpio and bzip2 headers, filesystem tooling.
- **Java deserialization and XML**: JEP-290 filters on remember-me style cookies, XXE in transformers, class-resolution gaps in RPC layers.
- **Crypto correctness**: certificate serial numbers that come out negative half the time, TLS contexts that verify nothing because a parameter defaulted, timing-unsafe comparisons on secrets, S/MIME structures re-encoded before they are checked.
- **Prototype pollution and injection in web frameworks**: direct property writes that accept `__proto__`, path segments that skip a denylist the sibling function applies.
- **PHP CMS and e-commerce**: signature validation, upload paths, permission checks.

## How I file

The rule I hold myself to is that nothing goes out that I have not reproduced first. In practice that means a test which fails without the fix **for the right reason**, passes with it, and both outputs written to disk rather than remembered. Then the full suite for regressions, and a run inside the project's own CI image where there is one, because "green on my machine" only proves my machine is tolerant.

I also try to be honest about the parts I did not measure. If exploitability rests on an assumption I could not test, that sentence goes into the report as an assumption, not as a finding. A report that overstates its own reach costs the maintainer more time than it saves.

Before anything is filed I check the project's own rules rather than my habits: where security reports are supposed to go, whether a CLA or DCO applies, whether the project even merges external contributions. Routing follows the written policy, not my read of the bug class.

## A note on AI

Yes, I use Claude Opus for a lot of my issue and PR drafting and for the verification passes that run before I file anything. It's a tool I rely on the same way I rely on an IDE or a linter.

If you maintain a project I've reported on and you'd rather not receive AI-assisted reports, just say so on any of my issues or PRs and I'll stop on your repo. I'd rather lose a finding than burn a maintainer relationship over disclosure style.

I sign every commit with my SSH key (`ED25519 SHA256:CWX60WPoOQcianliIELliGtEftFs9vEnkLmywphAUP8`) and read everything I push. AI does the heavy code reading and drafting; the call to file and the responsibility for what gets filed are mine.

## Reach out

For coordinated disclosure, or if you maintain something I've reported on: the email address in the sidebar of this profile.

## If you want to sponsor research time

Sometimes useful for a maintainer who'd like to send a thank-you for a finding, or just if something here helped you.

| Chain | Address |
|---|---|
| ETH / EVM (Mainnet, Base, Arbitrum, Optimism, Polygon) | `0xc70d9CAbe1d11Edb126E6be7793D1E09cf5C7F89` |
| Solana | `FqDxFXK21qsFamTrFgDAqYXd3L5MNshArf4RD2pbpTt` |
| Bitcoin (native SegWit) | `bc1qeepx83cenkjv29q0gvs8g74u7ujfexcgfsn9wc` |
