# Rivet

Rivet is an early exploration of a local smart-tool layer for AI agents.

The basic idea is simple:

> As first-party AI interfaces become stronger, the useful missing layer may be the local systems that prepare, filter, execute, remember, and verify work on their behalf.

Rivet is not trying to become another chat app or agent UI. It is about connecting AI agent interfaces to local resources such as files, scripts, indexes, memory, local models, policy, and audit trails.

## Why This Exists

AI products from major labs are becoming agent cockpits: they already include tools, memory, code execution, browsing, automations, permissions, and review flows.

That makes another standalone interface less interesting than the layer underneath it.

Rivet explores what that layer could look like:

- local context preparation before frontier-model calls;
- smart tools that combine scripts, indexes, parsers, and local models;
- source-backed context packs instead of raw data dumps;
- local memory and workflow state that can work across agent interfaces;
- policy and audit around local data, secrets, and tool execution;
- support for edge devices, local machines, and future AI hardware.

## Read First

The best short introduction is the essay:

[The Future of AI Agents Is Not Another Interface](https://medium.com/@mr.kestrel/the-future-of-ai-agents-is-not-another-interface-6d0728c7fe7e)

## Status

This repository is early and exploratory.

The project is currently looking for:

- clearer framing;
- adapter evaluations;
- small prototypes;
- smart-tool workflow proposals;
- critique of the thesis.

## Contributing

Start with [CONTRIBUTING.md](CONTRIBUTING.md).

The most useful contributions right now are:

- evaluating existing tools before rebuilding them;
- proposing narrow smart-tool workflows;
- testing how Codex App, Claude Code, and other agent surfaces can call local tools;
- identifying projects that already solve parts of this idea;
- improving the public explanation.

## Non-Goals

Rivet is not currently aiming to be:

- a chatbot;
- a new primary agent UI;
- a hosted memory product;
- a standalone LLM Wiki clone;
- a model gateway;
- a broad autonomous agent framework.

The goal is smaller: understand and prototype the local layer that can complement the agent interfaces people already use.
