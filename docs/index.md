# BrowserTools MCP

BrowserTools embeds AI code editors and agents directly into your web browser, providing a seamless integration for debugging and development.

## Overview

Built by [@tedx_ai](https://twitter.com/tedx_ai), BrowserTools gives AI code editors and agents the ability to monitor and interact with your web browser for highly effective debugging and a more seamless developer experience - all in a safe and secure manner.

### Key Features

With this MCP server tool, you can enable AI code editors and agents to have access to:

- Console logs and errors
- XHR network requests/responses
- Screenshot capabilities w/ optional auto-paste into Cursor
- Currently selected DOM elements
- Run SEO, Performance & Code Quality Scans via Lighthouse
- Run a NextJS-specific SEO audit
- Enter into "Debugger Mode" which uses many tools + prompts to fix bugs
- Enter into "Audit Mode" to perform a comprehensive web app audit

### Use Cases

Simply tell Cursor or any AI code editor with MCP integrations:
- "This isn't working… enter debugger mode!"
- "Can you edit the currently selected element to do x, y and z?"
- "I need to improve SEO and performance… enter audit mode"
- "Can you check console and network logs to see what went wrong?"
- "Something doesn't look right in the UI. Can you take a screenshot?"

## Requirements

- NodeJS installed on your machine
- Google Chrome or a Chromium-based Browser
- MCP Client Application (Cursor, Windsurf, RooCode, Cline, Continue, Zed, Claude Desktop)

> **Note**: Model Context Protocol (MCP) is specific to Anthropic models. When using an editor like Cursor, make sure to enable composer agent with Claude 3.5 Sonnet selected as the model.

## Quick Links

- [Installation Guide](installation.md)
- [Quickstart Guide](quickstart.md)
- [Troubleshooting](troubleshooting.md)
- [GitHub Repository](https://github.com/AgentDeskAI/browser-tools-mcp)