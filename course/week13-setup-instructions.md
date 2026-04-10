# Week 13 setup instructions

## 1. Install VS Code

Download from: https://code.visualstudio.com/Download

- **Mac:** Download the .dmg for your chip. If you have an M1, M2, M3, or M4 Mac, pick "Apple Silicon." If you're not sure, pick "Universal." Open the .dmg and drag [VS Code](https://code.visualstudio.com) into your Applications folder.
- **Windows:** Download the "User Installer" for x64. Run the installer and accept the defaults.

Open VS Code once it's installed.

## 2. Open your research folder

You created an `ai-research-and-practice` folder during Week 12. Open it in VS Code: go to File > Open Folder and navigate to `Documents/ai-research-and-practice`.

If you don't have the folder yet, create it first:

- **Mac:** Open Finder, go to Documents, create a new folder called `ai-research-and-practice`
- **Windows:** Open File Explorer, go to Documents, create a new folder called `ai-research-and-practice`

Then open it in VS Code.

## 3. Make sure your files are in the folder

Check VS Code's sidebar on the left. You should see your files from Week 12 listed there.

**Your workflow audit is required.** Look for `workflow-audit.md` in the sidebar. Two of tonight's prompts reference it directly. If it's not there, download it from Brightspace and copy it in.

Also copy in anything else relevant to your research that isn't already there: papers, notes, data files (CSVs, spreadsheets, .dta files). **Copy, don't move.** Your originals stay where they are.

## 4. Open the terminal inside VS Code

Go to the menu bar: **Terminal > New Terminal**

A terminal panel should appear at the bottom of VS Code. This is where you'll run [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview).

## 5. Start Claude Code

In the terminal, type:

```
claude
```

Quick test: ask Claude Code "What files are in this folder?" It should list whatever you just copied in.

**If Claude Code doesn't start:**
- Run `claude --version` in the terminal. If it says "command not found," Claude Code isn't installed yet. Follow the install guide at https://docs.anthropic.com/en/docs/claude-code/overview
- If you see an auth prompt, sign in with your Claude Pro account.

## 6. Connect Granola (your first connector)

A connector lets Claude pull data from another tool. This one gives Claude access to your [Granola](https://granola.ai) meeting notes. Because we're setting it up at claude.ai, it works everywhere you use Claude, not just Claude Code.

1. Open https://claude.ai/customize/connectors in your browser
2. Find **Granola** and click to enable it
3. Sign in with your Granola account when prompted

Test it by going back to Claude Code and asking: "Summarize my most recent Granola meeting."

If it pulls up your meeting notes, you're connected. After the break, you'll add a second connector for your research.

## 7. Install Superpowers

Back in your Claude Code session, type:

```
/plugin install superpowers@claude-plugins-official
```

This changes how Claude Code works. Instead of jumping straight to code, it'll think through the problem first.

**If you get an error:** Try `/plugin update superpowers` instead.
