# MCP Install - Install MCP Integration Commands

Install MCP (Model Context Protocol) integration commands into your project, enabling powerful development tools and workflows.

**Usage**: `/mcp:install`

## What This Command Does

When you run this command, I will:

1. **Create MCP Commands**
   - Add the `/mcp:integrate` command to your project
   - Ensure all MCP-related commands are available
   - Set up the command structure in `.claude/commands/`

2. **Update CLAUDE.md**
   - Add a reference to available MCP commands
   - Include basic MCP usage instructions
   - Preserve all existing content

3. **Verify Installation**
   - Check that commands are properly installed
   - Confirm MCP servers are accessible
   - Report any issues or missing dependencies

## Installation Process

```bash
/mcp:install

# What happens:
# 1. Creates .claude/commands/mcp-integrate.md
# 2. Updates CLAUDE.md with MCP command reference
# 3. Verifies MCP server availability
# 4. Reports installation status
```

## After Installation

Once installed, you can use:
- `/mcp:integrate` - Analyze your project and add MCP documentation
- Natural language requests like "check database schema" or "view container logs"

## Why Use MCP Commands?

MCP servers provide:
- **Docker Management**: Monitor and control containers
- **Database Access**: Run queries directly from Claude
- **AWS Integration**: Access CDK tools and documentation
- **Browser Testing**: Automate testing with Puppeteer
- **IDE Features**: Get diagnostics and run code

## Requirements

- Claude Code with MCP servers configured
- Project with CLAUDE.md file (or one will be created)
- Available MCP servers matching your project needs

## Example Output

```
✅ MCP commands successfully installed!

Available commands:
- /mcp:integrate - Analyze project and add MCP documentation

MCP servers detected:
- Docker management (mcp-server-docker)
- PostgreSQL access (postgres)
- AWS CDK tools (awslabs-cdk-mcp-server)
- Browser automation (puppeteer)
- IDE integration (ide)

Run /mcp:integrate to add project-specific MCP documentation.
```

## Notes

- This command is idempotent (safe to run multiple times)
- It won't overwrite existing customizations
- Works with any project structure
- Adapts to available MCP servers