# vibecoding-memory

Memory and workflow templates for AI coding assistants.

This repository keeps assistant-specific instruction files that enforce two habits:
- Long-term memory via a `Lessons` section
- Short-term execution tracking via a `Scratchpad` section

## Repository layout

- `AGENTS.md`: Codex-focused protocol (lessons, scratchpad, tooling, git conventions)
- `.codexrules`: Codex rules mirror
- `CLAUDE.md`: Claude-focused protocol
- `.cursorrules`: Cursor-focused protocol

## How it works

1. Start each new task by clearing and rewriting the scratchpad for that task.
2. Break work into atomic checkbox steps and update progress as you execute.
3. Record reusable lessons immediately when you discover constraints, fixes, or gotchas.
4. Follow the toolchain and git conventions defined in each assistant file.

## Why use this

- Reduces repeated mistakes across sessions
- Preserves project-specific context in-repo
- Standardizes behavior across Codex, Claude, and Cursor

## Current scope

This repo currently stores memory/process docs. Add project code as needed and extend this README with setup and architecture details when the codebase grows.
