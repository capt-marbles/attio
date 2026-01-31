# Attio CRM - OpenClaw Skill

Enhanced Attio CRM integration with batch operations, improved error handling, data validation, enrichment functions, and robust task management.

## Features

- 📦 **Batch Operations** - Efficiently import large volumes of records
- 🔄 **Retry Logic** - Automatic retry on rate limits with exponential backoff
- ✅ **Data Validation** - Validate data before import to prevent errors
- 🔍 **Enrichment Functions** - Enhance records with additional data
- 📋 **Task Management** - Robust task creation and tracking
- ⚡ **Progress Tracking** - Monitor bulk operations in real-time

## Quick Start

### 1. Setup

Set your Attio API key:
```bash
echo "ATTIO_API_KEY=your_api_key" >> ~/.env
```

Get your API key: Attio → Workspace Settings → Developers → New Access Token

### 2. Installation

```bash
# Via ClawHub (once published)
clawdhub install attio

# Via GitHub
git clone https://github.com/capt-marbles/attio ~/.openclaw/skills/attio
```

### 3. Usage

```bash
# Batch import companies
attio-enhanced batch import companies data.json

# Create a record with validation
attio-enhanced records create company data.json

# Enrich records with additional data
attio-enhanced enrich company-id
```

## Use Cases

Perfect for:
- **Sales prospecting** - Import and manage large prospect lists
- **Data migration** - Move existing CRM data into Attio
- **Lead enrichment** - Enhance contact records with additional data
- **Task automation** - Create and manage tasks programmatically
- **Bulk operations** - Handle large volumes of CRM data efficiently

## Documentation

See [SKILL.md](SKILL.md) for complete documentation.

## Requirements

- Attio API key
- `jq` for JSON processing
- `curl` for API requests

## License

MIT

## Author

Gameye Sales Team