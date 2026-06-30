<h1 align="center">evkir</h1>

<p align="center"><strong>Offensive security for the swarm.</strong></p>

<p align="center">
Independent security researcher — multi-agent &amp; embodied AI.<br>
Founder of <a href="https://maseclab.com"><strong>MASec Lab</strong></a>: offensive tooling &amp; audit methodology for the layer between agents.
</p>

<p align="center">
  <a href="https://maseclab.com">maseclab.com</a> ·
  <a href="https://maseclab.com/blog">Blog</a> ·
  <a href="https://x.com/evkir">x.com/evkir</a> ·
  <a href="https://hackerone.com/evkir">HackerOne</a> ·
  <a href="https://medium.com/@ekiriyak">Medium</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/focus-multi--agent%20%2F%20embodied%20AI-0B0F14?style=flat-square&labelColor=0B0F14" alt="focus">
  <img src="https://img.shields.io/badge/MCP%20%7C%20A2A-protocol%20security-1f6feb?style=flat-square" alt="protocols">
  <img src="https://img.shields.io/badge/OWASP-Agentic%20Top%2010-2ea043?style=flat-square" alt="owasp">
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
| **[CyberAI](https://github.com/evkir/CyberAI)** — AI-native **offensive** platform | Specialist agents run recon, exploitation and reporting as one coordinated system. Native tool-calling, prompt-injection defence, cost/budget tracking, structured findings. MCP scanner that flags tool-poisoning offensively. |
| **[mas-sentry-toolkit](https://github.com/evkir/mas-sentry-toolkit)** — **defensive** audit (AGPL-3.0) | Audits agentic systems from the outside: A2A client, MCP audit, **ABFP** behavioural fingerprinting, unified threat engine. One Typer CLI, SARIF out. OWASP Agentic Top-10 (ASI01–ASI10) detectors. |

---

### Research — methodology, in the open

- **ABFP** — *Agent Behavioural FingerPrint.* Baseline an agent by **how it acts** across 6 dimensions; surface drift, hijack and impersonation as statistical deviations instead of predefined rules.
- **HCAP** — *Hierarchical Capability &amp; Attestation Protocol.* Prove what an agent **may** do and where its authority came from, down a delegation chain. N-of-M quorum, confused-deputy detection.
- **ASI mapping** — findings mapped to the **OWASP Agentic Top 10** for a shared, recognised taxonomy.

---

### Other tooling

- **[phantom-grid](https://github.com/evkir/phantom-grid)** — free Burp Collaborator alternative: OOB interaction capture (HTTP/HTTPS/DNS), SQLite store + exfil reassembly.
- **[phantom-intel](https://github.com/evkir/phantom-intel)** — CVE threat-intelligence platform on the NVD API 2.0.
- **[reality-probe](https://github.com/evkir/reality-probe)** — VLESS/Reality transport probing.

---

### Recent writeups

- **The Layer Nobody Baselines** — runtime behavioural detection for the MCP agent bus. [→](https://maseclab.com/blog/the-layer-nobody-baselines/)
- **Hunting MCP Tool Poisoning** — malicious instructions hidden in tool metadata, and how CyberAI catches them. [→](https://maseclab.com/blog/hunting-mcp-tool-poisoning/)
- **Agent-in-the-Middle** — what's wrong with unsigned A2A agent cards. [→](https://maseclab.com/blog/agent-in-the-middle/)
- **Why the coordination layer is the real attack surface** — single-agent safety doesn't compose. [→](https://maseclab.com/blog/coordination-layer/)

---

### Currently

- **OSCP+** track · active on PortSwigger / HackTheBox / TryHackMe (Top 15%)
- Entering bug bounty — HackerOne · Bugcrowd · Intigriti · **Immunefi / Web3** (Aug 2026)
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
