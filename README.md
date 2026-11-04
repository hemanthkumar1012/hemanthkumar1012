<p align="center">
  <img src="./assets/hero.svg" width="100%" alt="Hemanth Kumar — AI Engineer · Backend Engineer · Agent Systems"/>
</p>
<p align="center">
  <a href="https://www.linkedin.com/in/v-hemanth-kumar-yadav/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://hemanthkumar1012.github.io/Hemanth-kumar-portfolio/"><img src="https://img.shields.io/badge/Portfolio-0F172A?style=for-the-badge&logo=googlechrome&logoColor=38BDF8"/></a>
  <a href="mailto:hemanthkumaryadav13@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <img src="https://komarev.com/ghpvc/?username=hemanthkumar1012&style=for-the-badge&color=0e75b6&label=PROFILE+VIEWS"/>
</p>
<img src="./assets/divider.svg" width="100%"/>
<table>
<tr>
<td width="52%" valign="top">
⚡ What I do
I engineer AI agents that are safe to give real permissions to — and the backends they run on.
Most agent demos stop at "it called a tool." I work on what comes after: who authorized that call, how risky it was, whether the answer was grounded, and whether the next model version is actually better.
Engineering principles
	
🛡️ Guard the runtime	Policies, scoped credentials and approvals on every tool call
📊 Measure, then ship	Eval suites and release gates before any prompt or model change
🔍 Trace everything	Decisions are logged, auditable and reproducible
⚙️ Boring backends	Typed contracts, clean APIs, Postgres, containers
🎓 B.Tech CSE · SVU College of Engineering  ·  📍 Tirupati, India
</td>
<td width="48%" valign="top">
<img src="./assets/terminal.svg" width="100%" alt="terminal"/>
</td>
</tr>
</table>
<img src="./assets/divider.svg" width="100%"/>
🚀 Flagship Systems
<p align="center">
  <a href="https://github.com/hemanthkumar1012/agentguard"><img src="./assets/cards/agentguard.svg" width="49%"/></a>
  <a href="https://github.com/hemanthkumar1012/retrieval-lab"><img src="./assets/cards/retrieval-lab.svg" width="49%"/></a>
  <a href="https://github.com/hemanthkumar1012/llm-evaluation-lab"><img src="./assets/cards/llm-eval-lab.svg" width="49%"/></a>
  <a href="https://github.com/hemanthkumar1012/verity-enterprise-agent"><img src="./assets/cards/verity.svg" width="49%"/></a>
</p>
<details>
<summary><b>🔬 Deep dive: AgentGuard architecture</b></summary>
<br/>
Problem: autonomous agents call tools with real credentials, so one bad plan or a prompt injection can leak data or take destructive actions.
Approach: every tool call passes through a deterministic policy layer before it executes, and every decision lands in a tamper-evident log.
```mermaid
flowchart LR
    A[AI Agent] -->|tool call| G{AgentGuard}
    G --> P[Policy Engine<br/>OPA]
    G --> R[Risk Scoring]
    G --> D[Data Inspection]
    P & R & D --> Dec{Decision}
    Dec -->|allow| T[Tool · scoped credential]
    Dec -->|review| H[Human Approval]
    Dec -->|deny| X[Blocked]
    H --> T
    T --> L[(Tamper-evident<br/>Audit Log)]
    G -. anomalies .-> M[Anomaly Detection]
```
</details>
<details>
<summary><b>🔬 Deep dive: how I evaluate LLM changes</b></summary>
<br/>
```mermaid
flowchart LR
    W[Workflow] --> V[Versioned Dataset]
    V --> E[Eval Run]
    Q[Retrieval configs] --> E
    E --> C{Compare vs baseline}
    C -->|better| S[Ship ✅]
    C -->|regression| B[Block ❌ · review failures]
```
Retrieval Lab scores the retrieval layer; LLM Evaluation Lab gates the full workflow. Together, no change ships on vibes.
</details>
🧩 Also Built
Project	What it does	Stack	Links
📦 ParcelPilot	Shipment tracking, SLA-aware workflows, AI support agent	Python · FastAPI · React	Live · Code · Agent
🎯 ApplyRight	AI recruitment: resume analysis & application workflows	React · TS · Gemini	Live · Code
🏛️ SevaSetu	Agentic GovTech: citizen questions → evidence-backed action plans · Bharat Agentic 2026	TypeScript · Agents	Code
🏏 Cricket Tournament Manager	Scheduling, live scores, points tables, JWT auth	Java · Spring Boot · MySQL	Live · Code
🏫 Kinder Garden Schools OS	Multi-tenant school management system	JavaScript	Code
📐 LLD Practice Lab	Low-level design patterns, implemented	TypeScript	Code
<img src="./assets/divider.svg" width="100%"/>
🧰 Stack
<p align="center">
  <img src="https://skillicons.dev/icons?i=python,java,typescript,fastapi,spring,nodejs,react,nextjs,postgres,mongodb,redis,supabase,docker,linux,githubactions,vercel&theme=dark&perline=16"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/LLM_Agents-0EA5E9?style=flat-square"/>
  <img src="https://img.shields.io/badge/Tool_Calling-7C3AED?style=flat-square"/>
  <img src="https://img.shields.io/badge/RAG-16A34A?style=flat-square"/>
  <img src="https://img.shields.io/badge/LLM_Evaluation-F59E0B?style=flat-square"/>
  <img src="https://img.shields.io/badge/Policy_as_Code_(OPA)-475569?style=flat-square"/>
  <img src="https://img.shields.io/badge/Gemini-1A73E8?style=flat-square&logo=googlegemini&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
</p>
<img src="./assets/divider.svg" width="100%"/>
📡 Live Telemetry
<p align="center">
  <img src="./assets/stats.svg" width="96%" alt="GitHub stats"/>
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com?user=hemanthkumar1012&theme=tokyonight&hide_border=true&background=0B1220&ring=38BDF8&fire=A78BFA&currStreakLabel=7DD3FC" width="48%"/>
</p>
Recently shipped <sub>· refreshed daily by a GitHub Action</sub>
<!-- RECENT:START -->
<!-- RECENT:END -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/hemanthkumar1012/hemanthkumar1012/output/github-snake-dark.svg"/>
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/hemanthkumar1012/hemanthkumar1012/output/github-snake.svg"/>
    <img alt="contribution snake" src="https://raw.githubusercontent.com/hemanthkumar1012/hemanthkumar1012/output/github-snake-dark.svg" width="96%"/>
  </picture>
</p>
<img src="./assets/divider.svg" width="100%"/>
<p align="center">
  <b>Building agents that need to be trustworthy? Let's talk.</b><br/><br/>
  <a href="https://www.linkedin.com/in/v-hemanth-kumar-yadav/"><img src="https://img.shields.io/badge/Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:hemanthkumaryadav13@gmail.com"><img src="https://img.shields.io/badge/Say_Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>
<p align="center"><sub>This profile updates itself — stats card, recent activity and snake are regenerated daily by GitHub Actions (<code>scripts/update_profile.py</code>).</sub></p>
