# .claude/commands/help.md

```md
# Project Help - Your Intelligent Project Management Guide

Get guidance on using Claude as your AI project manager for the VR Language Learning project.

**Usage**: `/project:help [topic]`

Topics:
- `/project:help` - This overview
- `/project:help commands` - Available commands
- `/project:help natural` - Natural language interaction
- `/project:help workflow` - Recommended workflows

## 🤖 Welcome to Your AI Project Manager!

I'm Claude, your intelligent project manager for the VR Language Learning project. Instead of manual project tracking, I use AI to understand your project context and provide smart recommendations.

### 🎯 What Makes This Different

**Traditional Project Management**: Manual updates, rigid commands, lots of overhead
**Your AI Project Manager**: I read your code, understand your epics, track git history, and provide intelligent analysis

I automatically understand:
- ✅ Your WebXR-based VR learning environment
- ✅ Speech recognition via Whisper API
- ✅ AI tutor powered by GPT-4
- ✅ Text-to-speech with ElevenLabs
- ✅ Meta Quest compatibility requirements
- ✅ FastAPI backend with PostgreSQL
- ✅ Learning progression and vocabulary tracking

---

## 🚀 Quick Start Guide

### Step 1: Get Current Status
\`\`\`
/project:sync
\`\`\`
I'll analyze everything and tell you where you are, what's blocking progress, and what to work on next.

### Step 2: Plan Next Phase
\`\`\`
/project:plan
\`\`\`
I'll help you plan the optimal next sprint based on dependencies, capacity, and critical path.

### Step 3: Just Talk to Me!
Instead of commands, just ask me naturally:
- "What should I work on next?"
- "How is the speech recognition integration going?"
- "What's blocking the Quest deployment?"
- "Should I focus on the VR UI or backend APIs first?"

---

## 📚 Available Commands

### Core Commands
- **`/project:sync`** - Intelligent project analysis
  - Reads epics, git history, codebase
  - Provides status, blockers, recommendations
  - Tracks VR/WebXR specific progress

- **`/project:plan`** - Smart planning assistance
  - Plans next development sprint
  - Analyzes dependencies and critical path
  - Optimizes for Quest performance

- **`/project:report [type]`** - Intelligent reporting
  - Generates stakeholder reports
  - Types: `executive`, `technical`, `timeline`, `risks`
  - Includes VR-specific metrics

- **`/project:help [topic]`** - This help system
  - Get guidance on using your AI project manager
  - Learn workflows and best practices

---

## 💬 Natural Language Interaction

**This is the real power!** Just talk to me like you would a smart project manager:

### Status & Progress Questions
- "What's our current progress on the MVP?"
- "How is the WebXR implementation coming along?"
- "Is the speech recognition pipeline working?"
- "Are we Quest-ready yet?"
- "What's the status of the AI tutor integration?"

### Planning & Decision Questions
- "What should I work on next?"
- "Should I implement hand tracking or controllers first?"
- "When should we start Quest device testing?"
- "How do we optimize the audio processing latency?"
- "What's the critical path to a working demo?"

### Problem-Solving Questions
- "What's blocking our progress?"
- "How do we handle WebXR permissions on Quest?"
- "Why is speech recognition slow?"
- "How do we reduce VR scene complexity?"
- "What are the biggest performance risks?"

### Strategic Questions
- "What's the minimum viable learning experience?"
- "When can we start user testing?"
- "What features are must-have vs nice-to-have?"
- "Should we support Quest 1 or just Quest 2/3?"

---

## 📊 Understanding Your Project Structure

### System Architecture
\`\`\`
Meta Quest Browser → WebXR Frontend (React/Three.js)
                            ↓
                    FastAPI Backend
                            ↓
                    ┌───────┴───────┐
              Whisper API      GPT-4 Tutor
              (Speech)         (Conversation)
                    │               │
                    └───────┬───────┘
                            ↓
                    PostgreSQL Database
                    (Progress Tracking)
\`\`\`

### Core Components I Track
- **VR Experience**: WebXR scene, hand tracking, UI components
- **Speech Pipeline**: Recording → Whisper → Validation → Feedback
- **Learning System**: Sentences, vocabulary, progression logic
- **AI Integration**: GPT-4 tutor, ElevenLabs TTS
- **Infrastructure**: Docker, PostgreSQL, API endpoints

---

## 🔄 Recommended Workflows

### Daily Workflow
1. **Morning Check-in**: Ask me "What should I focus on today?"
2. **Development**: I understand VR constraints and can help troubleshoot
3. **End of Day**: Ask me "What progress did we make? What's next?"

### Sprint Workflow
1. **Sprint Start**: `/project:plan` for sprint planning
2. **Mid-Sprint**: `/project:sync` to assess progress
3. **Sprint End**: `/project:report` to summarize achievements

### Testing Workflow
1. **Pre-Quest Testing**: Ask "Is the build Quest-ready?"
2. **Performance Check**: "What might cause frame drops?"
3. **User Testing Prep**: "What should we test first?"

---

## 🧠 How I Understand Your Project

### What I Read Automatically
- **CLAUDE.md**: Architecture, commands, development notes
- **Git History**: Recent commits and development activity
- **Codebase**: Frontend components, backend APIs, database schema
- **package.json/requirements.txt**: Dependencies and versions
- **Docker/Make files**: Development environment setup

### Intelligence I Provide
- **VR Performance**: Quest optimization recommendations
- **Audio Pipeline**: Latency reduction strategies
- **Learning Design**: Progression and retention optimization
- **Integration Planning**: API and service coordination
- **Risk Assessment**: Technical challenges and solutions

### VR-Specific Context I Maintain
- WebXR requirements and constraints
- Quest hardware limitations (memory, CPU, GPU)
- Audio processing latency targets (<2 seconds)
- Frame rate requirements (60 FPS minimum)
- Hand tracking vs controller support
- Network requirements for API calls

---

## 🎯 Getting the Most Value

### Best Practices
1. **Share VR Testing Results**: Tell me about Quest performance issues
2. **Discuss User Feedback**: I can help prioritize fixes
3. **Ask About Trade-offs**: "Should we simplify graphics for Quest 1?"
4. **Use My Analysis**: I understand VR/AR specific challenges
5. **Check In Frequently**: VR development has unique blockers

### When to Use Commands vs. Natural Language
- **Commands**: For formal reports or comprehensive analysis
- **Natural Language**: For decisions, troubleshooting, daily work (most of the time!)

### Red Flags I Watch For
- 🚨 Complex geometry causing Quest frame drops
- 🚨 Audio latency exceeding 2 seconds
- 🚨 Memory usage approaching Quest limits
- 🚨 Missing WebXR permission handling
- 🚨 Unoptimized API calls in VR session
- 🚨 Lack of error handling for network issues

---

## 🚀 Your Next Steps

1. **Start with**: `/project:sync` to see current status
2. **Then ask**: "What's the highest priority for getting to MVP?"
3. **Use me daily**: I'm most valuable when involved in decisions
4. **Trust the process**: I understand VR development challenges

Remember: I'm not just tracking your project - I'm actively helping you navigate the unique challenges of VR language learning development!

---

**Ready to build your VR language learning experience? Let's start with `/project:sync` to see exactly where we are!**
```

