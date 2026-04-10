# Week 13 session guide - build your research command center

Friday, April 10, 2026 | 5:30-9:00 PM | Hilton 304

---

## Tonight's schedule

| Time | What's happening |
|------|-----------------|
| 5:30 | Presentation |
| 5:50 | Workflow audit debrief |
| 6:05 | Environment setup (VS Code, research folder, Granola connector, Superpowers) |
| 6:50 | Break |
| 7:05 | Claude Code organizes your research context |
| 7:20 | Find connectors for your work |
| 7:40 | Build time - work on your #1 bottleneck |
| 8:40 | Closing + homework |

---

## Setup

Follow the setup instructions step by step: [week13-setup-instructions.md](week13-setup-instructions.md)

By the end of setup you should have:

1. VS Code installed and open
2. Your `dba-ai-research` folder open in VS Code (you created this during Week 12)
3. Your `workflow-audit.md` in the folder (required - two prompts tonight reference it. Download from Brightspace if you can't find it.)
4. Your other research files copied in (papers, data, notes)
5. Claude Code running in the VS Code terminal
6. Granola connector enabled at https://claude.ai/customize/connectors
7. Superpowers installed: `/plugin install superpowers@claude-plugins-official`

---

## Session prompts

### Prompt 1: organize your research context

Claude Code reads every file in your folder, figures out what each one is, and creates a README that indexes everything. Watch VS Code's file explorer on the left — you'll see it update in real time.

```text
Scan all the files in this folder. Before making changes, tell me what you found and what you plan
to do. Then create a README.md that indexes each file and how it relates to my research. Rename
unclear files and organize into subfolders if it makes sense.
```

### Prompt 2: find connectors for your work

Claude Code reads your workflow audit and recommends connectors that match your bottlenecks. You pick one and enable it at claude.ai/customize/connectors — same way you set up Granola.

The `@` symbol tells Claude Code to read a specific file as context. Type `@` and start typing `workflow` — it will autocomplete the path, even if the file moved during Prompt 1.

```text
@workflow-audit.md Based on my bottlenecks and data sources, recommend connectors I can enable at
claude.ai/customize/connectors. For each one, explain what it connects to and how it helps my
specific work. Then walk me through setting up whichever one I choose.
```

### Prompt 3: work on your #1 bottleneck

Claude Code reads your audit, finds your biggest bottleneck, and asks you questions before proposing anything. Use Wispr Flow to speak your answers — you'll say more than you'd type.

```text
@workflow-audit.md Identify my #1 bottleneck. Ask me one question at a time until you understand
the problem well enough to help. When you have enough context, tell me your thinking and propose
an approach. We'll agree on a plan before you build anything.
```

---

## If you get stuck

Ask Claude Code first. Open your research folder, start a session, and describe what you're stuck on. It's there at 2 AM when Greg isn't.

If Claude Code can't help, email Greg at gregory.lontok@lmu.edu or message him on Teams.

---

## Before you leave: create your CLAUDE.md

Run this inside your Claude Code session:

```
/init
```

This creates a `CLAUDE.md` file in your research folder. It's a configuration file that tells Claude Code about your project - what you're working on, what tools you use, and how you prefer to work. Every time you start a new Claude Code session in this folder, it reads this file first. Think of it as giving Claude Code a memory of your project so you don't have to re-explain things each time.

---

## Homework

Two things to do before your 1-on-1 meeting:

1. **Sync your research folder to cloud backup.** Your `dba-ai-research` folder needs to be synced to Google Drive, Dropbox, iCloud, Box, or OneDrive. Greg will ask for proof — a screenshot or live demo. If you need help setting this up, reach out.

2. **Keep Granola running in your meetings.** You need 1-2 weeks of meeting transcripts for the self-assessment prompt to work well. Just leave it running.

---

## What's next

### 1-on-1 coaching meetings (Weeks 14-16, Apr 13 - May 1)

Individual meetings where we go deep on your specific bottleneck. Come prepared with your workflow audit, your research folder, and any questions or blockers.

You must meet with Greg at least twice during the three-week window.

**Schedule here:** https://calendly.com/greg-lontok/dba-ai-1-on-1

**What to have ready:**
- `dba-ai-research` folder synced to cloud backup (bring proof)
- Your workflow audit reviewed
- Superpowers installed (if you didn't finish tonight, we'll do it together)
- Questions or blockers you've hit

### Demo Day (Finals week)

**Friday, May 8 | 9:00-10:30 AM | Zoom:** https://lmula.zoom.us/my/lontok

Present your workflow and its output to the class. Live demo, show what you built, Q&A.
