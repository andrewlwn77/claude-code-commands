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

```markdown
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
```

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

```bash
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
```

This command gives you a complete picture of where your project stands and what needs attention next.