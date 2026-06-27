# AI & LinkedIn digest

Last updated: 2026-06-27

How this file works: ask "update my digest" any time and Claude refreshes it. AI updates come from web search; LinkedIn notifications need your logged-in browser, so they are captured at refresh time, not automatically in the background.

---

## Current AI updates (as of 2026-06-27)

### Models
- Microsoft MAI suite — seven in-house models (2 Jun 2026), flagship MAI-Thinking-1 reasoning model, positioned for premium reasoning at competitive token cost.
- Anthropic Claude Fable 5 (9 Jun 2026).
- Cohere North Mini Code; NVIDIA Nemotron 3 Ultra 550B.
- Google Gemini 3.1 Ultra updates; Gemini 3.5 Pro general availability slipped from June to July (testers flagged token efficiency and long-horizon issues).

### Agents and MCP (your lane)
- Salesforce Agentforce 3 built around MCP (23 Jun): DX, Heroku, and MuleSoft MCP servers, with a Slack server in development.
- MCP security update (18 Jun): OAuth refinements, resource indicators to stop access tokens being reused across servers, and a new set of security best practices. Directly relevant to kql-sop-mcp and your gatekeeper design.
- MCP spec release candidate dated 28 Jul 2026 is upcoming.
- Scale: roughly 97M monthly SDK downloads, governance under the Linux Foundation, native support in Claude, ChatGPT, Gemini, Copilot, Cursor.

### Microsoft Fabric and governed agents (your positioning)
- Fabric Data Agents now support service principal authentication (app identity instead of delegated user) for backend, automation, and MCP-based scenarios. Reinforces the governed-agent story you are building toward.
- Governed agent stack going native in Azure AI Foundry: agent runtime, policy engine, and identity fabric that enforce who an agent acts as, what data it touches, and which actions it can take.
- ACS (Agent Control Specification): an open standard for deterministic allow/deny governance at five lifecycle checkpoints — input, LLM, state, tool execution, output. This is your kql-sop gatekeeper pattern, formalised as a standard. Worth reading closely.

### Hardware and policy (context)
- OpenAI and Broadcom "Jalapeño" inference chip (25 Jun); Qualcomm Dragonfly C1000 CPU for agentic workloads (25 Jun).
- US executive order "Promoting Advanced Artificial Intelligence Innovation and Security" (2 Jun). Colorado AI Act takes effect 30 Jun, the first comprehensive US state AI law to go live.

---

## LinkedIn notifications (snapshot 2026-06-27)

- Your governed-KQL post is live and getting engagement: "An LLM attempted to drop a table on my cluster..." — Nick Curum reacted (1h).
- Databricks posted a #DataAISummit 2026 recap (7m).
- Mark Howith posted on subdomain takeover and DNS hygiene (2h) — security topic.
- Two "Suggested for you" viral posts (interview and recruiting stories), 1h, high engagement (369 and 859 reactions).
- Engagement on Nyomi O'Dowd's post ("Next stop London") — 5h.

---

## Sources
- AI model news: https://llm-stats.com/llm-updates · https://www.crescendo.ai/news/latest-ai-news-and-updates
- MCP: https://thenewstack.io/model-context-protocol-roadmap-2026/ · https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/
- Fabric and governed agents: https://community.fabric.microsoft.com/t5/Fabric-Updates-Blog/Fabric-June-2026-Feature-Summary/ba-p/5190690 · https://azure.microsoft.com/en-us/blog/microsoft-build-2026-building-agentic-apps-with-microsoft-fabric-and-microsoft-databases/

---

## Update log
- 2026-06-27: first version (AI updates + LinkedIn notifications snapshot).
