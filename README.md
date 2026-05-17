# ai-branch

[![npm version](https://img.shields.io/npm/v/ai-branch)](https://www.npmjs.com/package/ai-branch)
[![npm downloads](https://img.shields.io/npm/dm/ai-branch)](https://www.npmjs.com/package/ai-branch)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue.svg)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/Node.js-%3E%3D18-green.svg)](https://nodejs.org/)

> Generate conventional git branch names from plain English. Stop wasting time on naming.

## Features

- Describe your task in plain English, get a clean branch name back
- Follows conventional prefixes: `feat/`, `fix/`, `chore/`, `docs/`, `refactor/`
- Auto-checkout option to create and switch to the branch instantly
- Kebab-case formatting for clean git history
- Powered by GPT-4o-mini for fast, accurate naming

## Installation

Run directly with npx:

```bash
npx ai-branch "your task description"
```

Or install globally:

```bash
npm install -g ai-branch
```

## Setup

Set your OpenAI API key:

```bash
export OPENAI_API_KEY=sk-...
```

## Usage

```bash
# Generate a branch name
npx ai-branch "Add dark mode to settings"
# → feat/add-dark-mode-settings

# Generate and checkout in one command
npx ai-branch "Fix login redirect loop" --checkout
# → fix/login-redirect-loop (creates branch and switches to it)

# Refactoring task
npx ai-branch "Extract user validation into separate module"
# → refactor/extract-user-validation-module
```

## Options

| Option | Description |
|--------|-------------|
| `-c, --checkout` | Create the branch and switch to it automatically |
| `-h, --help` | Show help message |

## How It Works

1. Send your plain English description to GPT-4o-mini
2. AI picks the right conventional prefix based on context
3. Formats the name in kebab-case
4. Optionally creates and checks out the branch

## Why Use This?

Consistent branch naming makes your git history scannable. No more `my-fix`, `test123`, or `johns-branch`. Every branch follows the same pattern, making PRs and changelogs cleaner.

## License

MIT

---

**Built by [LXGIC Studios](https://lxgicstudios.com)**

🔗 [GitHub](https://github.com/lxgicstudios) · [Twitter](https://x.com/lxgicstudios)

💡 Want more free tools like this? We have 100+ on our GitHub: [github.com/lxgicstudios](https://github.com/lxgicstudios)