# .claude/commands/install.md

```md
# Project Install - Set Up Intelligent Project Management

Install Claude's intelligent project management system in any Claude Code project.

**Usage**: `/project:install [project_name]`

## Instructions

I will set up a complete intelligent project management system for your project by:

1. **Update CLAUDE.md** with intelligent project management instructions
2. **Create command structure** in `.claude/commands/`
3. **Set up project tracking** with initial status files
4. **Configure epic and story templates** 
5. **Enable natural language project management**

## Implementation Steps

### 1. Read Current CLAUDE.md
First, I'll read your existing CLAUDE.md file to understand your project context and preserve existing instructions.

### 2. Add Project Management Section
I'll append comprehensive project management instructions to your CLAUDE.md:

\`\`\`markdown
---

# 🤖 CLAUDE'S PROJECT MANAGEMENT ROLE

## Acting as Your Intelligent Project Manager

I am your AI project manager for this project. I understand the project structure and can:

### 📊 Project Intelligence
- **Read & Understand**: I automatically read your epics, implementation plan, git history, and current codebase
- **Track Progress**: I understand where you are in each epic and what needs to happen next  
- **Suggest Actions**: I proactively recommend what to work on based on dependencies and priorities
- **Identify Blockers**: I spot potential issues before they become problems

### 🎯 Epic & Story Management
- **Epic Progress**: I track completion status across all epics automatically
- **Story Dependencies**: I understand which stories depend on others and suggest optimal sequencing
- **Acceptance Criteria**: I help validate when stories are truly complete
- **Technical Debt**: I identify when quick wins might create future problems

### 🔄 Sprint & Planning Intelligence  
- **Smart Sprint Planning**: I suggest stories for sprints based on capacity, dependencies, and risk
- **Velocity Tracking**: I learn your development patterns and improve estimates over time
- **Risk Assessment**: I flag stories that might be more complex than they appear
- **Resource Optimization**: I help balance development priorities and resource allocation

### 📈 Intelligent Reporting
- **Executive Summaries**: I generate business-focused progress reports for stakeholders
- **Technical Status**: I provide detailed status for development planning
- **Bottleneck Analysis**: I identify what's slowing down progress and suggest solutions
- **Milestone Tracking**: I track progress toward project goals and deadlines

### 🚀 Development Workflow Integration
- **Git Integration**: I understand commit history and can suggest what to work on based on recent changes
- **Code Context**: I read your codebase to understand what's implemented vs. what's planned
- **Deployment Planning**: I help sequence development for smooth integration and deployment
- **Testing Strategy**: I suggest testing approaches that fit your timeline and complexity

## How to Work with Me

### Natural Language Project Management
Instead of complex commands, just talk to me naturally:

- **"What should I work on next?"** → I analyze your epics and suggest optimal next steps
- **"How are we doing on [Epic/Feature]?"** → I give you detailed progress analysis with blockers
- **"Generate a status report"** → I create intelligent summaries for stakeholders  
- **"Plan the next sprint"** → I suggest story combinations based on capacity and dependencies
- **"What's blocking us?"** → I identify bottlenecks and suggest solutions

### Automatic Project Monitoring
I continuously monitor:
- **Implementation Status** (your progress tracking files)
- **Epic Progress** (from your epics structure)
- **Code Changes** (git history and current development)
- **Dependencies** (what needs to happen before what)
- **Timeline Health** (progress toward your project goals)

### Intelligent Suggestions
I proactively suggest:
- **High-Impact Next Steps**: What moves the needle most
- **Risk Mitigation**: Potential problems and solutions  
- **Resource Allocation**: When to focus on different areas of development
- **Integration Points**: When different components need to connect
- **Testing Priorities**: What needs validation before moving forward

## Quick Start Commands

Use these simple commands to trigger my intelligence:

### `/project:sync` 
I read everything (epics, implementation plan, git history, code) and provide:
- Current project status across all epics
- What's been completed recently
- What should be worked on next
- Any blockers or risks I've identified
- Timeline and milestone updates

### `/project:plan`
I help you plan the next phase by:
- Analyzing current progress and capacity
- Suggesting optimal story combinations for next sprint/phase
- Identifying dependencies that need attention
- Recommending focus areas and development priorities
- Providing time estimates based on complexity

### `/project:report`
I generate intelligent reports:
- **Executive Summary**: Business progress toward project goals
- **Technical Status**: Development progress and next milestones  
- **Risk Analysis**: Potential blockers and mitigation strategies
- **Timeline Health**: Progress against your implementation plan

### `/project:help`
Get comprehensive guidance on using your AI project manager:
- Available commands and workflows
- Natural language interaction examples
- Understanding project structure and dependencies
- Best practices and recommendations

### Natural Conversation
Just ask me anything about the project:
- "Should I focus on [X] or [Y] first?"
- "What's the critical path to [goal]?"
- "How much of [Epic] needs to be done before starting [other Epic]?"
- "What are the biggest risks to hitting our timeline?"

## Understanding Your Project Structure

I understand your project involves complex epics and dependencies. I track:

- **Epic Dependencies**: What blocks what, optimal sequencing
- **Critical Path Analysis**: The most important path to your goals
- **Resource Allocation**: When to focus where for maximum impact
- **Timeline Management**: Progress against your project milestones
- **Risk Assessment**: Technical challenges and business impact

I help balance parallel development across epics while ensuring critical paths stay on track.
\`\`\`

### 3. Create Command Structure
I'll create the `.claude/commands/` directory structure with these files:

- `sync.md` - Intelligent project analysis
- `plan.md` - Smart planning assistance  
- `report.md` - Intelligent reporting
- `help.md` - Comprehensive help system

### 4. Set Up Project Tracking
I'll create initial tracking files:

- `.claude/project_status.json` - Current project state tracking
- `epics.md` - Epic and story structure (if not exists)
- Update any existing implementation plan

### 5. Initialize Project Context
I'll analyze your current project and set up initial status based on:
- Existing files and structure
- Git history and current development state
- Any existing epic or planning documentation
- Project goals and timelines (if specified)

## Project Management Features Installed

After installation, you'll have:

### **Intelligent Analysis**
- Automatic epic and story progress tracking
- Dependency analysis and critical path identification
- Risk assessment and mitigation suggestions
- Timeline and milestone monitoring

### **Natural Language Interface**
- Ask questions naturally instead of using rigid commands
- Get context-aware recommendations
- Receive proactive suggestions and warnings
- Have intelligent conversations about project decisions

### **Smart Reporting**
- Executive summaries for stakeholders
- Technical status reports for development
- Timeline analysis and risk assessment
- Customizable reports for different audiences

### **Development Integration**
- Git history analysis for progress tracking
- Code-aware recommendations
- Integration planning and sequencing
- Testing and deployment guidance

## Example Usage After Installation

\`\`\`bash
# Get current project status
/project:sync

# Plan next development phase
/project:plan

# Generate stakeholder report
/project:report executive

# Get help and guidance
/project:help

# Or just talk naturally:
# "What should I work on next?"
# "How is progress on the user authentication epic?"
# "What's blocking us from deployment?"
\`\`\`

## Customization

After installation, you can customize:

1. **Epic Structure**: Update `epics.md` with your specific epics and stories
2. **Project Goals**: Modify project context in CLAUDE.md
3. **Timeline**: Adjust milestone and deadline information
4. **Commands**: Edit command files in `.claude/commands/` for project-specific needs
5. **Tracking**: Customize `.claude/project_status.json` for your metrics

## Benefits

- **Reduced Overhead**: No manual project tracking required
- **Intelligent Guidance**: AI-powered recommendations and risk assessment
- **Context Awareness**: Understanding of your specific project constraints
- **Natural Interaction**: Talk to Claude like a smart project manager
- **Proactive Management**: Early identification of issues and opportunities

The system grows with your project and becomes more intelligent over time, learning your patterns and preferences to provide better guidance.

---

**Installation Complete!** Your intelligent project management system is ready. Start with `/project:sync` to see your current status, or just ask me "What should I work on next?"
```

