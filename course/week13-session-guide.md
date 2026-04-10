# Week 13 session guide — build your research command center

Friday, April 10, 2026 | 5:30-9:00 PM | In person, LMU

---

## Tonight's schedule

| Time | What's happening |
|------|-----------------|
| 5:30 | Workflow audit debrief |
| 5:50 | Environment setup (VS Code, research folder, Granola MCP) |
| 6:35 | Claude Code organizes your research context |
| 6:50 | Break |
| 7:05 | Find MCP plugins for your work |
| 7:25 | Build time — work on your #1 bottleneck |
| 8:25 | Install Superpowers |
| 8:40 | Closing + homework |

---

## Setup

Full instructions: [week13-setup-instructions.md](week13-setup-instructions.md)

Quick reference:

**Create your research folder:**

Mac:
```
mkdir ~/Documents/dba-ai-research
cd ~/Documents/dba-ai-research
```

Windows:
```
mkdir $HOME\Documents\dba-ai-research
cd $HOME\Documents\dba-ai-research
```

**Copy your dissertation files in.** Research papers, data files, your workflow audit — anything relevant. Copy, don't move. Originals stay where they are.

**Open the folder in VS Code:** File > Open Folder > select `dba-ai-research`

**Start Claude Code** in the VS Code terminal:
```
claude
```

**Connect Granola MCP** (exit Claude Code first with `/exit`):
```
claude mcp add --transport http granola https://mcp.granola.ai/mcp
```

Then start Claude Code again and type `/mcp` to authenticate.

---

## Session prompts

### Prompt 1: organize your research context

Claude Code reads every file in your folder, figures out what each one is, and creates a README that indexes everything. Watch VS Code's file explorer on the left — you'll see it update in real time.

```text
Scan all the files in this folder. Before making changes, tell me what you found and what you plan
to do. Then create a README.md that indexes each file and how it relates to my research. Rename
unclear files and organize into subfolders if it makes sense.
```

### Prompt 2: find MCP plugins for your work

Claude Code reads your workflow audit and recommends data connectors that match your bottlenecks. You pick one and install it.

The `@` symbol tells Claude Code to read a specific file as context. Type `@` and start typing `workflow` — it will autocomplete the path, even if the file moved during Prompt 1.

```text
@workflow-audit.md Based on my bottlenecks and data sources, recommend plugins or data connectors
I can install right now. For each one, explain what it connects to and how it helps my specific
work. Then help me install whichever one I choose.
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
