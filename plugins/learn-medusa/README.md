# Learn Medusa - Interactive Tutorial Plugin

An interactive, guided tutorial for learning Medusa development from scratch by building a brands feature. Claude acts as your coding bootcamp instructor, teaching you step-by-step with checkpoints and verification.

> For installation and usage with other agents, refer to the [main README](../../README.md).

- [Installation with Claude Code](#installation-with-claude-code)
  - [Prerequisites](#prerequisites)
  - [Install Plugin](#install-plugin)
- [Installation for Other AI Agents](#installation-for-other-ai-agents)
- [Usage](#usage)
- [What You'll Learn](#what-youll-learn)
  - [Lesson 1: Build Custom Features (45-60 min)](#lesson-1-build-custom-features-45-60-min)
  - [Lesson 2: Extend Medusa (45-60 min)](#lesson-2-extend-medusa-45-60-min)
  - [Lesson 3: Customize Admin Dashboard (45-60 min)](#lesson-3-customize-admin-dashboard-45-60-min)
- [Features](#features)
- [Privacy](#privacy)

## Installation with Claude Code

### Prerequisites

- [Claude Code](https://github.com/anthropics/claude-code) installed
- A Medusa project (or planning to create one)

### Install Plugin

1. Start Claude:

```bash
claude
```

2. Add Medusa marketplace to Claude Code:

```bash
/plugin marketplace add medusajs/medusa-agent-skills
```

3. Install the plugin:

```bash
/plugin install learn-medusa@medusa
```

4. Verify the plugin is loaded:

```bash
/plugin
```

## Installation for Other AI Agents

For other AI agents like Cursor, you can use the [skills](https://skills.sh/) command to install the plugin's skills based on your AI agent:

```bash
npx skills add medusajs/medusa-agent-skills
# choose the following skills:
# - building-with-medusa
# - building-admin-dashboard-customizations
# - building-storefronts
# - db-generate
# - db-migrate
# - new-user
```

## Usage

Ask Claude to teach you:
- "Teach me how to build with Medusa"
- "Guide me through Medusa development"
- "I want to learn Medusa"

Claude will start an interactive tutorial where you'll build a brands feature while learning Medusa's architecture.

You can also trigger the skill manually with `/learn-medusa:learning-medusa`.

## What You'll Learn

### Lesson 1: Build Custom Features (45-60 min)

- Create a Brand Module (data model, service, migrations)
- Build a Workflow for creating brands (with rollback logic)
- Expose an API Route for creating brands (with validation)

### Lesson 2: Extend Medusa (45-60 min)

- Link brands to products using Module Links
- Extend core workflows using Workflow Hooks
- Query linked data across modules

### Lesson 3: Customize Admin Dashboard (45-60 min)

- Create a Widget to display brand on product page
- Build a UI Route for managing brands
- Use React Query and Medusa UI components

## Features

- **Interactive**: Claude guides you step-by-step, verifying your work at checkpoints
- **Architecture-Focused**: Learn WHY, not just WHAT
- **Error-Friendly**: Errors are treated as teaching opportunities
- **Hands-On**: Build a real feature (brands) while learning
- **Progressive**: Start simple, build complexity gradually

## Privacy

This plugin does not collect, store, or transmit any user data or conversation information. All instructional content is provided locally through skill files, and the MCP server only queries public Medusa documentation.
