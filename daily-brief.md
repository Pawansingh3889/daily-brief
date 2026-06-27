# Daily brief

Last updated: 2026-06-27

This is the actionable companion to [ai-linkedin-digest.md](ai-linkedin-digest.md). Two read passes feed it: a GitHub pass (notifications + feed, via the gh CLI) and a LinkedIn pass (notifications, via the logged-in browser). Ask "update my brief" to refresh.

---

## To do (reminders)

1. **kql-sop: flip the repo public.** Your LinkedIn post is already live and points readers to the repo; right now the link 404s for everyone. Highest priority because it's time-sensitive.
2. **sql-guard: review the pre-commit autoupdate PR.** GitHub flagged a `chore(deps): pre-commit autoupdate` PR with your review requested. Quick to merge or close.
3. **governed-agent-stack: push the local commit.** The pii-veil removal (commit a2d60ba) is committed locally but not pushed.
4. **Superset #39834: wait, don't code yet.** Monitor for a maintainer reply on which auth layer they will accept. No PR until they steer.
5. **Reply to Rowan / book the Kyle technical call.** The scheduling email is drafted; send it (free from 2 July).

## Suggested GitHub changes

- **Add kql-sop to governed-agent-stack.** It is now the KQL analog of sql-sop, so it belongs in the stack README and `stack.yaml` as a component. Concrete, small, and ties your new work into the umbrella.
- **kql-sop → PyPI.** Publish it like sql-sop so `pip install kql-sop` works without git.
- **kql-sop: SARIF reporter.** Reuse sql-guard's `reporters/sarif.py` so the linter plugs into CI and GitHub code scanning.
- **kql-sop-mcp: Streamable HTTP transport.** Needed for the Copilot Studio / Foundry demo (Path B). Harden its auth with the new MCP resource-indicator guidance when you do.
- **sql-guard: clear the dependency PR** to keep CI green and parity with kql-sop.

## New ideas

- **Align kql-sop with ACS (Agent Control Specification).** A new open standard defines deterministic allow/deny at five agent checkpoints (input, LLM, state, tool execution, output). Your gatekeeper is the same pattern. Map your rules to those checkpoints and reference ACS in the README; it positions you with the emerging standard rather than as a one-off.
- **Service-principal auth for the governed stack.** Fabric Data Agents just added app-identity auth. Designing your MCP auth around service principals (not delegated users) is the enterprise-ready pattern and a strong talking point for the Kyle call.
- **LocalAI as an on-prem backend option.** You follow mudler/LocalAI (very active, fresh release). Offering FloorMind a LocalAI backend alongside Ollama is on-brand with your on-prem ethos and broadens its reach.
- **chroma for the document/RAG gap.** You follow chroma-core. The "documents" side of governed agents (the ViewOps gap) is where a governed vector layer would extend your SQL-first stack.

## Inputs this refresh

- GitHub notifications: 1 (`sql-guard` pre-commit autoupdate, review requested).
- GitHub feed highlights: mudler/LocalAI (active, new release), drt-hub/drt activity, chroma-core/chroma, CHRISCARLON data-catalog repos.
- LinkedIn: your governed-KQL post is live (Nick Curum reacted); Databricks DataAISummit recap; security and recruiting posts. Full snapshot in the digest file.

---

## Update log
- 2026-06-27: first version (GitHub notifications + feed, LinkedIn snapshot, to-dos, suggestions, ideas).
