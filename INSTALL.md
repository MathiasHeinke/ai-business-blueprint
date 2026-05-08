# Installation Guide

The AI Business Blueprint is a collection of plain Markdown files. It works with **any** AI assistant. Below is a tool-specific guide for the most common ones — pick yours and you'll be running in under 10 minutes.

---

## Before you start

You don't need to be a developer. You don't need to install anything technical. You only need:

1. An AI assistant of your choice (Claude, ChatGPT, Cursor, Continue, Codex CLI, Gemini, etc.)
2. The files from this repo (download as ZIP via the green **Code** button, or `git clone`)

That's it.

---

## Option A — Claude Desktop (recommended for non-developers)

**Best for:** founders who want a clean chat-style assistant with project context.

### Step 1 — Get the files
- On GitHub, click the green **Code** button → **Download ZIP**
- Unzip somewhere stable, e.g. `~/Documents/ai-business-blueprint/`

### Step 2 — Set up a Claude Project
- Open Claude (web or desktop)
- Click **+ New Project** in the sidebar
- Name it: *AI Business Blueprint*
- In **Project knowledge**, upload:
  - `README.md`
  - `frameworks/00-overview.md`
  - The 4–5 files from `frameworks/` most relevant to your current focus (e.g. `02-diagnostics/`)
  - `prompts/ai-prompts.md`

### Step 3 — Paste the system prompt
In the Project's **Custom Instructions**, paste this:

```
You are an experienced operator and strategist. Your job is to help me apply
the AI Business Blueprint to my specific business. Operating principles:

1. Always ground your advice in the framework files I uploaded. Cite them by
   filename when relevant.
2. Default to fewer questions, more direct recommendations. I want signal,
   not therapy.
3. Use the diagnostic frameworks (Traffic-Systems-Skills, 1-1-1, Bottleneck
   Finder) before suggesting solutions.
4. When I ask a vague strategic question, run me through the four-step
   decision framework: Context → Issue → Risk → Map.
5. When I describe a problem, ask: "What's the smallest version of the fix
   that would still work?"
6. Replace "we should think about X" with "do X by Y, here's how."

Respond in clear, plain prose. No emoji. No filler. No "great question!"
```

### Step 4 — Start working
Open the project. Try one of these:

> *"Run me through the Diagnostic Checklist. My business is [your situation]."*

> *"Apply the Two Magic Questions to my product. Help me write the customer interview script."*

> *"I'm stuck. My business does $[X]/month. Use the Traffic-Systems-Skills framework to find my bottleneck."*

---

## Option B — Cursor / Windsurf / VS Code with AI

**Best for:** founders comfortable in code editors.

### Step 1 — Clone the repo
```bash
git clone https://github.com/<your-username>/ai-business-blueprint.git
cd ai-business-blueprint
```

### Step 2 — Open in your editor
Open the folder. Your AI panel can now read all files.

### Step 3 — Reference the framework
In the AI sidebar, type:

```
@frameworks Use the AI Business Blueprint as my operating system.
Run me through the Diagnostic Checklist for my business.
```

Cursor will load the relevant files into context automatically.

### Step 4 — Apply prompts
Open `prompts/ai-prompts.md` for ready-to-use prompts per scenario.

---

## Option C — ChatGPT / any web-based assistant

**Best for:** quick one-off sessions, no installation.

### Step 1 — Pick your file
Decide which framework you need right now. If unsure, start with `frameworks/00-overview.md` and `frameworks/02-diagnostics/03-bottleneck-finder.md`.

### Step 2 — Paste into ChatGPT
Open the file on GitHub, click **Raw**, copy everything. In ChatGPT:

```
This is my business operating framework. Read it carefully and use it to
answer my next question.

[paste the framework content here]

Now: my business is [describe in 2-3 sentences]. Apply the framework.
```

### Step 3 — Iterate
Each conversation can pull in a different framework file. Save useful chats with descriptive titles so you can revisit.

**Pro tip:** for long-form work, use ChatGPT's **Custom GPT** feature. Create one named "AI Business Blueprint" and upload the `frameworks/` folder once.

---

## Option D — OpenAI Codex CLI / Continue / any IDE plugin

**Best for:** developers who already use AI in their IDE.

### Step 1 — Clone
```bash
git clone https://github.com/<your-username>/ai-business-blueprint.git ~/blueprint
```

### Step 2 — Tell your tool where to look
For most IDE-based AI tools, set your project workspace or context to include `~/blueprint/frameworks/`.

In Continue (`config.json`):
```json
{
  "contextProviders": [
    { "name": "folder", "params": { "folder": "~/blueprint/frameworks" } }
  ]
}
```

### Step 3 — Use the prompts
The prompts in `prompts/ai-prompts.md` are designed to work in any of these tools.

---

## Option E — Gemini / Perplexity / any other assistant

The pattern is the same:

1. Get the files (ZIP or clone).
2. Upload or paste the relevant framework file(s).
3. Reference them in your prompt: *"Apply the framework above to my situation: [description]"*

If your assistant supports **system prompts** or **custom instructions**, paste the prompt from Option A → Step 3.

---

## Recommended workflow (after install)

The Blueprint is most powerful when used in a rhythm, not a one-off:

| Cadence | What to run |
|---|---|
| **Daily** | Use AI as your memo-writing partner. Any decision → write a memo (Template in `09-templates-and-worksheets/01-memo-template.md`). |
| **Weekly** | Sunday session: Top-3 priorities for the week, using the Attention Management framework (`01-core-principles/03-attention-management.md`). |
| **Monthly** | Run the Diagnostic Checklist (`08-implementation-plan/03-diagnostic-checklist.md`). |
| **Quarterly** | Soft Shop review (`04-business-architecture/02-soft-shop-strategy.md`) and Bottleneck audit. |

---

## When you need implementation, not just diagnosis

This repo helps you diagnose and simplify the business. It does not install an
AI operating system into your company.

If the Blueprint shows that your company has a real bottleneck, repeatable
workflows, and a safe first department wedge, the next step is a **Company.OS
Readiness Audit** by FYN Labs.

The audit checks:

- current AI usage and tool sprawl
- GDPR / privacy / governance risks
- which workflows can safely use AI first
- what should stay human-gated
- the likely first department rollout
- a savings and capacity range, not a guaranteed claim

Typical path:

```text
Blueprint self-diagnosis
-> Company.OS Readiness Audit
-> first department pilot
-> done-for-you Company.OS implementation
```

Contact: [support@fyn-labs.com](mailto:support@fyn-labs.com)

---

## Troubleshooting

**"My AI keeps giving generic advice."**
→ The framework files aren't in context. Re-upload, or paste the relevant file directly into the prompt.

**"I have too much context now and the AI is confused."**
→ Don't load all 33 files at once. Load 3–5 relevant to the question at hand. Less is more.

**"I want the AI to remember my situation between sessions."**
→ Use Claude Projects, ChatGPT Custom GPTs, or save your business profile to a file like `my-business.md` and include it in every session.

**"How do I keep up with updates?"**
→ Star the repo on GitHub. Watch releases for major updates.

---

## Next: see [README.md](README.md) for what to expect from your first 30 days.
