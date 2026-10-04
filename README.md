# roblox-games
My Roblox game project.

## Roblox Studio MCP

This repo ships a project-scoped `.mcp.json` that registers the Roblox Studio MCP server
(`Roblox_Studio`) for Claude Code. It runs `%LOCALAPPDATA%\Roblox\mcp.bat`, so it only works
on Windows with Roblox Studio installed. Open the repo in Claude Code locally and approve the
server when prompted (or check with `/mcp`). Equivalent manual command:

```
claude mcp add --transport stdio Roblox_Studio -- "cmd.exe" "/c" "cd /d %LOCALAPPDATA%\Roblox && .\mcp.bat"
```