# .claude/commands/mcp-install.md

```md
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

\`\`\`bash
/mcp:install

# What happens:
# 1. Creates .claude/commands/mcp-integrate.md
# 2. Updates CLAUDE.md with MCP command reference
# 3. Verifies MCP server availability
# 4. Reports installation status
\`\`\`

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

\`\`\`
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
\`\`\`

## Notes

- This command is idempotent (safe to run multiple times)
- It won't overwrite existing customizations
- Works with any project structure
- Adapts to available MCP servers
```

# .claude/commands/mcp-integrate.md

```md
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
\`\`\`bash
# Docker commands with your container names
mcp__mcp-server-docker__fetch_container_logs --container_id="myapp-backend-1"

# Database queries for your schema
mcp__postgres__query --sql="SELECT * FROM user_progress ORDER BY created_at DESC"

# Testing your actual endpoints
mcp__puppeteer__puppeteer_navigate --url="http://localhost:3000"

# AWS planning for your services
mcp__awslabs-cdk-mcp-server__SearchGenAICDKConstructs --query="lambda websocket"
\`\`\`

## Development Workflows

The command also adds complete workflows:
- Database migration verification
- Container debugging procedures
- Performance monitoring setup
- Automated testing patterns

## Usage Flow

\`\`\`bash
# First time setup:
/mcp:install    # Install MCP commands (if not done)
/mcp:integrate  # Analyze and integrate MCP

# After changes to project:
/mcp:integrate  # Re-run to update documentation
\`\`\`

## Features

- **Smart Detection**: Automatically finds relevant MCP servers
- **Project-Aware**: Uses your actual service names and ports
- **Idempotent**: Safe to run multiple times
- **Preserves Content**: Won't overwrite customizations
- **Adaptive**: Works with any tech stack

## Example Output

\`\`\`
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
\`\`\`

## Requirements

- Project with identifiable structure
- Available MCP servers
- CLAUDE.md file (or it will be created)

## Notes

- Adapts to your specific project
- Updates documentation as project evolves
- Provides immediately useful commands
- Focuses on your actual use cases
```

# .claude/commands/plan.md

```md
# Project Plan - Intelligent Sprint & Development Planning

Help plan your next development phase with AI-powered recommendations.

**Usage**: `/project:plan`

## What I Do

When you run this command, I will:

1. **Analyze Current State**
   - Review completed work and velocity
   - Check remaining stories and epics
   - Assess team capacity and constraints
   - Identify technical dependencies

2. **Calculate Optimal Sprint**
   - Group stories by dependencies
   - Balance workload across areas
   - Prioritize high-impact items
   - Consider risk mitigation

3. **Provide Development Sequence**
   - Order tasks for smooth integration
   - Minimize context switching
   - Enable parallel development
   - Reduce blocking dependencies

4. **Estimate Timeline**
   - Project completion dates
   - Account for complexity
   - Include buffer for unknowns
   - Track against milestones

## Output Format

\`\`\`markdown
# 🎯 VR Language Learning - Sprint Planning

## Recommended Sprint Focus
**Theme**: [Primary focus area]
**Duration**: [Estimated days/weeks]
**Goal**: [What will be achieved]

## Sprint Backlog (Prioritized)
### 🔴 Critical Path (Must Complete)
1. **[Story Name]** - [Why critical]
   - Estimated: [X] hours
   - Dependencies: [What it blocks]
   - Acceptance: [Clear criteria]

2. **[Story Name]** - [Why critical]
   [Details...]

### 🟡 High Priority (Should Complete)
[Stories that add significant value...]

### 🟢 Nice to Have (If Time Permits)
[Lower priority items...]

## Development Sequence
\`\`\`mermaid
graph LR
    A[Setup WebXR] --> B[Audio Recording]
    B --> C[Whisper Integration]
    C --> D[Progress Tracking]
    D --> E[Quest Testing]
\`\`\`

## Parallel Work Streams
- **Stream 1**: Frontend VR components
- **Stream 2**: Backend API endpoints
- **Stream 3**: Database and state management

## Risk Mitigation
- **Risk**: WebXR compatibility issues
  **Mitigation**: Early Quest device testing
- **Risk**: Audio latency on speech
  **Mitigation**: Implement client-side buffering

## Success Metrics
- [ ] All critical path items complete
- [ ] Core learning loop functional
- [ ] Successful Quest deployment
- [ ] Sub-2s speech response time
\`\`\`

## Planning Intelligence

I consider:
- **Technical Dependencies**: What must be built first
- **Integration Points**: Where components connect
- **Testing Requirements**: What needs validation
- **Performance Constraints**: Quest hardware limits
- **Learning Curve**: New technology adoption time

## VR Language Learning Specific Planning

I optimize for:
- **Quest Performance**: Keep scenes lightweight
- **Audio Pipeline**: Minimize speech recognition latency
- **User Experience**: Smooth VR interactions
- **Learning Effectiveness**: Progression and retention
- **Development Speed**: MVP feature prioritization

## Example Usage

\`\`\`bash
/project:plan

# Output:
# 🎯 VR Language Learning - Sprint Planning
#
# ## Recommended Sprint Focus
# **Theme**: Core Speech Recognition Loop
# **Duration**: 5 days
# **Goal**: Complete end-to-end speech practice in VR
#
# ## Sprint Backlog (Prioritized)
# ### 🔴 Critical Path (Must Complete)
# 1. **WebXR Audio Permissions** - Blocks all speech features
#    - Estimated: 4 hours
#    - Dependencies: All speech recording
#    - Acceptance: Audio captures on Quest
#
# [... continued planning ...]
\`\`\`

This command helps you make intelligent decisions about what to build next and in what order.
```

