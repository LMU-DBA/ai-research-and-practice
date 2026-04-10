# Week 13 session prompts

## Prompt 1: organize your research context

**When:** After you've copied your files into the research folder and Claude Code is running (around 6:35).

**What to expect:** Claude Code will read every file in your folder, figure out what each one is, and create a README that indexes everything. It may rename files with unclear names or move things into subfolders. Watch VS Code's file explorer sidebar on the left — you'll see it update in real time.

**Paste this into Claude Code:**

```text
Scan all the files in this folder. Create a README.md that indexes everything: what each file is, what it contains, and how it relates to my research. Rename any files that have unclear names. Organize into subfolders if it makes sense. Explain what you're doing as you go.
```

## Prompt 2: find MCP plugins for your work

**When:** After the break (around 7:05).

**What to expect:** Claude Code will read your workflow audit from the Week 12 assignment and recommend MCP servers (data source connectors) that match your specific bottlenecks. You'll pick one and install it — your second MCP connection of the night.

**Paste this into Claude Code:**

```text
Read my workflow-audit.md file. Based on my bottlenecks and data sources, recommend MCP servers or Claude Code plugins that would help me. For each recommendation, explain what it connects to and how it would help my specific work. Then help me install whichever one I choose.
```

## Prompt 3: work on your #1 bottleneck

**When:** Build time starts (around 7:25). You'll use this for the next hour.

**What to expect:** Claude Code will read your workflow audit, identify your biggest bottleneck, and ask you questions to understand the problem before proposing a solution. Use Wispr Flow to speak your answers — you'll give better detail by talking than typing.

**How to use it:** Type the `@` symbol in Claude Code followed by the path to your workflow audit file. The `@` tells Claude Code to read that specific file as context. Start typing `@workflow` and it should autocomplete the path for you — handy if the file moved during Prompt 1.

**Type this into Claude Code (adjust the path to match where your file is):**

```text
@workflow-audit.md Identify my #1 bottleneck — the thing that takes the most time or is blocking my progress. Ask me questions until you understand the problem well enough to help. When you feel you have enough context, tell me your thinking. We'll plan together first, then implement based on complexity.
```

If Claude Code reorganized your files during Prompt 1, your audit may be in a subfolder. Type `@` and start typing `workflow` — Claude Code will show you matching files wherever they are.
