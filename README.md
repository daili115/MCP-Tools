# MCP Tools

A curated collection of 100 Model Context Protocol (MCP) servers/tools with standardized install JSONs, complete metadata, and CI validation.

## Structure
- `/tools/index.json` — full metadata for all collected tools (name, version, description, author, compatibility, category)
- `/configs/tools-install.json` — standardized install configurations for each tool
- `.github/workflows/validate-configs.yml` — CI to validate JSON format and required fields
- `LICENSE` — MIT License
- `.gitignore` — standard ignores

## Categories
- Aggregators, File Systems, Browser Automation, Databases, Cloud Storage, Communication, Version Control, Monitoring, Search & Web, Productivity, Social Media, Finance, Dev Tools, Data Visualization, Identity, Security, IoT, Art & Media, E‑Commerce, Data Platforms, Robotics

## Usage
- Pick a tool from `/tools/index.json`
- Check its install commands in `/configs/tools-install.json`
- Add the server to your MCP client configuration (e.g., Claude Desktop `claude_desktop_config.json` under `"mcpServers"`)

## Notes
- Compatibility: MCP v1 unless otherwise stated. Most entries work with Claude Desktop, Zed, Cursor, Cody, etc.
- Versions are set to `latest` unless upstream provides explicit releases.
- Sources: Official MCP servers and curated community lists [modelcontextprotocol/servers], [awesome-mcp-servers] and related.

## Contribution
PRs welcome to update metadata, add servers, or improve install commands.