# .claude/commands/record-help.md

```md
# Record Help - API Recording System Guide

Get comprehensive help for the Claude Recording System.

**Usage**: `/record:help [topic]`

**Topics**:
- `/record:help` - Overview and quick start (this page)
- `/record:help modes` - Detailed explanation of recording modes
- `/record:help commands` - Full command reference
- `/record:help apis` - Configuring specific APIs
- `/record:help troubleshooting` - Common issues and solutions
- `/record:help best-practices` - Tips for effective recording

## Instructions

When you use this command, I will:

1. **For general help** (no topic):
   - Show current recording status
   - Provide quick start guide
   - List common commands
   - Suggest next steps based on context

2. **For specific topics**:
   - Display detailed documentation
   - Include relevant examples
   - Show current configuration
   - Provide interactive guidance

## Help Topics

### General Overview (`/record:help`)
\`\`\`
🎬 Claude Recording System Help
═══════════════════════════════════════════════════

The recording system helps you capture and replay API calls,
reducing costs and speeding up development.

QUICK START:
1. Install system:     /record:install
2. Start recording:    /record start my-session
3. Make API calls normally
4. Stop recording:     /record stop
5. Use recordings:     /record replay my-session

CURRENT STATUS:
Mode: replay (using recorded responses)
Active Cassette: feature-dev-2024-01-15
Cost Saved: $12.50 this session

COMMON COMMANDS:
• /record status         Show current state
• /record list          See available recordings
• /record bypass        Use real APIs temporarily
• /record:help modes    Learn about different modes

For detailed help on any topic, use:
/record:help [topic]
\`\`\`

### Recording Modes (`/record:help modes`)
\`\`\`
🎭 Recording Modes Explained
═══════════════════════════════════════════════════

The recording system supports four modes:

📹 RECORD MODE
When to use: Capturing new API interactions
How it works: Intercepts API calls and saves responses
Example: /record start feature-test
Benefits: Build reusable test data, document API behavior

📼 REPLAY MODE (Default)
When to use: Development and testing
How it works: Returns saved responses instead of calling APIs
Example: /record replay feature-test
Benefits: Zero API costs, instant responses, consistent data

🚫 BYPASS MODE
When to use: Production testing, fresh data needed
How it works: Disables recording system completely
Example: /record bypass --duration 1h
Benefits: Real API responses, production behavior

🔄 HYBRID MODE
When to use: Incremental development
How it works: Uses recordings if available, else real API
Example: /record config --mode hybrid
Benefits: Automatic fallback, records new endpoints

SWITCHING MODES:
• Temporary: /record [mode] --duration 30m
• Permanent: /record config --mode [mode]
• Per-API: /record bypass --apis openai
• Environment: export CLAUDE_RECORDING_MODE=bypass
\`\`\`

### Command Reference (`/record:help commands`)
\`\`\`
📚 Complete Command Reference
═══════════════════════════════════════════════════

RECORDING COMMANDS:
/record start [name]     Begin recording session
  --append              Add to existing cassette
  --apis api1,api2      Only record specific APIs
  --duration 1h         Auto-stop after time

/record stop            End recording session
  --save-as [name]      Save with different name
  --discard             Don't save recording

PLAYBACK COMMANDS:
/record replay [name]    Use specific recording
  --latest              Use most recent
  --list                Show options first

/record bypass          Use real APIs
  --duration 1h         Temporary bypass
  --apis api1,api2      Bypass specific APIs only

MANAGEMENT COMMANDS:
/record list            Show all recordings
  --details             Include size/api info
  --api [name]          Filter by API
  --recent [n]          Show last N recordings

/record delete [name]   Remove recording
  --older-than 30d      Delete old recordings
  --pattern "test-*"    Delete by pattern

/record info [name]     Detailed cassette info
  --costs               Show cost breakdown
  --requests            List all requests

CONFIGURATION:
/record config          Update settings
  --mode [mode]         Set default mode
  --filter-header [h]   Add header filter
  --api-cost [api] [n]  Set API cost

UTILITIES:
/record status          Current state
/record validate        Check cassette integrity
/record export [name]   Export for sharing
/record import [file]   Import shared cassette
\`\`\`

### API Configuration (`/record:help apis`)
\`\`\`
🔧 Configuring API Recording
═══════════════════════════════════════════════════

Configure which APIs to record and how:

DEFAULT CONFIGURATION:
• External APIs (https://*): Recorded
• Localhost (http://localhost:*): Not recorded
• Sensitive headers: Automatically filtered

ADDING CUSTOM APIS:
/record config --api-pattern "https://api.myservice.com/*"
/record config --api-cost myservice 0.001

FILTERING SENSITIVE DATA:
/record config --filter-header "x-custom-auth"
/record config --filter-param "user_password"
/record config --filter-body-field "ssn"

API-SPECIFIC SETTINGS:
{
  "apis": {
    "openai": {
      "pattern": "https://api.openai.com/*",
      "record": true,
      "cost_per_request": 0.02,
      "filter_headers": ["authorization"],
      "timeout": 30000
    },
    "internal": {
      "pattern": "https://api.internal.com/*",
      "record": false,
      "reason": "Contains PII data"
    }
  }
}

COMMON PATTERNS:
• Payment APIs: Usually not recorded (PCI compliance)
• AI/ML APIs: Record with cost tracking
• Internal APIs: Configurable based on data sensitivity
• Third-party APIs: Record for reliability
\`\`\`

### Troubleshooting (`/record:help troubleshooting`)
\`\`\`
🔍 Troubleshooting Guide
═══════════════════════════════════════════════════

COMMON ISSUES:

1. "Recording not working"
   ✓ Check mode: /record status
   ✓ Verify installation: /record:install --check
   ✓ Enable debug: export CLAUDE_RECORDING_DEBUG=true
   ✓ Check permissions on cassette directory

2. "Replay not matching requests"
   ✓ Check request matching config
   ✓ Verify headers aren't changing
   ✓ Look for timestamps in requests
   ✓ Try relaxed matching: /record config --match-relaxed

3. "Sensitive data in recordings"
   ✓ Add filters: /record config --filter-header "auth"
   ✓ Review before sharing: /record info [name]
   ✓ Clean existing: /record clean [name]

4. "Performance issues"
   ✓ Check cassette size: /record info [name]
   ✓ Split large recordings: /record split [name]
   ✓ Use selective recording: --apis specific

5. "Integration conflicts"
   ✓ Check for other interceptors
   ✓ Load order matters in tests
   ✓ Use exclusive mode: --exclusive

DEBUG COMMANDS:
/record debug --last-error
/record debug --show-config
/record debug --test-intercept

GET MORE HELP:
• Check logs: .claude/recording/debug.log
• Validate setup: /record validate
• Report issues: Include /record debug output
\`\`\`

### Best Practices (`/record:help best-practices`)
\`\`\`
✨ Best Practices for API Recording
═══════════════════════════════════════════════════

DEVELOPMENT WORKFLOW:
1. Start with replay mode (default)
2. Use bypass when you need fresh data
3. Record new interactions incrementally
4. Clean up old cassettes regularly

NAMING CONVENTIONS:
✓ feature-name-YYYY-MM-DD
✓ bugfix-ISSUE-123
✓ test-user-journey
✗ test1, temp, asdf

SECURITY:
• Never record production credentials
• Review cassettes before committing
• Use filters for sensitive data
• Rotate test API keys regularly

TEAM COLLABORATION:
• Share cassettes for consistent testing
• Document special recording needs
• Use descriptive names
• Keep cassettes in version control

COST OPTIMIZATION:
• Set accurate API costs in config
• Monitor savings with /record status
• Use hybrid mode for partial coverage
• Schedule bypass windows carefully

TESTING:
• Record happy path and error cases
• Include rate limit responses
• Capture timeout scenarios
• Test with degraded responses

MAINTENANCE:
/record delete --older-than 30d
/record clean --remove-duplicates
/record optimize [name]
/record validate --all

ADVANCED TIPS:
• Chain recordings: /record chain test1 test2
• Conditional recording: Based on env vars
• Parallel recording: Multiple cassettes
• Mock specific endpoints only
\`\`\`

## Interactive Features

The help system is context-aware and will:

1. **Show relevant information** based on current state
2. **Highlight potential issues** in your configuration  
3. **Suggest next actions** based on your workflow
4. **Provide copy-paste examples** for your specific setup
5. **Track which help topics** you've viewed

## Getting Started

New to the recording system? Follow this path:
1. `/record:help` - Get overview
2. `/record:install` - Set up system
3. `/record:help modes` - Understand options
4. `/record start` - Try recording
5. `/record:help best-practices` - Level up

Need specific help? Jump directly to:
- `/record:help commands` - Full reference
- `/record:help troubleshooting` - Fix issues
- `/record:help apis` - Configure APIs
```

