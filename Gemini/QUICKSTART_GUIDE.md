# QUICKSTART GUIDE: AI-ASSISTED DEVELOPMENT (BEGINNER FRIENDLY)

Welcome! This setup allows you to build software safely with AI tools like ChatGPT, Gemini, Claude, Claude Code, or Codex—even if you are a beginner ("vibe coder").

---

## 1. How the 3-Role AI Workflow Works

Instead of asking one AI to do everything, you separate responsibilities across 3 prompts:

1. **AI 1 — Engineering Advisor / Product Owner (ChatGPT / Gemini / Claude Web)**
   - **Role:** Planner & Technical Lead.
   - **Job:** Helps you define your app, designs architecture, breaks work into tiny safe steps, and writes ready-to-copy prompts for AI 2.

2. **AI 2 — Coding Agent (Claude Code / Codex / Gemini CLI / Cursor)**
   - **Role:** Developer.
   - **Job:** Runs in your terminal/editor, inspects files, writes code, runs tests, and reports diffs.

3. **AI 3 — Independent Reviewer (OpenCodeReview / ChatGPT / Claude)**
   - **Role:** Security & QA Auditor.
   - **Job:** Inspects the diff before you commit to make sure there are no bugs or security flaws.

4. **YOU — The Project Owner**
   - **Role:** Final Approver.
   - **Job:** Copy-paste prompts between AI tools, grant permission for each step, and press "Approve".

---

## 2. Step-by-Step Instructions to Start a New Project

### Step 1: Initialize AI 1 (Engineering Advisor)
1. Open ChatGPT, Gemini, or Claude in your browser.
2. Paste the entire contents of **`PROMPT_A_ENGINEERING_ADVISOR.md`**.
3. Send your first message:
   > *"I want to build [YOUR IDEA HERE, e.g., 'a simple web application to track daily habits using React and Node.js']." *
4. AI 1 will guide you through discovery, recommend a tech stack, and generate your first command for AI 2.

### Step 2: Initialize AI 2 (Coding Agent)
1. Open your terminal or coding tool (e.g., Claude Code, Cursor, terminal with Gemini CLI).
2. Open your project folder.
3. Paste **`PROMPT_B_CODING_AGENT.md`** as your system prompt or initial instructions.
4. Copy the exact task prompt that AI 1 generated for you in Step 1 and paste it to AI 2.
5. AI 2 will analyze your project and report back.

### Step 3: Review & Loop
1. Copy AI 2's output back into your AI 1 chat session.
2. AI 1 will verify the work. When code changes are ready, copy the patch/diff into **`PROMPT_C_INDEPENDENT_REVIEWER.md`** for a quick sanity check.
3. Once approved, allow AI 2 to commit and push!

---

## 3. Strict Rules for Beginners
- Never let a coding agent push or deploy without checking with AI 1 first.
- Always keep changes small (one feature at a time).
- If something breaks, ask AI 1 to generate an investigation prompt for AI 2 instead of randomly changing code.
