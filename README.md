# Hi, I'm Nexory 👋

## Security Research · SDK Code-Correctness · Open Source Audit

I focus on finding concrete, reproducible bugs in open-source SDKs and developer infrastructure. My work is grounded in deep code reading, adversarial verification, and structured disclosure — not exploit theatre.

Active contributor to ecosystems across DeFi, AI agents, Web3 bridges, fintech SDKs, and developer tooling. I prefer execution over speculation, structured disclosure over hype, and merged contributions over closed PRs.

---

## About Me

My work spans security research, SDK auditing, and open-source contribution across multiple ecosystems.

Focus areas:
- SDK code-correctness audits (TypeScript, Python, Rust, Solidity)
- Async race conditions and lifecycle bugs
- Type-binding drift between SDK declarations and runtime behavior
- OpenAPI generator artifacts and schema validation gaps
- Decimal/precision handling in financial systems
- Responsible disclosure via HackerOne and GitHub Security Advisories

I work in long structured audit sweeps, verify every finding via adversarial 3-lens review, and only file what survives independent confirmation. Reputation over volume.

---

## Tech Stack

### Languages
![TypeScript](https://img.shields.io/badge/TypeScript-0d1117?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-0d1117?style=for-the-badge&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-0d1117?style=for-the-badge&logo=rust&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-0d1117?style=for-the-badge&logo=solidity&logoColor=white)
![Go](https://img.shields.io/badge/Go-0d1117?style=for-the-badge&logo=go&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-0d1117?style=for-the-badge&logo=kotlin&logoColor=white)

### Security & Disclosure
![HackerOne](https://img.shields.io/badge/HackerOne-0d1117?style=for-the-badge&logo=hackerone&logoColor=white)
![GHSA](https://img.shields.io/badge/GHSA-0d1117?style=for-the-badge&logo=github&logoColor=white)
![CVSS%204.0](https://img.shields.io/badge/CVSS%204.0-0d1117?style=for-the-badge)
![CWE](https://img.shields.io/badge/CWE-0d1117?style=for-the-badge)
![Responsible%20Disclosure](https://img.shields.io/badge/Responsible%20Disclosure-0d1117?style=for-the-badge)

### Audit Domains
![DeFi](https://img.shields.io/badge/DeFi-0d1117?style=for-the-badge)
![AI%20Agents](https://img.shields.io/badge/AI%20Agents-0d1117?style=for-the-badge)
![Web3%20Bridges](https://img.shields.io/badge/Web3%20Bridges-0d1117?style=for-the-badge)
![Cross%E2%80%91Chain](https://img.shields.io/badge/Cross--Chain-0d1117?style=for-the-badge)
![Fintech%20SDK](https://img.shields.io/badge/Fintech%20SDK-0d1117?style=for-the-badge)
![Developer%20Tooling](https://img.shields.io/badge/Developer%20Tooling-0d1117?style=for-the-badge)

### Methodology
![Adversarial%20Verification](https://img.shields.io/badge/Adversarial%20Verification-0d1117?style=for-the-badge)
![Multi%E2%80%91Repo%20Pattern%20Hunt](https://img.shields.io/badge/Multi--Repo%20Pattern%20Hunt-0d1117?style=for-the-badge)
![Code%20Reading](https://img.shields.io/badge/Code%20Reading-0d1117?style=for-the-badge)
![Static%20Analysis](https://img.shields.io/badge/Static%20Analysis-0d1117?style=for-the-badge)

---

## Focus Areas

- SDK code-correctness in TypeScript / Python / Rust / Solidity
- Async race conditions and lifecycle bugs
- Type-binding drift between SDK declarations and runtime behavior
- OpenAPI generator artifacts and schema validation gaps
- Decimal/precision handling in financial systems
- Open-redirect, SSRF, and timing-oracle patterns
- Auth-callback routing failures and token-lifecycle violations
- GitHub Security Advisory (GHSA) coordinated disclosure
- HackerOne report drafting (CVSS 4.0, CWE classification)

---

## Selected Contribution Focus

### → SDK Code-Correctness Audits
I audit production-runtime SDKs for concrete code-correctness bugs that affect SDK consumers and downstream applications. The goal is always a 1-3 line fix and a passing test, not a theoretical hazard.

**Recent merged contributions:**
- [`initia-labs/initia.js#168`](https://github.com/initia-labs/initia.js/pull/168) — Cosmos denom regex spec alignment
- [`vercel/turborepo#12976`](https://github.com/vercel/turborepo/pull/12976) — HTTP timeout added to auth path (closed [#12975](https://github.com/vercel/turborepo/issues/12975))

**Active sprints:**
- Polymarket SDK ecosystem (py-sdk, ts-sdk, clob-client-v2)
- Across-protocol (toolkit, relayer, json-constants, sdk)
- Cloudflare OSS (workers-sdk, agents, sandbox-sdk)
- Plaid React Native SDK
- Vercel Tier-1 OSS

---

### → Security Research & Disclosure
I file responsibly via the channel that fits the finding class — HackerOne for in-scope programs, GitHub Security Advisory for direct-to-maintainer coordination, public GitHub Issues for pure code-quality bugs.

**Disclosure principles:**
- Verify every claim via independent code reading + grep + cross-reference
- Calibrate severity conservatively (CVSS 4.0 with reasoned vector)
- Submit one finding per report, no padding
- Include suggested fix and concrete reproduction steps

---

### → Multi-Repo Pattern Hunts
When a bug class appears once, it usually appears across the ecosystem. I systematically hunt the same pattern across related repositories to surface cross-project occurrences and structural causes.

Recent pattern hunts:
- Missing `AbortSignal.timeout()` on critical-path fetches (7 repos surveyed)
- Map/Set leak on consumer unsubscribe (6 repos surveyed)
- Type signature drift on optional fields (multiple SDKs)

---

### → Adversarial Verification
Every finding I file passes through a 3-lens adversarial verification: correctness (does the code actually behave as described), reproducibility (could a maintainer trigger this from the description), and refutation (try to disprove the finding). Only findings surviving 2-of-3 lenses are filed.

This pipeline prioritizes signal quality over volume — I'd rather file 5 reports that all confirm than 50 that maintainers dispute.

---

## Current Direction

Right now, I'm especially focused on:
- Coordinated GHSA disclosure on cross-chain bridge SDKs
- Cloudflare OSS production-runtime audit pass
- Plaid React Native SDK lifecycle and type-binding review
- Building a multi-program signal-pool strategy across HackerOne, GHSA, and direct GitHub

---

## Streak Stats

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Nexory&theme=github-dark-blue&hide_border=true" />
</p>

---

## Contribution Graph

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Nexory&theme=github-dark&hide_border=true&area=true" />
</p>

---

## Profile Views

<p align="left">
  <img src="https://komarev.com/ghpvc/?username=Nexory&label=Profile%20Views&color=0e75b6&style=flat" />
</p>

---

## Reach Out

- **HackerOne:** [hackerone.com/nexory](https://hackerone.com/nexory)
- **Email:** open to coordinated disclosure on private security advisories

If you maintain an SDK and want a focused audit pass, reach out — I work in structured sprints and only file what I can confirm.

---

## Support My Work

If something I've reported helped your project or saved your users from a bug class, consider sponsoring future research:

| Chain | Address |
|---|---|
| **ETH / EVM** (Mainnet, Base, Arbitrum, Optimism, Polygon) | `0xc70d9CAbe1d11Edb126E6be7793D1E09cf5C7F89` |
| **Solana** | `FqDxFXK21qsFamTrFgDAqYXd3L5MNshArf4RD2pbpTt` |
| **Bitcoin** (native SegWit) | `bc1qeepx83cenkjv29q0gvs8g74u7ujfexcgfsn9wc` |

Every contribution funds more research time spent reading code and filing high-signal disclosures.

---

## Additional Information

- **Location:** Europe
- **Background:** Security research, SDK audit, responsible disclosure
- **Work Style:** Long structured sweeps, adversarial verification, conservative severity calibration
- **Interests:** SDK code-correctness, cross-chain bridges, AI agent security, fintech integrity
- **Approach:** Read code carefully, verify aggressively, disclose responsibly
- **Mindset:** Reputation over volume, merged contributions over filed reports

