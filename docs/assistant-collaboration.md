# Collaborating with the AI assistant (plain-English guide)

Use this short checklist to get clear, useful help from the built-in AI assistant—no IDE required. It works from a phone, tablet, or any browser tab.

**If you’re on mobile or a tablet:**
- Say you’re on mobile so replies stay short.
- Ask for copy/paste-ready snippets with minimal scrolling and tap-by-tap steps.
- Prefer text over screenshots; if you must share an image, add a 1–2 line description.

## 1) Say the goal first
- In one sentence, state what you want to build, fix, or learn.
- Add limits up front: deadlines, files to avoid, preferred tools, or privacy/security rules.
- If you only need ideas or a draft (not production code), call that out.
- Mention where you’re working (web app, mobile browser, SSH) so the assistant tailors steps accordingly.

## 2) Share exactly what you see
- Paste logs, errors, or command output directly; avoid summaries like "it broke." Copy/paste beats screenshots whenever possible.
- Include the exact command and file path that produced the issue so the assistant can reproduce it.
- On small screens, send shorter snippets in separate messages—long screenshots are harder to read and quote back.
- Handy project commands:
  - `pnpm dev` – run the app locally.
  - `pnpm test` – run unit tests (Vitest).
  - `pnpm lint` – check code style.
- Mention your environment if it differs (OS, Node version, package manager).

## 3) Ask for one move at a time
- Request a single clear action (e.g., "fix this error" or "add a test for X").
- If you’re on a small screen, ask for short, copy/paste steps. Ask to repeat commands near where they’re used so you don’t have to scroll.
- After the response, ask for a quick recap if you want confirmation before continuing.

## 4) State your preferences
- Call out coding style, libraries to use or avoid, and how much explanation you want.
- Note if you expect tests, docs updates, or screenshots with the answer.

## 5) Invite options when unsure
- Ask for 2–3 approaches with quick pros/cons, then pick one to execute.
- If time is tight, request the “fastest shippable” option instead of full refactors.

## 6) Define “done”
- Spell out what a complete answer must include: summary, tests run, follow-ups, and whether you want a PR.
- Say if you prefer commands you can run directly (no IDE) or copy-ready snippets.

---

### Quick-start message template
Copy, fill, and paste (add "I’m on mobile" if needed):
```
Goal: <what you need>
Constraints: <deadlines, files to avoid, tools, security/privacy notes>
Current info: <logs, errors, commands run>
Preferences: <style, libraries, explanation depth, tests/docs/screenshots>
Finish line: <what you expect back>
```

### Example filled-in message
```
Goal: Fix the failing sidebar toggle in mobile view.
Constraints: I’m on my phone; please keep steps short. No changes to API routes.
Current info: `pnpm test sidebar` fails with "Cannot read property 'open' of undefined" in app/sidebar.tsx line 42.
Preferences: Use existing Tailwind classes; brief explanation only. Include the exact test command to rerun.
Finish line: Patch + test command I can run from Terminal, plus a one-line summary of what changed.
```

### Example for quick mobile help
```
Goal: Unblock a lint error while I’m away from my laptop.
Constraints: I’m on a phone; please keep replies under 8 lines and include copy/paste commands.
Current info: `pnpm lint` fails with "Prefer const" in app/layout.tsx line 18 and "Unused variable user" in lib/auth.ts line 72.
Preferences: Show the minimal code edits inline; no screenshots. Repeat each command near the related fix.
Finish line: Exact code snippets to paste plus the lint command to rerun.
```

### Another example (non-code)
```
Goal: Draft release notes for the latest update.
Constraints: I’m on a tablet; please keep formatting simple Markdown. Highlight only user-facing changes.
Current info: Features shipped: new mobile sidebar, faster model switching, and a bug fix for 500 errors when saving projects.
Preferences: Keep it concise (under 8 bullet points) and add a short headline.
Finish line: A ready-to-paste Markdown section I can drop into the changelog.
```

### Ultra-short mobile ask (copy/paste)
```
Goal: <what you need>
Context: I’m on <phone/tablet>. Keep replies under <X> lines.
What I see: <error/command output + file path>
Finish line: <code snippet/steps + command to rerun>
```

Using this checklist keeps the conversation fast, focused, and ready for immediate action without needing an IDE.
