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

```markdown
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
```mermaid
graph LR
    A[Setup WebXR] --> B[Audio Recording]
    B --> C[Whisper Integration]
    C --> D[Progress Tracking]
    D --> E[Quest Testing]
```

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
```

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

```bash
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
```

This command helps you make intelligent decisions about what to build next and in what order.