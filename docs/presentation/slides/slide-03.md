# Slide 03: Installing Claude Code
**Duration**: 3 minutes | **ADR**: PRES-003

---

## What is Claude Code?

> An AI-powered CLI that integrates directly into your terminal.
> It reads your codebase, understands context, and writes production code.

---

## Installation

### macOS / Linux (Recommended)

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

### Windows (Recommended)

```powershell
irm https://claude.ai/install.ps1 | iex
```

### Homebrew (macOS/Linux)

```bash
brew install --cask claude-code
```

### WinGet (Windows)

```bash
winget install Anthropic.ClaudeCode
```

---

## First Run Setup

```bash
# 1. Set your API key
export ANTHROPIC_API_KEY="sk-ant-..."

# 2. Initialize in your project
cd /workspaces/huron-portland
claude

# 3. Claude Code reads your codebase automatically:
#    - CLAUDE.md (project instructions)
#    - package.json, go.mod (dependencies)
#    - Architecture docs (ADRs, DDD)
```

---

## Key Capabilities

```
┌──────────────────────────────────────────┐
│          CLAUDE CODE FEATURES            │
├──────────────┬───────────────────────────┤
│ Read Files   │ Understands entire repo   │
│ Write Code   │ Creates production code   │
│ Run Commands │ Execute builds & tests    │
│ Multi-file   │ Edits across the project  │
│ Git Native   │ Commits, branches, PRs    │
│ Agent Tasks  │ Spawns sub-agents         │
│ Web Search   │ Finds docs & solutions    │
│ MCP Servers  │ Extends with custom tools │
└──────────────┴───────────────────────────┘
```

---

## The CLAUDE.md File

```markdown
# CLAUDE.md - Your AI's instruction manual
## Project Structure (what goes where)
## Coding Standards (how to write)
## Swarm Patterns (how to coordinate)
## Domain Context (what the app does)
## File Organization (never save to root)
```

> This file is the single most important artifact
> for controlling AI agent behavior.

---

### [ILLUSTRATION: Terminal screenshot mockup showing Claude Code CLI interface. Left side shows a prompt. Right side shows generated code appearing in real-time. Clean dark theme with syntax highlighting. Include the Claude logo subtly in the terminal prompt.]
