# Week 13 session prompts

## Prompt 1: organize your research context

**When:** After the break, once setup is done.

**What to expect:** Claude Code reads every file in your folder, figures out what each one is, and creates a README that indexes everything. It may rename files or move things into subfolders. Watch VS Code's file explorer sidebar on the left. You'll see it update in real time.

**Paste this into Claude Code:**

```text
Scan all the files in this folder. Before making changes, tell me what you found and what you plan
to do. Then create a README.md that indexes each file and how it relates to my research. Rename
unclear files and organize into subfolders if it makes sense.
```

## Prompt 2: find connectors for your work

**When:** After Prompt 1.

**What to expect:** Claude Code reads your workflow audit from the Week 12 assignment and recommends connectors that match your bottlenecks. You pick one and enable it at claude.ai/customize/connectors — same way you set up Granola.

**How to use it:** Type the `@` symbol in Claude Code followed by the path to your workflow audit file. The `@` tells Claude Code to read that specific file as context. Start typing `@workflow` and it should autocomplete the path for you — handy if the file moved during Prompt 1.

**Type this into Claude Code (adjust the path to match where your file is):**

```text
@workflow-audit.md Based on my bottlenecks and data sources, recommend connectors I can enable at
claude.ai/customize/connectors. For each one, explain what it connects to and how it helps my
specific work. Then walk me through setting up whichever one I choose.
```

If Claude Code reorganized your files during Prompt 1, your audit may be in a subfolder. Type `@` and start typing `workflow` — Claude Code will show you matching files wherever they are.

## Prompt 3: work on your #1 bottleneck

**When:** Build time starts. You'll use this for the rest of the session.

**What to expect:** Claude Code reads your workflow audit, finds your biggest bottleneck, and asks you questions before proposing anything. Use Wispr Flow to speak your answers. You'll say more than you'd type.

**Type this into Claude Code (same `@` reference as Prompt 2):**

```text
@workflow-audit.md Identify my #1 bottleneck. Ask me one question at a time until you understand
the problem well enough to help. When you have enough context, tell me your thinking and propose
an approach. We'll agree on a plan before you build anything.
```
