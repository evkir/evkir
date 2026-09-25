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
  <a href="https://hackerone.com/evkir">HackerOne</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/focus-multi--agent%20%2F%20embodied%20AI-0B0F14?style=flat-square&labelColor=0B0F14" alt="focus">
  <img src="https://img.shields.io/badge/MCP%20%7C%20A2A%20%7C%20MQTT-protocol%20security-1f6feb?style=flat-square" alt="protocols">
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
| **[CyberAI](https://github.com/evkir/CyberAI)** — **offensive** platform · Apache-2.0 | Runtime offensive testing for **MCP servers and LLM agents** — blind findings proven **out-of-band**, not inferred from response diffs. Coordinated specialist agents for recon, exploitation and reporting; native tool-calling, prompt-injection defence, cost/budget tracking, structured findings. Air-gapped-ready, 3000+ tests. |
| **[mas-sentry-toolkit](https://github.com/evkir/mas-sentry-toolkit)** — **defensive** audit · AGPL-3.0 · [PyPI](https://pypi.org/project/mas-sentry-toolkit/) | Active scanner that audits agentic systems **from the outside**: speaks **MCP / A2A / MQTT / AMQP on the wire** and probes live targets instead of reading config off disk. Deterministic — no model gives the verdict, nothing about the target leaves the host. **ABFP** behavioural fingerprinting, unified threat engine, SARIF out, OWASP Agentic Top-10 (ASI01–ASI10). |

`pip install mas-sentry-toolkit`

---

### Research — methodology, in the open

- **ABFP** — *Agent Behavioural FingerPrint.* Baseline an agent by **how it acts** across 6 dimensions; surface drift, hijack and impersonation as statistical deviations instead of predefined rules.
- **HCAP** — *Hierarchical Capability &amp; Attestation Protocol.* Prove what an agent **may** do and where its authority came from, down a delegation chain. N-of-M quorum, confused-deputy detection.
- **ASI mapping** — findings mapped to the **OWASP Agentic Top 10 (2026)** for a shared, recognised taxonomy.

---

### Other tooling

- **[phantom-grid](https://github.com/evkir/phantom-grid)** — free Burp Collaborator alternative: OOB interaction capture (HTTP/HTTPS/DNS), SQLite store + DNS exfil reassembly.
- **[phantom-intel](https://github.com/evkir/phantom-intel)** — CVE threat-intelligence platform on the NVD API 2.0 (CVSS, exploit assessment, CWE KB, EN/RU).
- **[reality-probe](https://github.com/evkir/reality-probe)** — VLESS/Reality SNI selection under 2026 DPI: freeze-test, ASN/subnet topology scoring, subnet-neighbor discovery.

---

### Recent writeups

- **The Layer Nobody Baselines** — runtime behavioural detection for the MCP agent bus. [→](https://maseclab.com/blog/the-layer-nobody-baselines/)
- **Hunting MCP Tool Poisoning** — malicious instructions hidden in tool metadata, and how CyberAI catches them. [→](https://maseclab.com/blog/hunting-mcp-tool-poisoning/)
- **Agent-in-the-Middle** — what's wrong with unsigned A2A agent cards. [→](https://maseclab.com/blog/agent-in-the-middle/)
- **Why the coordination layer is the real attack surface** — single-agent safety doesn't compose. [→](https://maseclab.com/blog/coordination-layer/)

---

### Currently

- **OSCP+** track · active on PortSwigger / HackTheBox / TryHackMe
- Bug bounty — HackerOne · Bugcrowd · Intigriti · Immunefi
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
