# Record - Manage API Recording and Replay

Control API recording, replay recorded responses, or bypass to use real APIs.

**Usage**: `/record [action] [options]`

## Actions

### `start [name]` - Start Recording Session
Begin recording API interactions to a named cassette.

```bash
/record start feature-testing
/record start login-flow --append
/record start integration --apis openai,anthropic
```

**Options**:
- `--append` - Add to existing cassette instead of overwriting
- `--apis [names]` - Only record specific APIs (comma-separated)
- `--duration [time]` - Auto-stop after specified time (e.g., "30m", "2h")

### `stop` - Stop Recording Session
Stop the current recording session and save the cassette.

```bash
/record stop
/record stop --save-as production-test
```

### `replay [name]` - Use Recorded Responses
Switch to replay mode using a specific cassette.

```bash
/record replay feature-testing
/record replay latest
/record replay --list  # Show available cassettes first
```

### `bypass` - Use Real APIs
Temporarily bypass recordings and use actual APIs.

```bash
/record bypass                    # Bypass all recordings
/record bypass --duration 1h      # Bypass for 1 hour
/record bypass --apis kameleo     # Bypass specific API only
```

### `status` - Show Current State
Display current recording mode and active cassettes.

```bash
/record status
```

**Example Output**:
```
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
```

### `list` - Show Available Recordings
List all available cassettes with details.

```bash
/record list
/record list --details
/record list --api kameleo
```

### `delete [name]` - Remove Cassette
Delete a recorded cassette.

```bash
/record delete old-test
/record delete --older-than 30d
/record delete --all
```

### `info [name]` - Cassette Details
Show detailed information about a cassette.

```bash
/record info feature-testing
```

### `config` - Update Configuration
Modify recording settings.

```bash
/record config --mode hybrid
/record config --filter-header x-custom-key
/record config --api-pattern "https://api.custom.com/*"
```

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

```bash
# Set recording mode
export CLAUDE_RECORDING_MODE=bypass

# Set cassette directory
export CLAUDE_CASSETTE_DIR=/path/to/cassettes

# Enable debug logging
export CLAUDE_RECORDING_DEBUG=true

# Disable cost tracking
export CLAUDE_RECORDING_TRACK_COSTS=false
```

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
```bash
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
```

### Testing Workflow
```bash
# Run tests with consistent data
/record replay test-fixtures

# Update test data
/record start test-fixtures --append
# ... run test scenarios ...
/record stop
```

### Cost-Conscious Development
```bash
# Check how much you're saving
/record status

# See detailed cost breakdown
/record info feature-testing --costs

# Use hybrid mode for new features
/record config --mode hybrid
```

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