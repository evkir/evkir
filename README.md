<h1 align="center">evkir</h1>

<p align="center"><strong>Offensive security for the swarm.</strong></p>

<p align="center">
Independent security researcher — multi-agent &amp; embodied AI.<br>
Founder of <a href="https://maseclab.com"><strong>MASec Lab</strong></a>: offensive tooling &amp; audit methodology for the layer between agents.
</p>

<p align="center">
  <a href="https://maseclab.com">maseclab.com</a> ·
  <a href="https://maseclab.com/blog">Blog</a> ·
  <a href="https://x.com/maseclab">x.com/maseclab</a> ·
  <a href="https://bugcrowd.com/h/evkir">Bugcrowd</a> ·
  <a href="https://app.hackthebox.com/users/3039943">HTB</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/focus-multi--agent%20%2F%20embodied%20AI-0B0F14?style=flat-square&labelColor=0B0F14" alt="focus">
  <img src="https://img.shields.io/badge/MCP%20%7C%20A2A%20%7C%20MQTT%20%7C%20AMQP-protocol%20security-1f6feb?style=flat-square" alt="protocols">
  <img src="https://img.shields.io/badge/OWASP-Agentic%20Top%2010%20(2026)-2ea043?style=flat-square" alt="owasp">
  <img src="https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white" alt="python">
</p>

---

### whoami

Offensive security + agentic-AI safety. The industry is racing to test AI **models**; the riskier surface — how agents **coordinate, delegate and act together** — goes largely unexamined. I build the methodology and tooling for that layer, and publish it openly.

Single-agent safety doesn't compose. The boundary moved from the model to the **protocol traffic between agents** — that's where MASec Lab works.

---

### Building at MASec Lab

| | |
|---|---|
| **[CyberAI](https://github.com/evkir/CyberAI)** — offensive platform · Apache-2.0 · [PyPI](https://pypi.org/project/cyberai/) | **Metadata audit for MCP servers:** it reads what a server declares — `initialize`, instructions, tools, prompts, resources — scores it, and names the risk classes it does *not* check. It does not call a target's tools. **Runtime red-team for LLM agents:** injected canaries proven **out-of-band** via [phantom-grid](https://github.com/evkir/phantom-grid), not inferred from response diffs. Eight specialist agents on a typed, auditable pipeline; Web3 track on Slither with Immunefi severity mapping; prompt-injection guard in front of every provider call; fully air-gapped path on local models. |
| **[mas-sentry-toolkit](https://github.com/evkir/mas-sentry-toolkit)** — active scanner · AGPL-3.0 · [PyPI](https://pypi.org/project/mas-sentry-toolkit/) · [Docs](https://evkir.github.io/mas-sentry-toolkit/) | **The target is probed, not described.** Speaks **MCP / A2A / MQTT / AMQP on the wire** against live systems instead of reading config off disk: tool drift and rug-pull, elicitation consent, DNS rebinding, A2A card signatures, retained-payload injection, RabbitMQ tracing taps. Deterministic — no model gives the verdict, nothing about the target leaves the host. Protocol clients verified against the reference SDKs (`mcp`, `a2a-sdk`). **ABFP** behavioural fingerprinting, SARIF out, OWASP Agentic Top-10 (ASI01–ASI10). |

```bash
pip install cyberai
pip install mas-sentry-toolkit
```

---

### Recent writeups

- **Delegated, Not Attributed** — the first systematic security analysis of A2A: eleven protocol-level flaws. [→](https://maseclab.com/blog/delegated-not-attributed/)
- **Three Calls to Compromise** — a malicious MCP server distributed through 23 GitHub pull requests in 74 minutes. [→](https://maseclab.com/blog/three-calls-to-compromise/)
- **Approved, Not Shown** — the screen a human reads before approving an agent's action is rendered from attacker-controlled input. [→](https://maseclab.com/blog/approved-not-shown/)
- **ASI to the AI Act** — OWASP ASI01–ASI10 mapped onto EU AI Act Articles 12, 13 and 15. [→](https://maseclab.com/blog/asi-to-eu-ai-act/)
- **Stateless, Not Traceless** — every detection rule that grouped by session ID just lost its primary key. [→](https://maseclab.com/blog/stateless-not-traceless/)

[All posts →](https://maseclab.com/blog)

---

### Research — methodology, in the open

- **ABFP** — *Agent Behavioural FingerPrint.* Baseline an agent by **how it acts** across 6 dimensions; surface drift, hijack and impersonation as statistical deviations instead of predefined rules. Shipped in mas-sentry-toolkit; a live baseline is walked through [here](https://maseclab.com/blog/abfp-baseline/).
- **HCAP** — *Hierarchical Capability &amp; Attestation Protocol.* Prove what an agent **may** do and where its authority came from, down a delegation chain. N-of-M quorum, confused-deputy detection. [Specification](https://evkir.github.io/mas-sentry-toolkit/hcap-spec/).
- **ASI mapping** — findings mapped to the **OWASP Agentic Top 10 (2026)** for a shared, recognised taxonomy.

---

### Other tooling

- **[phantom-grid](https://github.com/evkir/phantom-grid)** — free Burp Collaborator alternative: OOB interaction capture (HTTP/HTTPS/DNS), SQLite store + DNS exfil reassembly. Backs CyberAI's out-of-band proofs.
- **[reality-probe](https://github.com/evkir/reality-probe)** — VLESS/Reality SNI selection under 2026 DPI: freeze-test, ASN/subnet topology scoring, subnet-neighbor discovery.
- **[phantom-intel](https://github.com/evkir/phantom-intel)** — CVE threat-intelligence desktop tool on the NVD API 2.0 (CVSS, exploit assessment, CWE KB, EN/RU).

---

### Currently

- **OSCP+** track · active on PortSwigger / HackTheBox / TryHackMe
- Bug bounty — Bugcrowd · Intigriti · Immunefi
- Web3 audit stack: Foundry · Slither · Aderyn · Halmos · Echidna

---

### Stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black">
  <img src="https://img.shields.io/badge/Kali-557C94?style=flat-square&logo=kalilinux&logoColor=white">
  <img src="https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white">
  <img src="https://img.shields.io/badge/nuclei-1f6feb?style=flat-square">
  <img src="https://img.shields.io/badge/MCP-JSON--RPC%202.0-0B0F14?style=flat-square">
  <img src="https://img.shields.io/badge/Foundry-2A2A2A?style=flat-square">
  <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white">
</p>

---

<p align="center"><sub>The agentic frontier is shipping faster than anyone is testing it.</sub></p>
