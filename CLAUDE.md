# Claude Code Project Instructions

You are acting as an agentic developer for this project. Your primary goal is to maintain project continuity and self-improve by using this `CLAUDE.md` file as your persistent memory and task coordinator.

---

## 🧠 Memory & Lessons Learned
Whenever you encounter a reusable pattern, a specific library version requirement, or a fix to a mistake you made:
1.  **Self-Correction**: Immediately update the `## 📚 Lessons Learned` section in this file.
2.  **Context**: Include the date and a concise description of the "lesson" so you do not repeat the error in future sessions.

---

## 📝 Task Management (Scratchpad)
Use the `## 🏗️ Scratchpad` section at the bottom of this file for every task:
1.  **Initialization**: When a new task starts, clear the old Scratchpad.
2.  **Planning**: Explain the task in your own words and list the atomic steps using `[ ]` checkboxes.
3.  **Execution**: Update `[ ]` to `[X]` as you complete subtasks.
4.  **Reflection**: Upon reaching a milestone, update the plan if the "big picture" has changed.
5.  **Always refer to the Scratchpad** before suggesting or executing the next command.

---

## 🛠️ Tooling & Environment

### Python Environment
- **Virtual Env**: Located at `./venv`.
- **Activation**: You must ensure the venv is active for all Python commands.
- **Packages**: 
  1. Check for `uv` (`which uv`). 
  2. If present: Use `uv pip install`.
  3. Otherwise: Fall back to `pip install`.

### Custom Tools (Python 3)
- **Screenshot Verification**: 
  - Capture: `venv/bin/python3 tools/screenshot_utils.py <URL> [--output <path>]`
  - LLM Verify: `venv/bin/python3 tools/llm_api.py --prompt "..." --provider {openai|anthropic} --image <path>`
- **LLM API**: Use `tools/llm_api.py`. Default is `openai` (gpt-4o).
- **Web Browser**: `venv/bin/python3 tools/web_scraper.py --max-concurrent 3 <URLs>`
- **Search Engine**: `venv/bin/python3 tools/search_engine.py "<keywords>"`
  - *Note: Always use the current year (2026) for time-sensitive queries.*

### Git Workflow
- **Commit Messages**: For multiline messages, write the message to a temporary file first, then use `git commit -F <filename>`. Delete the temp file afterward.
- **Prefix**: Include `[Claude] ` in all commit messages and PR titles.

---

## 📚 Lessons Learned

### User Specified
- Always use the `./venv` environment. Check for `uv` availability first.
- For multiline git commits, use the file-based (`-F`) approach to avoid terminal character issues.

### Claude Learned
- [2026-02-23] **Matplotlib**: Use style `seaborn-v0_8` instead of the deprecated `seaborn`.
- [2026-02-23] **Vision Tasks**: Use model name `gpt-4o` for OpenAI vision-related API calls.
- [2026-02-23] **Search**: Ensure UTF-8 handling for non-English search results.

---

## 🏗️ Scratchpad
### Current Task: 
[Pending Task Description]

### Plan:
- [ ] Step 1: Initialize environment and verify tools
- [ ] Step 2: ...