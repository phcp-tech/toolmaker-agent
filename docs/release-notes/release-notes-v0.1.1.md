## Toolmaker Agent v0.1.1

First public release. Toolmaker Agent is an Agentic AI SDLC platform — humans and agents collaborate on the same structured data model: manage Products, Features, Requirements, and architecture through the web UI, an LLM chat agent, or MCP.

### New Features

- Product, Feature, and Requirement management with optimistic concurrency and soft delete
- Architecture design: create Components and arrange them in parent/child trees
- 4+1 system-design views with Mermaid diagrams (flowchart, sequence, C4, state, ER), exportable as PNG or SVG
- Technical documents organized in a tree
- Test case management
- Defect management
- LLM chat agent with SSE streaming, persistent history, and automatic summarization of long conversations
- LLM providers: OpenAI, Anthropic, Gemini, DeepSeek, Ollama, LM Studio, Hunyuan, Moonshot AI, and any OpenAI-compatible endpoint (Custom)
- MCP server (Streamable HTTP) with CRUD and query tools for all entities, so coding agents such as Claude Code can drive the same data
- Semantic search across Products, Features, Requirements, and UML diagrams, available from the UI, chat, and MCP
- Light/dark theme, and localized UI

### Free Edition

- For local use by a single person only.
- Up to 2 products per organization.

