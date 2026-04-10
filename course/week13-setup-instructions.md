# Week 13 setup instructions

## 1. Install VS Code

Download from: https://code.visualstudio.com/Download

- **Mac:** Download the .dmg for your chip. If you have an M1, M2, M3, or M4 Mac, pick "Apple Silicon." If you're not sure, pick "Universal." Open the .dmg and drag VS Code into your Applications folder.
- **Windows:** Download the "User Installer" for x64. Run the installer and accept the defaults.

Open VS Code once it's installed.

## 2. Open the terminal inside VS Code

- **Mac:** Press Cmd+` (the backtick key, above Tab)
- **Windows:** Press Ctrl+` (same key, above Tab)

A terminal panel should appear at the bottom of VS Code. This is where you'll run Claude Code.

## 3. Create your research folder

Type these commands into the terminal you just opened.

**Mac:**
```
mkdir ~/Documents/dba-ai-research
cd ~/Documents/dba-ai-research
```

**Windows (PowerShell):**
```
mkdir $HOME\Documents\dba-ai-research
cd $HOME\Documents\dba-ai-research
```

## 4. Copy your files in

Open Finder (Mac) or File Explorer (Windows) and copy your dissertation files into the `dba-ai-research` folder you just created. Grab anything relevant:

- Research papers and notes
- Data files (CSVs, spreadsheets, .dta files)
- Your workflow-audit.md from the Week 12 assignment
- Anything else related to your dissertation

**Copy, don't move.** Your originals stay where they are. This folder is a working copy.

Then open it in VS Code: go to File > Open Folder and navigate to your `dba-ai-research` folder.

## 5. Start Claude Code

In the VS Code terminal, type:

```
claude
```

Quick test: ask Claude Code "What files are in this folder?" It should list whatever you just copied in.

**If Claude Code doesn't start:**
- Run `claude --version` in the terminal. If it says "command not found," Claude Code isn't installed yet. Follow the install guide at https://docs.anthropic.com/en/docs/claude-code/overview
- If you see an auth prompt, sign in with your Claude Pro account.

## 6. Connect Granola (your first connector)

A connector bridges Claude to an external tool. This one connects Claude to your Granola meeting notes. Because we're setting it up at claude.ai, it works everywhere you use Claude — web chat, desktop app, and Claude Code.

1. Open https://claude.ai/customize/connectors in your browser
2. Find **Granola** and click to enable it
3. Sign in with your Granola account when prompted

Test it by going back to Claude Code and asking: "Summarize my most recent Granola meeting."

If it pulls up your meeting notes, you're connected. After the break, you'll add a second connector for your research.

**If Granola doesn't appear in the connector list:** Make sure you're signed into claude.ai with your Claude Pro account. Refresh the page and try again.