# .claude/commands/record-install.md

```md
# Record Install - Setup API Recording Infrastructure

Install a generic, portable API recording system for cost-effective development.

**Usage**: `/record:install [options]`

**Options**:
- `--language [auto|python|node|java|go]` - Programming language (default: auto-detect)
- `--mode [replay|record|bypass|hybrid]` - Default recording mode (default: replay)
- `--apis [all|external|none]` - Which APIs to record (default: external)

## Instructions

I will set up a complete API recording infrastructure for your project by:

1. **Detecting Project Type**
   - Analyze project files to determine language and framework
   - Identify package management system (pip, npm, maven, etc.)
   - Check for existing test infrastructure

2. **Installing Recording Libraries**
   - **Python**: Add `vcrpy` to requirements-dev.txt or pyproject.toml
   - **Node.js**: Add `nock` or `polly.js` to package.json devDependencies
   - **Java**: Add WireMock to pom.xml or build.gradle
   - **Go**: Add go-vcr to go.mod
   - **Other**: Set up mitmproxy-based recording

3. **Creating Recording Infrastructure**
   \`\`\`
   .claude/recording/
   ├── config.json          # Recording configuration
   ├── status.json          # Current recording state
   ├── cassettes/           # Recorded API interactions
   │   └── .gitkeep
   ├── utilities/           # Helper scripts
   │   └── record_helper.{py|js|java|go}
   └── help/               # Help documentation
       ├── modes.md
       ├── commands.md
       ├── apis.md
       ├── troubleshooting.md
       └── best-practices.md
   \`\`\`

4. **Generating Configuration**
   \`\`\`json
   {
     "recording": {
       "version": "1.0",
       "language": "python",
       "library": "vcr",
       "default_mode": "replay",
       "cassette_dir": ".claude/recording/cassettes",
       "filters": {
         "headers": ["authorization", "x-api-key", "cookie"],
         "body_params": ["password", "secret", "token"],
         "query_params": ["apikey", "key"]
       },
       "apis": {
         "external": {
           "pattern": "https://*",
           "record": true,
           "replay": true
         },
         "localhost": {
           "pattern": "http://localhost:*",
           "record": false,
           "replay": false
         }
       },
       "cost_tracking": {
         "enabled": true,
         "apis": {
           "openai": {"per_request": 0.02},
           "anthropic": {"per_request": 0.01},
           "default": {"per_request": 0.001}
         }
       }
     }
   }
   \`\`\`

5. **Creating Helper Utilities**
   - Language-specific recording wrapper
   - Cassette management functions
   - Sensitive data filtering
   - Cost tracking utilities

6. **Setting Up Test Integration**
   - Add recording fixtures to test framework
   - Create example test with recording
   - Configure CI/CD to use replay mode

7. **Updating Project Documentation**
   - Add recording section to CLAUDE.md
   - Create README in .claude/recording/
   - Add examples for common use cases

## Language-Specific Setup

### Python Setup
\`\`\`python
# .claude/recording/utilities/record_helper.py
import vcr
from pathlib import Path
import json
import os

class RecordingHelper:
    def __init__(self):
        self.config = self._load_config()
        self.vcr = self._setup_vcr()
    
    def get_cassette_path(self, name):
        return Path(self.config['cassette_dir']) / f"{name}.yaml"
    
    def _setup_vcr(self):
        return vcr.VCR(
            cassette_library_dir=self.config['cassette_dir'],
            record_mode=self._get_record_mode(),
            filter_headers=self.config['filters']['headers'],
            decode_compressed_response=True
        )
    
    def _get_record_mode(self):
        mode = os.environ.get('CLAUDE_RECORDING_MODE', self.config['default_mode'])
        return {
            'record': 'new_episodes',
            'replay': 'none',
            'bypass': 'all',
            'hybrid': 'once'
        }.get(mode, 'once')
\`\`\`

### Node.js Setup
\`\`\`javascript
// .claude/recording/utilities/record_helper.js
const nock = require('nock');
const fs = require('fs');
const path = require('path');

class RecordingHelper {
  constructor() {
    this.config = this.loadConfig();
    this.setupNock();
  }
  
  setupNock() {
    if (this.getMode() === 'replay') {
      nock.loadRecording(this.config.cassette_dir);
    } else if (this.getMode() === 'record') {
      nock.recorder.rec({
        output_objects: true,
        dont_print: true
      });
    }
  }
  
  getMode() {
    return process.env.CLAUDE_RECORDING_MODE || this.config.default_mode;
  }
}
\`\`\`

## Benefits

1. **Cost Reduction**: Save money on API calls during development
2. **Speed**: Instant responses from recordings
3. **Reliability**: No network issues or API downtime
4. **Testing**: Consistent test data
5. **Debugging**: Inspect exact API interactions
6. **Compliance**: Filter sensitive data automatically

## Post-Installation

After installation, you can:
- Start recording: `/record start`
- Check status: `/record status`
- Use recordings: `/record replay`
- Get help: `/record:help`

The system is designed to be:
- **Non-intrusive**: Doesn't change your existing code
- **Flexible**: Multiple modes for different scenarios
- **Secure**: Automatic filtering of sensitive data
- **Portable**: Works across different environments
```

