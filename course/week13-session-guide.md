# Week 13 session guide - build your research command center

Friday, April 10, 2026 | 5:30-9:00 PM | Hilton 304

By the end of tonight, your research files will be organized, Claude will have access to your data, and you'll have a working start on your biggest bottleneck.

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

### 1. Install VS Code

Download from: https://code.visualstudio.com/Download

- **Mac:** Download the .dmg for your chip. If you have an M1, M2, M3, or M4 Mac, pick "Apple Silicon." If you're not sure, pick "Universal." Open the .dmg and drag [VS Code](https://code.visualstudio.com) into your Applications folder.
- **Windows:** Download the "User Installer" for x64. Run the installer and accept the defaults.

Open VS Code once it's installed.

### 2. Open your research folder

You created an `ai-research-and-practice` folder during Week 12. Open it in VS Code: go to File > Open Folder and navigate to `Documents/ai-research-and-practice`.

If you don't have the folder yet, create it first:

- **Mac:** Open Finder, go to Documents, create a new folder called `ai-research-and-practice`
- **Windows:** Open File Explorer, go to Documents, create a new folder called `ai-research-and-practice`

Then open it in VS Code.

### 3. Make sure your files are in the folder

Check VS Code's sidebar on the left. You should see your files from Week 12 listed there.

**Your [workflow audit](https://github.com/LMU-DBA/ai-research-and-practice/blob/main/course/week12-workflow-audit.md) is required.** Look for `workflow-audit.md` in the sidebar. Two of tonight's prompts reference it directly. If it's not there, download it from Brightspace and get it into the folder. Two easy ways:

- Drag the file straight into VS Code's sidebar. It'll copy it in.
- Or open the folder in Finder (Mac) or File Explorer (Windows) and drop it there. VS Code's sidebar is just showing you what's in that folder on your computer.

Now gather everything related to your current research and copy it into this folder. Claude Code can only work with files it can see, so the more context you give it, the better it can help. Look through your Google Drive, Dropbox, OneDrive, desktop, Downloads folder, email attachments, wherever your stuff lives. Grab your research papers, literature reviews, data files (CSVs, spreadsheets, .dta, .sav files), drafts, notes, outlines, anything. If it's related to your dissertation, put a copy here.

**Copy, don't move.** Your originals stay where they are. This folder is a working copy.

### 4. Open the terminal inside VS Code

Go to the menu bar: **Terminal > New Terminal**

A terminal panel should appear at the bottom of VS Code. This is where you'll run [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview).

### 5. Start Claude Code

In the terminal, type:

```
claude
```

Quick test: ask Claude Code "What files are in this folder?" It should list whatever you just copied in.

### 6. Set [output style](https://code.claude.com/docs/en/output-styles) to explanatory

Type `/config` in Claude Code, select output style, and choose "explanatory." This tells Claude Code to explain its thinking as it works, not just show you the result. You'll learn more this way.

### 7. Connect Granola (your first connector)

A connector lets Claude pull data from another tool. This one gives Claude access to your [Granola](https://granola.ai) meeting notes. Because we're setting it up at [claude.ai](https://claude.ai) (the web chat), it works everywhere you use Claude, not just Claude Code.

1. Open https://claude.ai/customize/connectors in your browser
2. Find **Granola** and click to enable it
3. Sign in with your Granola account when prompted

Test it by going back to Claude Code and asking: "Summarize my most recent Granola meeting."

If it pulls up your meeting notes, you're connected. After the break, you'll add a second connector for your research.

### 8. Install Superpowers

Back in your Claude Code session, type:

```
/plugin install superpowers@claude-plugins-official
```

[Superpowers](https://github.com/obra/superpowers) changes how Claude Code works. Instead of jumping straight to code, it'll think through the problem first.

---

## Session prompts

### Prompt 1: organize your research context

**When:** After the break, once setup is done.

**What to expect:** Claude Code reads every file in your folder, figures out what each one is, and creates a README that indexes everything. It may rename files or move things into subfolders. Watch VS Code's file explorer sidebar on the left. You'll see it update in real time.

**Paste this into Claude Code:**

```text
Scan all the files in this folder. Before making changes, tell me what you found and what you plan
to do. Then create a README.md that indexes each file and how it relates to my research. Rename
unclear files and organize into subfolders if it makes sense.
```

### Prompt 2: find connectors for your work

**When:** After Prompt 1.

**What to expect:** Claude Code reads your workflow audit from the Week 12 assignment and recommends connectors that can help with your dissertation research. You pick one and enable it at claude.ai/customize/connectors — same way you set up Granola.

**How to use it:** Type the `@` symbol in Claude Code followed by the path to your workflow audit file. The `@` tells Claude Code to read that specific file as context. Start typing `@workflow` and it should autocomplete the path for you — handy if the file moved during Prompt 1.

**Type this into Claude Code (adjust the path to match where your file is):**

```text
@workflow-audit.md Focus on my dissertation research. Recommend connectors I can enable at
claude.ai/customize/connectors that would help with my research. For each one, explain what it
connects to and how it helps. Then walk me through setting up whichever one I choose.
```

If Claude Code reorganized your files during Prompt 1, your audit may be in a subfolder. Type `@` and start typing `workflow` — Claude Code will show you matching files wherever they are.

### Prompt 3: work on your biggest dissertation bottleneck

**When:** Build time starts. You'll use this for the rest of the session.

**What to expect:** Claude Code reads your workflow audit, finds the biggest bottleneck in your dissertation research, and asks you questions before proposing anything. Even if your day job has bigger pain points, tonight we're focused on moving your research forward. Use Wispr Flow to speak your answers. You'll say more than you'd type.

**Type this into Claude Code (same `@` reference as Prompt 2):**

```text
@workflow-audit.md Focus on my dissertation research. Identify my biggest bottleneck related to my
research or dissertation. Ask me one question at a time until you understand the problem well
enough to help. When you have enough context, tell me your thinking and propose an approach.
We'll agree on a plan before you build anything.
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

1. **Sync your research folder to cloud backup.** Your `ai-research-and-practice` folder needs to be synced to Google Drive, Dropbox, iCloud, Box, or OneDrive. Greg will ask for proof — a screenshot or live demo. If you need help setting this up, reach out.

2. **Keep Granola running in your meetings.** You need 1-2 weeks of meeting transcripts for the self-assessment prompt to work well. Just leave it running.

---

## What's next

### 1-on-1 coaching meetings (Weeks 14-16, Apr 13 - May 1)

Individual meetings where we go deep on your specific bottleneck. Come prepared with your workflow audit, your research folder, and any questions or blockers.

You must meet with Greg at least twice during the three-week window.

**Schedule here:** https://calendly.com/greg-lontok/dba-ai-1-on-1

**What to have ready:**
- `ai-research-and-practice` folder synced to cloud backup (bring proof)
- Your workflow audit reviewed
- Superpowers installed (if you didn't finish tonight, we'll do it together)
- Questions or blockers you've hit

### Demo Day (Finals week)

**Friday, May 8 | 9:00-10:30 AM | Zoom:** https://lmula.zoom.us/my/lontok

Present your workflow and its output to the class. Live demo, show what you built, Q&A.
