# Project Intelligence & Memory (Codex)

## 🤖 Role & Core Protocol
You are an expert software engineer. Your goal is to maintain project continuity by strictly following the **Lessons** and **Scratchpad** system defined below.

---

## 🧠 Memory Management (The Lessons System)
Whenever you discover a reusable pattern, fix a mistake, or receive a correction:
1.  **Update this file**: Immediately record the insight in the `## 📚 Lessons Learned` section.
2.  **Scope**: Include library versions, model names, and specific "gotchas" discovered during development.
3.  **Persistence**: This file is your "Long-term Memory". Always check it before starting a new task.

---

## 📝 Active Task Management (The Scratchpad)
Use the `## 🏗️ Current Scratchpad` section as your "Short-term Memory".
- **New Task**: Clear the old Scratchpad. Explain the new task in your own words.
- **Planning**: Break it down into atomic steps with checkboxes.
- **Progress**: Update `[ ]` to `[X]` as you finish subtasks.
- **Reflection**: After milestones, update the Scratchpad to refine the next steps.

---

## 🛠️ Toolchain Specifications

### 🐍 Python Environment
- **Venv**: Always use the virtual environment in `./venv`. 
- **Package Manager**: 
  1. Check for `uv` first (`which uv`).
  2. If `uv` exists: `source venv/bin/activate && uv pip install <package>`.
  3. Otherwise: `source venv/bin/activate && pip install <package>`.

### 📸 Screenshot & Verification
- **Capture**: `venv/bin/python3 tools/screenshot_utils.py <URL> [--output OUTPUT]`
- **LLM Verify**: `venv/bin/python3 tools/llm_api.py --prompt "..." --provider {openai|anthropic} --image <path>`

### 🤖 LLM & Web Tools
- **LLM API**: Use `tools/llm_api.py`. Default provider: `openai` (Model: `gpt-4o`).
- **Browsing**: Use `tools/web_scraper.py` for content extraction.
- **Search**: Use `tools/search_engine.py` for web queries. Use current year **2026** for time-sensitive queries.

### 🐙 Git & GitHub Workflow
- **Commit Messages**: For multiline messages, write to a temporary file and use `git commit -F <file>`.
- **Tagging**: Prefix all commit messages and PR titles with `[Codex] `.

---

## 📚 Lessons Learned

### User Specified
- Always activate `./venv` before execution.
- Matplotlib Style: Use `seaborn-v0_8` (not `seaborn`).
- OpenAI Vision: Use model name `gpt-4o`.

### Automatically Learned
- [Entry 2026-02-23]: Ensure UTF-8 encoding for international search queries.
- [Entry 2026-02-23]: Use current year 2026 for recent news searches.

---

## 🏗️ Current Scratchpad
### Task Definition:
[Describe the current goal here]

### Action Plan:
- [ ] Step 1: ...
- [ ] Step 2: ...