# .claude/commands/record.md

```md
# Record - Manage API Recording and Replay

Control API recording, replay recorded responses, or bypass to use real APIs.

**Usage**: `/record [action] [options]`

## Actions

### `start [name]` - Start Recording Session
Begin recording API interactions to a named cassette.

\`\`\`bash
/record start feature-testing
/record start login-flow --append
/record start integration --apis openai,anthropic
\`\`\`

**Options**:
- `--append` - Add to existing cassette instead of overwriting
- `--apis [names]` - Only record specific APIs (comma-separated)
- `--duration [time]` - Auto-stop after specified time (e.g., "30m", "2h")

### `stop` - Stop Recording Session
Stop the current recording session and save the cassette.

\`\`\`bash
/record stop
/record stop --save-as production-test
\`\`\`

### `replay [name]` - Use Recorded Responses
Switch to replay mode using a specific cassette.

\`\`\`bash
/record replay feature-testing
/record replay latest
/record replay --list  # Show available cassettes first
\`\`\`

### `bypass` - Use Real APIs
Temporarily bypass recordings and use actual APIs.

\`\`\`bash
/record bypass                    # Bypass all recordings
/record bypass --duration 1h      # Bypass for 1 hour
/record bypass --apis kameleo     # Bypass specific API only
\`\`\`

### `status` - Show Current State
Display current recording mode and active cassettes.

\`\`\`bash
/record status
\`\`\`

**Example Output**:
\`\`\`
🎬 Recording Status
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Mode: replay (using recorded responses)
Active Cassette: feature-testing-2024-01-15
Cassette Size: 45 requests, 2.3MB
APIs Recorded: kameleo (12), decodo (8), s3 (25)
Cost Saved: ~$4.50
Last Modified: 2 hours ago

Available Commands:
• /record bypass - Switch to real APIs
• /record start new-feature - Begin new recording
• /record:help - Get detailed help
\`\`\`

### `list` - Show Available Recordings
List all available cassettes with details.

\`\`\`bash
/record list
/record list --details
/record list --api kameleo
\`\`\`

### `delete [name]` - Remove Cassette
Delete a recorded cassette.

\`\`\`bash
/record delete old-test
/record delete --older-than 30d
/record delete --all
\`\`\`

### `info [name]` - Cassette Details
Show detailed information about a cassette.

\`\`\`bash
/record info feature-testing
\`\`\`

### `config` - Update Configuration
Modify recording settings.

\`\`\`bash
/record config --mode hybrid
/record config --filter-header x-custom-key
/record config --api-pattern "https://api.custom.com/*"
\`\`\`

## Recording Modes

### **Record Mode**
- Captures all API interactions
- Stores in cassette files
- Filters sensitive data
- Tracks costs

### **Replay Mode** (Default)
- Uses recorded responses
- No actual API calls
- Instant responses
- Zero cost

### **Bypass Mode**
- Skips recording system
- Direct API calls
- Useful for production testing
- Can be temporary

### **Hybrid Mode**
- Uses recordings if available
- Falls back to real API
- Records new interactions
- Best of both worlds

## Environment Variables

Control recording behavior with environment variables:

\`\`\`bash
# Set recording mode
export CLAUDE_RECORDING_MODE=bypass

# Set cassette directory
export CLAUDE_CASSETTE_DIR=/path/to/cassettes

# Enable debug logging
export CLAUDE_RECORDING_DEBUG=true

# Disable cost tracking
export CLAUDE_RECORDING_TRACK_COSTS=false
\`\`\`

## Instructions

When you use this command, I will:

1. **For `start` action**:
   - Initialize a new recording session
   - Set up API interceptors
   - Begin capturing requests/responses
   - Track API costs

2. **For `replay` action**:
   - Load specified cassette
   - Configure replay mode
   - Route API calls to recordings
   - Report cost savings

3. **For `bypass` action**:
   - Disable recording/replay
   - Allow direct API calls
   - Set optional time limit
   - Log actual API usage

4. **For `status` action**:
   - Show current mode
   - List active cassettes
   - Display cost tracking
   - Suggest next actions

## Examples

### Development Workflow
\`\`\`bash
# Start development with existing recordings
/record replay production-data

# Need fresh data? Switch to bypass
/record bypass --duration 10m

# Found a bug? Record the scenario
/record start bug-reproduction
# ... reproduce the bug ...
/record stop

# Share the recording with team
/record info bug-reproduction
\`\`\`

### Testing Workflow
\`\`\`bash
# Run tests with consistent data
/record replay test-fixtures

# Update test data
/record start test-fixtures --append
# ... run test scenarios ...
/record stop
\`\`\`

### Cost-Conscious Development
\`\`\`bash
# Check how much you're saving
/record status

# See detailed cost breakdown
/record info feature-testing --costs

# Use hybrid mode for new features
/record config --mode hybrid
\`\`\`

## Best Practices

1. **Name cassettes descriptively**: Use feature or ticket names
2. **Clean up old recordings**: Delete unused cassettes regularly
3. **Review before committing**: Check cassettes for sensitive data
4. **Use replay by default**: Save costs during development
5. **Document special cases**: Note any APIs that shouldn't be recorded

## Troubleshooting

If recordings aren't working:
1. Check mode: `/record status`
2. Verify setup: `/record:install --check`
3. Enable debug: `export CLAUDE_RECORDING_DEBUG=true`
4. Get help: `/record:help troubleshooting`
```

