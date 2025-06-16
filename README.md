# Claude Code Commands

A curated collection of slash commands for [Claude Code](https://claude.ai/code) that enhance your development workflow with AI-powered project management and tool integrations.

## 🚀 Overview

Claude Code Commands is a repository of custom slash commands that extend Claude Code's capabilities, providing intelligent project management, automated workflows, and seamless integration with development tools. These commands transform Claude into a smart project manager and development assistant.

## 📦 Available Commands

### Project Management Commands

#### `/project:install [project_name]`
Set up a complete AI-powered project management system in any Claude Code project.
- Adds intelligent project tracking to CLAUDE.md
- Creates command structure for project management
- Enables natural language project queries
- Tracks epics, stories, and progress automatically

#### `/project:sync`
Get an intelligent analysis of your current project status.
- Reads epics, git history, and codebase
- Identifies blockers and dependencies
- Provides prioritized recommendations
- Tracks progress across all project areas

#### `/project:plan`
Generate smart sprint and development plans.
- Analyzes dependencies and critical paths
- Suggests optimal task sequencing
- Estimates timelines based on complexity
- Balances workload across development areas

#### `/project:report [type]`
Create intelligent reports for different audiences.
- Types: `general`, `executive`, `technical`, `timeline`, `risks`
- Tailored content for each audience
- Visual progress indicators
- Actionable insights and recommendations

#### `/project:help [topic]`
Get comprehensive guidance on using AI project management.
- Learn available commands and workflows
- Understand natural language interactions
- Access best practices and tips
- Get project-specific recommendations

### MCP Integration Commands

#### `/mcp:install`
Install MCP (Model Context Protocol) integration commands.
- Adds MCP commands to your project
- Verifies MCP server availability
- Updates CLAUDE.md with MCP references
- Enables powerful development tools

#### `/mcp:integrate`
Automatically integrate MCP servers with your project.
- Analyzes project structure (Docker, databases, frameworks)
- Generates project-specific MCP documentation
- Adds custom workflows for your tech stack
- Provides ready-to-use MCP commands

## 🛠️ Installation

### Quick Start

1. Clone this repository or copy the `.claude` directory to your project:
```bash
# Clone the entire repository
git clone https://github.com/andrewlwn77/claude-code-commands.git

# Or copy just the commands to your project
cp -r claude-code-commands/.claude /your/project/
```

2. The commands are immediately available in Claude Code when you open your project.

### Installing Individual Command Sets

To install specific command sets in your existing project:

```bash
# For project management commands
/project:install

# For MCP integration commands
/mcp:install
```

## 💡 Usage Examples

### Natural Language Project Management

Instead of rigid commands, just talk to Claude naturally:

```
"What should I work on next?"
"How is the authentication epic progressing?"
"What's blocking our deployment?"
"Generate an executive summary of our progress"
```

### Project Status Check

```bash
/project:sync

# Output:
# 📊 Project Status
# 
# ## Current Sprint
# - 3 stories completed, 2 in progress
# - Velocity: 1.5 stories/day
# 
# ## Recommended Next Actions
# 1. Complete user authentication (blocks 3 other features)
# 2. Fix performance regression in search
# 3. Update API documentation
```

### Sprint Planning

```bash
/project:plan

# Output:
# 🎯 Sprint Planning
#
# ## Recommended Sprint Focus
# Theme: Core Authentication Flow
# Duration: 5 days
# Goal: Complete user login and session management
#
# ## Sprint Backlog (Prioritized)
# 1. Implement JWT tokens (Critical - blocks API access)
# 2. Add password reset flow (High - user requirement)
# 3. Set up OAuth providers (Medium - nice to have)
```

### MCP Integration

```bash
/mcp:integrate

# Output:
# 🔍 Analyzing project structure...
# ✅ Found Docker Compose with PostgreSQL and Node.js
# ✅ Detected React frontend
# 
# 📝 Updating CLAUDE.md...
# ✅ Added Docker management commands
# ✅ Added database query examples
# ✅ Added testing workflows
#
# Your project now has MCP commands like:
# - Check container logs: mcp__docker__logs
# - Query database: mcp__postgres__query
# - Run browser tests: mcp__puppeteer__navigate
```

## 🌟 Features

### AI-Powered Intelligence
- **Automatic Context Understanding**: Claude reads your entire project structure
- **Smart Recommendations**: Get AI-driven suggestions for what to work on next
- **Risk Detection**: Identify potential blockers before they become problems
- **Progress Tracking**: Automatic tracking without manual updates

### Natural Language Interface
- Talk to Claude like a smart project manager
- No need to remember complex commands
- Get context-aware responses
- Have intelligent conversations about your project

### MCP Server Integration
- **Docker Management**: Monitor and control containers
- **Database Access**: Run queries directly from Claude
- **Browser Testing**: Automate testing with Puppeteer
- **AWS Tools**: Access CDK documentation and patterns
- **IDE Features**: Get diagnostics and execute code

### Customizable and Extensible
- Adapt commands to your project's needs
- Add custom workflows and commands
- Integrate with your existing tools
- Scale with your project

## 🤝 Contributing

We welcome contributions! To add a new command:

1. Create a new `.md` file in `.claude/commands/`
2. Follow the existing command structure:
   - Clear description and usage
   - What the command does
   - Example outputs
   - Implementation details

3. Commands should be:
   - Self-documenting
   - Provide clear value
   - Include examples
   - Be idempotent when possible

### Command Structure

```markdown
# Command Name - Brief Description

Brief overview of what the command does.

**Usage**: `/namespace:command [parameters]`

## What I Do

Detailed explanation of the command's functionality...

## Example Usage

```bash
/namespace:command parameter

# Expected output...
```
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Links

- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Report Issues](https://github.com/andrewlwn77/claude-code-commands/issues)
- [Claude Code](https://claude.ai/code)

## 🙏 Acknowledgments

These commands are designed to enhance the Claude Code experience and make AI-assisted development more powerful and intuitive. Special thanks to the Anthropic team for creating Claude Code.

---

**Ready to supercharge your Claude Code workflow?** Start with `/project:install` or `/mcp:install` to add these powerful commands to your project!