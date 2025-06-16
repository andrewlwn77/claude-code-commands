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
```
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
```

### Recording Modes (`/record:help modes`)
```
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
```

### Command Reference (`/record:help commands`)
```
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
```

### API Configuration (`/record:help apis`)
```
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
```

### Troubleshooting (`/record:help troubleshooting`)
```
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
```

### Best Practices (`/record:help best-practices`)
```
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
```

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