# Installation Guide

Follow these steps to get BrowserTools up and running in your development environment.

## 1. Chrome Extension Installation

### Option A: Chrome Web Store (Recommended)
The official chrome extension is pending approval on the Google extension marketplace. Once approved, you'll be able to install it directly from the Chrome Web Store.

### Option B: Manual Installation
1. Clone the repository:
```bash
git clone https://github.com/AgentDeskAI/browser-tools-mcp.git
```

2. Open Chrome's Extension Management:
   - Navigate to `chrome://extensions/`
   - Or use Menu → More Tools → Extensions

3. Enable Developer Mode:
   - Toggle the "Developer mode" switch in the top-right corner

4. Load the Extension:
   - Click "Load unpacked"
   - Navigate to the `chrome-extension` directory in the cloned repository
   - Click "Select"

You should now see BrowserTools MCP in your list of extensions.

## 2. MCP Server Setup

### Setting up in Cursor

1. Open Cursor Settings:
   - Click on the gear icon or use the keyboard shortcut
   - Navigate to "Features"
   - Scroll down to "MCP Servers"

2. Add New MCP Server:
   - Click "Add new MCP server"
   - Name: `browser-tools`
   - Type: `command`
   - Command: 
     ```bash
     npx @agentdeskai/browser-tools-mcp@1.2.0
     ```

   > Note for Windows users: Use `which npx` to find the correct path to NPX if needed.

3. Verify Connection:
   - Look for a green circle next to the tool name
   - All tools should be listed
   - If not connected, try clicking the refresh button or wait a few seconds

### Other MCP Clients

BrowserTools is compatible with various MCP clients. Check their respective documentation for setup instructions:
- [Windsurf](https://windsurf.io)
- [Zed](https://zed.dev)
- [RooCode](https://roocode.com)
- [Cline](https://cline.dev)
- [Claude Desktop](https://claude.ai/desktop)
- [LibreChat](https://librechat.ai)

## 3. Start the BrowserTools Server

Run the following command in your terminal:

```bash
npx @agentdeskai/browser-tools-server@1.2.0
```

> Note: The server runs on port 3025. Ensure no other processes are using this port.

## 4. Configure Chrome Developer Tools

1. Open Chrome Developer Tools:
   - Right-click on any webpage and select "Inspect"
   - Or use `Ctrl+Shift+I` (Windows/Linux) / `Cmd+Option+I` (Mac)

2. Navigate to the BrowserTools panel to configure:
   - Screenshot capture settings
   - Screenshot save location (default: Downloads/mcp-screenshots)
   - Log management
   - Size limits and truncation settings

## Verification

To verify your installation:

1. Ensure the Chrome extension is active (check the extension icon)
2. Confirm the BrowserTools server is running in your terminal
3. Open Chrome DevTools and check for the BrowserTools panel
4. Verify MCP server connection in your code editor

## Next Steps

- Check out our [Quickstart Guide](quickstart.md) to begin using BrowserTools
- Review [Troubleshooting](troubleshooting.md) if you encounter any issues
- Join our community for support and updates