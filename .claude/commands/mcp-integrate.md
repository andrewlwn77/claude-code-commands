# MCP Integrate - Integrate MCP Servers with Your Project

Automatically analyze your project and integrate MCP (Model Context Protocol) servers with project-specific documentation and workflows.

**Usage**: `/mcp:integrate`

## What This Command Does

When you run this command, I will:

1. **Analyze Available MCP Servers**
   - List all MCP servers and their capabilities
   - Identify which servers are relevant to your project
   - Group servers by functionality

2. **Analyze Your Project Structure**
   - Detect Docker configuration and container names
   - Identify database type and schema
   - Find frontend and backend frameworks
   - Discover infrastructure code (CDK, Terraform)
   - Note API integrations and external services

3. **Generate Custom Documentation**
   - Create MCP documentation specific to your project
   - Use actual container names from docker-compose.yml
   - Include database queries for your schema
   - Add testing commands for your tech stack
   - Provide debugging workflows

4. **Update CLAUDE.md**
   - Add or update "MCP Server Integration" section
   - Include project-specific examples
   - Add development workflows
   - Create quick reference guide

## What Gets Added

### 🐳 Docker Management
If Docker is detected:
- Container management with your actual container names
- Log viewing commands
- Resource monitoring
- Service restart procedures

### 🗄️ Database Access
If a database is found:
- Direct query access
- Schema inspection commands
- Data verification queries
- Performance analysis tools

### 🏗️ AWS Integration
If AWS services are used:
- CDK guidance and patterns
- Documentation search
- Infrastructure planning
- Deployment automation

### 🌐 Testing Automation
If a web frontend exists:
- Browser automation
- Screenshot capture
- Performance testing
- WebXR testing (for VR projects)

### 💻 IDE Features
Based on your languages:
- Error diagnostics
- Code execution
- Dependency verification
- Linting integration

## Example Integration

For a project with:
- Docker Compose (PostgreSQL + FastAPI + React)
- WebXR frontend
- AWS deployment plans

The command will add:
```bash
# Docker commands with your container names
mcp__mcp-server-docker__fetch_container_logs --container_id="myapp-backend-1"

# Database queries for your schema
mcp__postgres__query --sql="SELECT * FROM user_progress ORDER BY created_at DESC"

# Testing your actual endpoints
mcp__puppeteer__puppeteer_navigate --url="http://localhost:3000"

# AWS planning for your services
mcp__awslabs-cdk-mcp-server__SearchGenAICDKConstructs --query="lambda websocket"
```

## Development Workflows

The command also adds complete workflows:
- Database migration verification
- Container debugging procedures
- Performance monitoring setup
- Automated testing patterns

## Usage Flow

```bash
# First time setup:
/mcp:install    # Install MCP commands (if not done)
/mcp:integrate  # Analyze and integrate MCP

# After changes to project:
/mcp:integrate  # Re-run to update documentation
```

## Features

- **Smart Detection**: Automatically finds relevant MCP servers
- **Project-Aware**: Uses your actual service names and ports
- **Idempotent**: Safe to run multiple times
- **Preserves Content**: Won't overwrite customizations
- **Adaptive**: Works with any tech stack

## Example Output

```
🔍 Analyzing project structure...
✅ Found Docker Compose with 3 services
✅ Detected PostgreSQL database
✅ Found React frontend with WebXR
✅ Identified FastAPI backend

📝 Updating CLAUDE.md...
✅ Added Docker management section
✅ Added database access queries
✅ Added browser testing commands
✅ Added development workflows
✅ Added quick reference

🎉 MCP integration complete!
Your CLAUDE.md now includes project-specific MCP documentation.
```

## Requirements

- Project with identifiable structure
- Available MCP servers
- CLAUDE.md file (or it will be created)

## Notes

- Adapts to your specific project
- Updates documentation as project evolves
- Provides immediately useful commands
- Focuses on your actual use cases