# .claude/commands/report.md

```md
# Project Report - Intelligent Status Reports

Generate intelligent project reports for different audiences and purposes.

**Usage**: `/project:report [type]`

Report Types:
- `/project:report` - General status report
- `/project:report executive` - Business-focused summary for stakeholders
- `/project:report technical` - Detailed technical progress
- `/project:report timeline` - Timeline and milestone analysis
- `/project:report risks` - Risk assessment and mitigation

## What I Do

When you run this command, I will:

1. **Gather Project Data**
   - Analyze epics and story progress
   - Review git commit history
   - Assess codebase implementation
   - Track milestone achievement

2. **Generate Tailored Reports**
   - Match report style to audience
   - Focus on relevant metrics
   - Provide actionable insights
   - Include visual progress indicators

3. **Identify Key Insights**
   - Progress trends and velocity
   - Risk factors and mitigation
   - Resource utilization
   - Timeline projections

## Report Formats

### General Status Report
\`\`\`markdown
# 📊 VR Language Learning - Project Status Report
Generated: [Date]

## Executive Summary
- **Overall Progress**: [X]% complete
- **Timeline Status**: ✅ On Track / ⚠️ At Risk / 🚨 Behind
- **Budget Health**: Within budget / Over by [X]%
- **Quality Metrics**: All tests passing / [X] issues

## Progress by Epic
### Core VR Experience
- Progress: ████████░░ 80%
- Completed: 8/10 stories
- Current: Implementing hand tracking
- Blockers: WebXR audio permissions

### Speech Recognition
- Progress: ███░░░░░░░ 30%
- Completed: 3/10 stories
- Current: Whisper API integration
- Blockers: None

[Additional epics...]

## Recent Achievements
- ✅ VR scene rendering on Quest
- ✅ Basic navigation implemented
- ✅ Database schema deployed

## Upcoming Milestones
- [ ] MVP Demo Ready - [Date]
- [ ] Speech loop complete - [Date]
- [ ] Quest store submission - [Date]

## Key Metrics
- Development Velocity: 2.5 stories/week
- Bug Resolution Time: <24 hours
- Test Coverage: 75%
- Performance: 60 FPS on Quest 2
\`\`\`

### Executive Report
\`\`\`markdown
# 🎯 VR Language Learning - Executive Briefing

## Business Impact
- **Market Opportunity**: $2B language learning market
- **Competitive Advantage**: First true VR immersion
- **Time to Market**: 8 weeks to MVP
- **ROI Projection**: Break-even at 500 users

## Key Achievements
- VR prototype functional on Quest devices
- Core learning loop validated
- AI tutor integration working

## Investment Needs
- Additional developer: $15k/month
- Quest Pro for testing: $1,000
- Marketing budget: $5k initial

## Go-to-Market Timeline
- MVP Complete: [Date]
- Beta Launch: [Date]
- Public Release: [Date]
\`\`\`

### Technical Report
\`\`\`markdown
# 🔧 VR Language Learning - Technical Status

## Architecture Health
### Frontend (React/WebXR)
- Components: 15 implemented, 5 remaining
- Bundle Size: 2.1MB (target: <3MB)
- Quest Performance: Stable 60 FPS
- Memory Usage: 450MB average

### Backend (FastAPI)
- Endpoints: 12/15 complete
- Response Time: <200ms average
- Database Queries: Optimized
- External APIs: Stable integration

## Code Quality
- Test Coverage: 75% (target: 80%)
- Linting: All passing
- Type Safety: Full TypeScript coverage
- Documentation: 90% complete

## Technical Debt
- [ ] Refactor audio processing pipeline
- [ ] Optimize VR scene for Quest 1
- [ ] Add comprehensive error handling
- [ ] Implement caching layer

## Performance Metrics
- Whisper API: 1.2s average response
- TTS Generation: 0.8s average
- Database Queries: <50ms
- WebXR Frame Time: 16ms (60 FPS)
\`\`\`

## Intelligence Features

- **Automatic Analysis**: I identify trends and patterns
- **Risk Detection**: I flag potential issues early
- **Recommendation Engine**: I suggest optimal next steps
- **Custom Metrics**: I track VR-specific performance

## VR Language Learning Specific Reporting

I track:
- **Quest Performance**: FPS, memory, thermals
- **Speech Pipeline**: Recognition accuracy, latency
- **Learning Metrics**: Progression, retention
- **User Experience**: Session length, completion rates
- **Technical Health**: API performance, error rates

## Example Usage

\`\`\`bash
/project:report executive

# Output:
# 🎯 VR Language Learning - Executive Briefing
# 
# ## Business Impact
# - Market Opportunity: $2B language learning market
# - Competitive Advantage: First true VR immersion
# - Time to Market: 6 weeks remaining to MVP
# - ROI Projection: Break-even at 500 monthly users
#
# [... continued report ...]
\`\`\`

This command provides stakeholder-appropriate views of your project's health and progress.
```

# .claude/commands/sync.md

