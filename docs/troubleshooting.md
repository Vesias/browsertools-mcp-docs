# Troubleshooting Guide

If you're experiencing issues with BrowserTools, this guide will help you diagnose and resolve common problems.

## Common Issues

### 1. MCP Server Connection Issues

If you're having trouble connecting the MCP server:

1. Verify Installation:
   - Check if the MCP server is properly configured in your editor
   - Ensure the command is correct: `npx @agentdeskai/browser-tools-mcp@1.2.0`

2. Check Server Status:
   - Confirm the browser-tools-server is running
   - Verify it's running on port 3025
   - Check for any error messages in the terminal

3. Port Conflicts:
   - Ensure no other process is using port 3025
   - Try terminating any conflicting processes

### 2. Chrome Extension Issues

If the Chrome extension isn't working:

1. Extension Installation:
   - Verify the extension is properly installed
   - Check if it appears in Chrome's extension list
   - Look for any error indicators in the extension icon

2. Developer Tools:
   - Ensure Chrome DevTools is open in the target tab
   - Check if the BrowserTools panel is visible
   - Verify logs are being captured

### 3. Screenshot Capture Problems

If screenshots aren't working:

1. Check Permissions:
   - Verify the extension has necessary permissions
   - Ensure the screenshot directory exists
   - Check write permissions for the screenshot directory

2. Directory Configuration:
   - Verify the screenshot save path in the BrowserTools panel
   - Default path: Downloads/mcp-screenshots

## Debugging Steps

### 1. Check MCP Logs

Run this command to monitor Cursor MCP logs:

```bash
tail -n 20 -F ~/Library/Application\ Support/Cursor/**/*MCP.log
```

### 2. Gather Debug Information

If you need to report an issue, collect:

1. MCP Logs:
   - Screenshot of the MCP logs from the above command
   - Any error messages from the terminal

2. Browser Extension Logs:
   - Open Chrome's extension management page
   - Click on any error indicators
   - Take screenshots of error messages

3. Server Logs:
   - Screenshot of the browser-tools-server terminal output
   - Any error messages or warnings

## Common Error Messages

### "Port 3025 is already in use"

Solution:
1. Find the process using the port:
   ```bash
   lsof -i :3025
   ```
2. Terminate the process:
   ```bash
   kill -9 <PID>
   ```

### "Extension not responding"

Solutions:
1. Reload the extension
2. Restart Chrome
3. Reinstall the extension

## Getting Help

If you're still experiencing issues:

1. Check the [GitHub Issues](https://github.com/AgentDeskAI/browser-tools-mcp/issues) for similar problems
2. Contact [@tedx_ai](https://twitter.com/tedx_ai) on X
3. Create a new issue with:
   - Detailed description of the problem
   - Steps to reproduce
   - Collected debug information
   - Your environment details (OS, Chrome version, etc.)