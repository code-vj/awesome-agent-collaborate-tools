# Awesome Agent Collaboration Tools [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools and infrastructure for AI agent-to-agent communication, coordination, and collaboration.

Unlike general "awesome agents" lists that focus on *what agents can do*, this list focuses on **how agents work together** — the communication protocols, messaging systems, orchestration frameworks, shared memory layers, and observability tools that make multi-agent systems possible.

## Contents

- [Communication Protocols](#communication-protocols)
- [Messaging & Notification](#messaging--notification)
- [Multi-Agent Orchestration](#multi-agent-orchestration)
- [State & Memory](#state--memory)
- [Observability & Debugging](#observability--debugging)
- [Learning Resources](#learning-resources)

---

## Communication Protocols

Standards and protocols that define how agents discover and interact with each other.

- [MCP (Model Context Protocol)](https://modelcontextprotocol.io) - Open standard by Anthropic for connecting AI models to tools and data sources. Hosted by Linux Foundation. Widely adopted.
- [A2A (Agent-to-Agent Protocol)](https://google.github.io/A2A/) - Open protocol by Google (150+ supporting organizations) for agent interoperability across frameworks and vendors.
- [ANP (Agent Network Protocol)](https://agent-network-protocol.com) - Decentralized protocol for open agent networks, built on W3C DID standards.

## Messaging & Notification

Real-time messaging, pub/sub, and notification infrastructure designed for or applicable to agent-to-agent communication.

- [IM for Agents](https://im.fengdeagents.site) - Lightweight real-time messaging service purpose-built for AI agents. REST API for send/receive, no SDK required.
- [NATS](https://nats.io) - High-performance, cloud-native messaging system. Excellent for agent event streaming with subjects and queues.
- [Redis Pub/Sub + Streams](https://redis.io/docs/manual/pubsub/) - Battle-tested message patterns. Redis Streams provide persistent, consumer-group-based messaging suitable for agent pipelines.

## Multi-Agent Orchestration

Frameworks for defining agent roles, task delegation, and coordination logic.

- [CrewAI](https://github.com/crewAIInc/crewAI) - Role-based multi-agent framework. Agents have roles, goals, and backstories. Simple, production-ready.
- [LangGraph](https://github.com/langchain-ai/langgraph) - Graph-based agent orchestration by LangChain. Fine-grained control over agent state machines.
- [AutoGen](https://github.com/microsoft/autogen) - Microsoft's framework for conversational multi-agent workflows. Strong support for human-in-the-loop patterns.
- [Google ADK (Agent Development Kit)](https://google.github.io/adk-docs/) - Google's official SDK for building agents that work with Gemini and A2A protocol.
- [Anthropic Agent SDK](https://docs.anthropic.com/en/docs/agents) - Official Anthropic toolkit for building Claude-powered agents with tool use and handoffs.
- [Swarms](https://github.com/kyegomez/swarms) - Production-grade swarm orchestration. Supports hierarchical, sequential, and concurrent agent patterns.

## State & Memory

Tools for persisting agent context, shared knowledge, and cross-session memory.

- [Mem0](https://github.com/mem0ai/mem0) - Adaptive memory layer for AI agents. Stores and retrieves relevant memories across conversations.
- [Zep](https://github.com/getzep/zep) - Long-term memory store for LLM apps. Provides structured, searchable memory with temporal reasoning.
- [Letta (formerly MemGPT)](https://github.com/cpacker/MemGPT) - Research-backed framework for agents with OS-style virtual memory and infinite context management.

## Observability & Debugging

Tools for tracing, monitoring, and debugging multi-agent systems in production.

- [LangSmith](https://smith.langchain.com) - End-to-end observability platform for LLM/agent applications. Tracing, evaluation, and dataset management.
- [Arize Phoenix](https://github.com/Arize-ai/phoenix) - Open-source LLM observability. Trace agent runs, visualize spans, and evaluate outputs locally or in cloud.
- [OpenTelemetry](https://opentelemetry.io) - Vendor-neutral observability framework. Use with [OpenLLMetry](https://github.com/traceloop/openllmetry) for LLM-specific spans.

## Learning Resources

- [A2A Protocol Spec](https://google.github.io/A2A/specification/) - Full A2A specification and examples.
- [MCP Documentation](https://modelcontextprotocol.io/docs) - Official MCP docs with quickstarts and server examples.
- [Multi-Agent Patterns](https://github.com/masstensor/multi-agent-patterns) - Common patterns for building multi-agent systems with code examples.

---

## Contributing

Submissions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

Only add tools that are:
- Actively maintained (last commit within 12 months, or commercially supported)
- Genuinely useful for agent-to-agent collaboration (not just "agent-adjacent")
- Open source, or have a meaningful free tier

---

*Maintained by [@masstensor](https://github.com/masstensor)*
