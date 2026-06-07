# Contributing

Rivet is early. The most valuable contributions right now are clear thinking, careful adapter evaluations, small working prototypes, and pressure tests of the thesis.

The project is open to collaboration, but intentionally focused. Rivet is a local smart-tool substrate for existing agent interfaces. It should help Codex App, Claude Code, and future first-party AI surfaces use local compute, memory, tools, context, policy, and audit without becoming another primary chat UI.

## Principles

- Build under the interface, not instead of it.
- Prefer local, inspectable state before cloud sync.
- Reuse strong existing tools before rebuilding them.
- Treat memory, skills, and model routing as modular, replaceable parts.
- Make context source-backed and compact before sending it to frontier models.
- Keep secrets out of prompts, memory, logs, and context packs.
- Audit meaningful state changes and risky actions.
- Start with a solo technical user and a Mac mini / Mac Studio style machine.

## Good First Contributions

The best early contributions fit one of these tracks:

1. **Adapter evaluations**
   - Install and test an existing project such as QMD, OpenKB, LLM Wiki tools, Contextful, Serena, codex-agent-mem, Dory, Ollama, MLX, llama.cpp, or MCP servers.
   - Report whether it can run locally, expose CLI/MCP/HTTP APIs, constrain paths, return source-backed outputs, and be wrapped without becoming the primary UI.

2. **Workflow RFCs**
   - Propose a specific smart-tool workflow.
   - Good examples: LLM Wiki maintenance, context pack generation, local document ingest, code impact analysis, memory linting, secret-safe browser actions, or local model extraction.

3. **Smart-tool specs**
   - Define a tool's inputs, outputs, allowed resources, audit behavior, failure modes, and verification examples.
   - Prefer narrow, testable tools over large autonomous workflows.

4. **Small prototypes**
   - Build tiny proofs that clarify a question.
   - Examples: deterministic Markdown context packer, QMD wrapper, SQLite audit log, Keychain reference injector, Ollama extraction script, or Codex/Claude MCP smoke test.

5. **Thesis pressure tests**
   - Find existing projects that make Rivet unnecessary.
   - Identify assumptions that are too broad, too vague, or already solved elsewhere.

## Non-Goals

Please do not steer the project toward:

- another chatbot;
- another coding-agent UI;
- a generic hosted memory product;
- a standalone LLM Wiki clone;
- a model gateway as the main product;
- an agent framework that competes with Codex App or Claude Code;
- broad unsupervised autonomy before policy and audit exist;
- cloud sync before the local schema and trust model are stable.

These may be useful adjacent projects, but they are not Rivet's first job.

## RFC Style

Use lightweight Markdown proposals for design work. Until the project has more structure, open an issue or pull request with one proposal per file or discussion.

- Start with status, motivation, proposed behavior, risks, and open questions.
- Keep proposals concrete enough that someone can build or reject them.

A good RFC should answer:

- What user workflow does this improve?
- Which interface uses it first: Codex App, Claude Code, CLI, or scheduler?
- What local resources does it need?
- What data is returned to the frontier model?
- What must be audited?
- What existing project could we wrap instead?
- What is explicitly out of scope?

## Adapter Evaluation Style

Use issues or pull requests for hands-on adapter evaluations until a permanent evaluation format exists.

Each evaluation should include:

- project name and link;
- install method;
- license and maturity signals;
- local-first behavior;
- available APIs: CLI, MCP, HTTP, library;
- Codex App / Codex CLI fit;
- Claude Code fit;
- source-backed output quality;
- path and permission controls;
- auditability;
- extension points;
- reasons to wrap it;
- reasons not to wrap it.

Prefer evidence from running the tool over marketing claims. When the tool cannot be tested, say so plainly.

## Development Posture

Until the runtime exists, docs and small experiments are the implementation surface.

When code appears:

- keep changes narrow;
- add verification notes;
- avoid large rewrites;
- prefer boring storage and simple schemas;
- make adapters replaceable;
- keep provider-specific behavior at the edges.

## Communication

Good discussion is welcome. The project needs critique as much as enthusiasm.

Helpful comments usually include:

- a concrete workflow;
- a competing project or prior art;
- a failure mode;
- a small test case;
- a proposed simpler design.

Avoid vague "agent OS" expansion unless it maps to a specific local resource, tool, context pack, policy, or audit behavior.
