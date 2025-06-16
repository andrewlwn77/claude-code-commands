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
   ```
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
   ```

4. **Generating Configuration**
   ```json
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
   ```

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
```python
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
```

### Node.js Setup
```javascript
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
```

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