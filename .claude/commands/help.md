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
```
/project:sync
```
I'll analyze everything and tell you where you are, what's blocking progress, and what to work on next.

### Step 2: Plan Next Phase
```
/project:plan
```
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
```
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
```

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