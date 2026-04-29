# Platform Compatibility Map

| Platform | Common Terms | Best Repo Term | Typical Use | Notes |
|---|---|---|---|---|
| ChatGPT / OpenAI | Apps, Connectors, Actions, Tools, Function calling, File search, Deep research, Sync | Integration Adapter | Search files, reference external data, take approved actions, call APIs, use tools | Describe capability needed instead of assuming a specific product name. |
| OpenAI API / Agents SDK | Tools, Function calling, Tool calls, Function tools, Custom tools, Actions | Integration Adapter or Tool Adapter | API calls, external data retrieval, structured actions, custom workflows | Map each tool to access level and approval rule. |
| Claude / Anthropic | Connectors, MCP connectors, MCP servers, Tools, Resources, Prompts | MCP Integration Adapter | Read external tools, call APIs, search data sources, perform actions through MCP | Treat MCP servers as powerful and permission-sensitive. |
| Gemini / Google | Apps, Connected apps, Extensions, Tools, Function calling | Google Integration Adapter | Google Workspace access, Gmail, Docs, Drive, Calendar, Tasks, Keep, API-based function calls | Confirm available app permissions before promising behavior. |
| Microsoft Copilot Studio | Connectors, Actions, Tools, Knowledge sources, Agent flows, MCP servers, Power Platform connectors | Microsoft Integration Adapter | SharePoint knowledge, Microsoft 365 data, Power Automate workflows, Power BI integration, business system actions | Separate knowledge retrieval from actions. |
| Cursor / Claude Code / IDE Agents | MCP servers, Tools, Commands, Context providers, Codebase indexing | IDE Integration Adapter | Codebase context, repo editing, local tools, developer workflows | Require approval for writes, commands, and destructive actions. |
| GitHub | GitHub App, API, Repository integration, Pull request tools, Issues | GitHub Adapter | Read repos, create issues, review PRs, write documentation, track changes | Writes require approval. |
| Netlify | Integration, API, Deploy hook, Build settings, Environment variables | Deployment Adapter | Create sites, deploy projects, check build logs, manage environment variables | Deployment and env changes always require approval. |
| Figma | Plugin, API, Dev Mode, MCP app, Design context | Design Adapter | Read design context, extract UI requirements, generate design-to-code notes, review UI consistency | Edits require approval. |
| Canva | App, Integration, Design tool, Brand kit, Template | Visual Content Adapter | Create visuals, generate reports, prepare client-facing assets, use brand kits | Client-facing publishing requires review. |