```md
# Project Sync - Intelligent Project Status Analysis

Analyze the current state of your VR Language Learning project and provide intelligent recommendations.

**Usage**: `/project:sync`

## What I Do

When you run this command, I will:

1. **Read Project Structure**
   - Scan epics.md for epic and story definitions
   - Check implementation plan for timeline and milestones
   - Review git history for recent changes
   - Analyze codebase for implementation status

2. **Analyze Progress**
   - Track completion percentage across epics
   - Identify completed vs in-progress stories
   - Check acceptance criteria fulfillment
   - Assess technical debt accumulation

3. **Identify Dependencies**
   - Map story and epic dependencies
   - Find critical path items
   - Highlight blocking issues
   - Suggest optimal sequencing

4. **Provide Recommendations**
   - Suggest next high-impact tasks
   - Identify risks and blockers
   - Recommend resource allocation
   - Propose timeline adjustments

## Output Format

\`\`\`markdown
# 📊 VR Language Learning Project Status

## Current Sprint/Phase
- Active epic and stories
- Progress metrics
- Velocity indicators

## Epic Progress
### Epic 1: [Name]
- ✅ Completed: [X] stories
- 🚧 In Progress: [Y] stories  
- 📋 Remaining: [Z] stories
- **Blockers**: [Any blocking issues]
- **Next Steps**: [Recommended actions]

### Epic 2: [Name]
[Similar breakdown...]

## Recent Activity
- Last commits and their impact
- Completed stories in past week
- New issues or technical debt

## Recommended Next Actions
1. **High Priority**: [Task] - [Reason]
2. **Medium Priority**: [Task] - [Reason]
3. **Low Priority**: [Task] - [Reason]

## Risk Assessment
- 🚨 **Critical**: [Risk and mitigation]
- ⚠️ **Warning**: [Potential issue]
- 💡 **Opportunity**: [Quick wins available]

## Timeline Health
- Current progress vs plan
- Milestone status
- Projected completion dates
\`\`\`

## Intelligence Features

- **Automatic Prioritization**: I rank tasks by impact and dependencies
- **Risk Detection**: I identify potential blockers before they happen
- **Progress Tracking**: I calculate velocity and completion estimates
- **Context Awareness**: I understand your specific project constraints

## VR Language Learning Specific Analysis

I will specifically analyze:
- **WebXR Implementation**: Frontend VR components and hand tracking
- **Speech Pipeline**: Whisper API integration and audio processing
- **Learning System**: Sentence progression and vocabulary tracking
- **Quest Compatibility**: Performance and UX on Meta Quest devices
- **AI Integration**: GPT-4 tutor and ElevenLabs TTS implementation

## Example Usage

\`\`\`bash
/project:sync

# Output:
# 📊 VR Language Learning Project Status
# 
# ## Current Sprint/Phase
# Working on MVP Core Features (Week 1 of 2)
# - 3 stories completed, 2 in progress
# - Velocity: 1.5 stories/day
# 
# ## Epic Progress
# ### Epic 1: Core VR Experience
# - ✅ Completed: 5 stories (50%)
# - 🚧 In Progress: 2 stories
# - 📋 Remaining: 3 stories
# - **Blockers**: WebXR audio permissions on Quest
# - **Next Steps**: Complete hand tracking, then test on device
#
# [... continued analysis ...]
\`\`\`

This command gives you a complete picture of where your project stands and what needs attention next.
```

# .claude/settings.local.json

```json
{
  "permissions": {
    "allow": [
      "Bash(find:*)",
      "Bash(git init:*)"
    ],
    "deny": []
  }
}
```

# README.md

```md
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

### API Recording Commands

#### `/record [action]`
Manage API recording and replay for cost-effective development.
- Actions: `start`, `stop`, `replay`, `bypass`, `status`, `list`, `delete`, `info`
- Record API interactions to reusable cassettes
- Replay recorded responses with zero API costs
- Track cost savings automatically
- Filter sensitive data from recordings

#### `/record:install`
Install a complete API recording infrastructure.
- Auto-detects project language and framework
- Installs appropriate recording libraries (vcr, nock, etc.)
- Creates recording configuration and utilities
- Sets up test integration and CI/CD support

#### `/record:help [topic]`
Get comprehensive help for the recording system.
- Topics: `modes`, `commands`, `apis`, `troubleshooting`, `best-practices`
- Context-aware guidance
- Interactive examples
- Configuration assistance

## 🛠️ Installation

### Quick Start

1. Clone this repository or copy the `.claude` directory to your project:
\`\`\`bash
# Clone the entire repository
git clone https://github.com/andrewlwn77/claude-code-commands.git

# Or copy just the commands to your project
cp -r claude-code-commands/.claude /your/project/
\`\`\`

2. The commands are immediately available in Claude Code when you open your project.

### Installing Individual Command Sets

To install specific command sets in your existing project:

\`\`\`bash
# For project management commands
/project:install

# For MCP integration commands
/mcp:install

# For API recording commands
/record:install
\`\`\`

## 💡 Usage Examples

### Natural Language Project Management

Instead of rigid commands, just talk to Claude naturally:

\`\`\`
"What should I work on next?"
"How is the authentication epic progressing?"
"What's blocking our deployment?"
"Generate an executive summary of our progress"
\`\`\`

### Project Status Check

\`\`\`bash
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
\`\`\`

### Sprint Planning

\`\`\`bash
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
\`\`\`

### MCP Integration

\`\`\`bash
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
\`\`\`

### API Recording

\`\`\`bash
# Start recording API interactions
/record start feature-development

# Make your API calls normally...
# Then stop and save the recording
/record stop

# Later, replay without hitting real APIs
/record replay feature-development

# Check your cost savings
/record status

# Output:
# 🎬 Recording Status
# ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
# Mode: replay (using recorded responses)
# Active Cassette: feature-development
# Cassette Size: 45 requests, 2.3MB
# APIs Recorded: openai (12), stripe (8), aws (25)
# Cost Saved: ~$4.50
# Last Modified: 2 hours ago
\`\`\`

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

### MCP Server Integration (Examples)
When you install MCP integration, you can connect to various development tools. Examples include:
- **Docker Management**: Monitor and control containers
- **Database Access**: Run queries directly from Claude
- **Browser Testing**: Automate testing with Puppeteer
- **AWS Tools**: Access CDK documentation and patterns
- **IDE Features**: Get diagnostics and execute code
- **And many more**: The MCP ecosystem is constantly growing with new integrations

### API Recording & Replay
- **Cost Optimization**: Save money by replaying recorded API responses
- **Multiple Recording Modes**: Record, replay, bypass, or hybrid modes
- **Automatic Filtering**: Remove sensitive data from recordings
- **Speed & Reliability**: Instant responses without network delays
- **Testing Support**: Consistent test data across environments

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

\`\`\`markdown
# Command Name - Brief Description

Brief overview of what the command does.

**Usage**: `/namespace:command [parameters]`

## What I Do

Detailed explanation of the command's functionality...

## Example Usage

\`\`\`bash
/namespace:command parameter

# Expected output...
\`\`\`
\`\`\`

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
```

