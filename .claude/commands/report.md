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
```markdown
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
```

### Executive Report
```markdown
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
```

### Technical Report
```markdown
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
```

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

```bash
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
```

This command provides stakeholder-appropriate views of your project's health and progress.