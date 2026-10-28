# Offensive security for the swarm.

Independent security researcher working on multi-agent and embodied AI. Founder of **MASec Lab**, which builds offensive tooling and audit methodology for how AI agents coordinate with each other.

Single-agent safety does not carry over to multi-agent systems. Once agents delegate to each other, the attack surface is the protocol traffic between them — and the authority that travels, or fails to travel, with it.

---

## Research

**Privilege-Differential Drift: Measuring Mandate Inflation in Hierarchical LLM Agent Systems** — a pre-registered study of whether the size of the privilege gap between the agent writing shared state and the agent reading it predicts policy violation, with no adversary present anywhere in the chain.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23513214.svg)](https://doi.org/10.5281/zenodo.23513214)

Hypotheses, metric and falsification criteria fixed before data collection. A null result will be published. Code and documents in [privilege-differential-drift](https://github.com/evkir/privilege-differential-drift).

**ABFP** — Agent Behavioural FingerPrint. Agents are non-deterministic, so signature matching misses them; ABFP baselines an agent by the shape of what it does and treats deviation as the finding.

**HCAP** — Hierarchical Capability & Attestation Protocol. Makes capability and its provenance explicit and verifiable down a delegation chain, so over-privilege and confused-deputy conditions become detectable rather than structural.

ORCID [0009-0001-9871-2924](https://orcid.org/0009-0001-9871-2924)

---

## MASec Lab projects

| | |
| --- | --- |
| **[CyberAI](https://github.com/evkir/CyberAI)** · Apache-2.0 | Offensive testing platform for MCP servers and LLM agents. Coordinated specialist agents, async recon, CVE enrichment with EPSS scoring, out-of-band finding validation, sealed subprocess execution |
| **[mas-sentry-toolkit](https://github.com/evkir/mas-sentry-toolkit)** · AGPL-3.0 | Audits agentic systems over MCP, A2A, MQTT and AMQP. ABFP behavioural engine, MCP offensive audit module — tool poisoning, SSRF, path traversal — HTML and SARIF reporting. On [PyPI](https://pypi.org/project/mas-sentry-toolkit/) |
| **[privilege-differential-drift](https://github.com/evkir/privilege-differential-drift)** · CC BY 4.0 / Apache-2.0 | The pre-registered study above: frozen task set, capability allowlists, power analysis, policy gate and hash-chained event journal, all under test |

## Other tooling

| | |
| --- | --- |
| **[phantom-grid](https://github.com/evkir/phantom-grid)** · MIT | Out-of-band interaction capture over HTTP, HTTPS and DNS — a free Burp Collaborator alternative |
| **[phantom-intel](https://github.com/evkir/phantom-intel)** · MIT | CVE threat-intelligence platform on the NVD API 2.0 |
| **[reality-probe](https://github.com/evkir/reality-probe)** · MIT | VLESS/Reality SNI selection and TLS analysis |

---

## Writing

Twelve research pages at **[maseclab.com/research](https://maseclab.com/research/)**. Four ship reference SARIF 2.1.0 bundles with build gates that compare the page against the artifact in both directions and fail the build on disagreement — including when a probe that could not run is quietly dropped instead of being declared.

Recent:

- **Specified, Not Enforced** — the nine MCP authorization requirements of the 2026-07-28 revision, classified by whether an external prober can decide compliance. Six of nine can; one is decidable by nothing
- **Shared State Crosstalk** — tenant boundaries in agent runtimes: network isolation held, the shared package mirror carried the data
- **Delegated, Not Attributed** — eleven A2A protocol flaws, mapped to the OWASP Agentic Top 10, with the three unreachable by observation kept as `notApplicable`
- **Three Calls to Compromise** — runtime-gated MCP rug pulls generalised into six gate classes
- **Stateless, Not Traceless** — what the 2026-07-28 MCP revision cost detection by removing the session
- **Checked, Then Changed** — TOCTOU as one class across UI redress, skill-registry poisoning and catalogue drift

---

## Currently

- OSCP+ track; preparing for Burp Suite Certified Practitioner
- Active on HackTheBox and PortSwigger Web Security Academy
- Building out the v1.0 harness for the pre-registered study
- Next: Web3 and Immunefi — Foundry, Slither, Aderyn, Halmos, Echidna

---

[maseclab.com](https://maseclab.com) · [blog](https://maseclab.com/blog/) · [x.com/maseclab](https://x.com/maseclab) · [HackTheBox](https://app.hackthebox.com/users/3039943)
