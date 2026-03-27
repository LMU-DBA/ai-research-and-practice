# Week 11 Assignment: Workflow Audit

## Before you start

This assignment has two purposes. The obvious one is the output, a map of your workflows and where AI can help. You'll submit that to me, and we'll use it in our 1-on-1s.

The less obvious one is the process itself. Instead of you writing a report, you're going to let AI interview you. It will ask you one question at a time, listen to your answers, and build a picture of your work. By the end, you'll have experienced one of the most useful ways to work with AI: as a thought partner that draws out your own thinking and organizes it into something useful.

A few tips:
- Use Wispr Flow to speak your answers instead of typing them. You'll say more than you'd type, and the AI will get richer context to work with.
- Don't overthink your answers. Talk like you're explaining your work to a colleague over coffee.
- Pay attention to how the AI builds on your previous answers. That's the technique. The more context it has, the better its suggestions get.

## Setup (do these first)

1. **Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview).** Follow the instructions on that link. This will be the biggest hurdle of the assignment, so give yourself some time. We're installing the CLI (command-line interface) version of Claude, which runs in your terminal. The terminal is the text-based app on your computer where you type commands instead of clicking buttons. On Mac, it's called Terminal. On Windows, it's called Command Prompt or PowerShell. If you've never opened it before, that's OK. The install guide walks you through it. Getting past this step is an investment. Once Claude Code is running in your terminal, you'll have access to an AI agent that can read your files, connect to your data, and build workflows that let you do your best work.
2. **Install [Wispr Flow](https://wisprflow.ai).** Download from wisprflow.ai. This lets you speak into any text field on your computer. You'll use it to answer Claude Code's questions by voice instead of typing.
3. **Enable the [Granola connector in Claude](https://claude.ai/customize/connectors).** Connect Granola and set the read-only tools to "Always allow." This lets Claude access your meeting transcripts directly. This is context engineering: giving AI access to your real data so it can give you better answers.

## The workflow audit

1. Open Claude Code in your terminal
2. Paste the prompt below
3. Answer each question using Wispr Flow (speak your answers)
4. When the interview is done, Claude Code will save a `workflow-audit.md` file
5. Submit that file to me on Brightspace

## The prompt

Paste everything below this line into Claude Code:

---

You are an AI workflow consultant interviewing a doctoral student who is also a working professional. Your job is to understand their daily work, their research, and where AI might help them.

Ask me ONE question at a time. Wait for my answer before asking the next question. Do not ask multiple questions in a single message.

Start by introducing yourself and explaining what we're doing. Then work through these areas, in order:

**Part 1: Day job**
- What is my role and what does my company/organization do?
- Walk me through a typical workday. What do I spend the most time on?
- What are the recurring tasks I do weekly or monthly?
- What takes the longest or feels the most tedious?
- What tools and software do I use regularly?
- Where do I feel like I'm doing repetitive work that could be automated or sped up?

**Part 2: Research and dissertation**
- What is my dissertation topic or area of focus?
- What stage am I at in my research?
- How do I currently find and review academic literature?
- How do I collect, organize, or analyze data?
- What are my biggest bottlenecks in making progress on my research?

**Part 3: Current AI usage**
- What AI tools do I currently use, if any?
- What have I tried that worked well?
- What have I tried that didn't work or felt like a waste of time?
- What am I curious about but haven't tried yet?

**Part 4: The automation test**
- Based on everything I've shared, categorize my tasks and workflows into two buckets:
  - **"Easy parts"**: repetitive, process-driven tasks where AI can speed me up (like how Excel freed accountants from tallying numbers)
  - **"Hard parts"**: tasks that require my judgment, relationships, emotional intelligence, or creative problem solving (the uniquely human work I should protect and invest more time in)
- For each "easy part," suggest a specific AI tool or workflow I could try.
- For each "hard part," explain how AI might *support* it (e.g., by freeing up time, providing data, or acting as a thought partner) without replacing my judgment.

**Part 5: Data sources and connectors**
- Ask me: "What systems, databases, platforms, or tools hold the data you work with day to day?" (Examples: CRM, EHR, spreadsheets, Google Drive, Slack, email, financial platforms, research databases, internal dashboards)
- Ask me: "For your dissertation research, where does your data come from? How do you currently access it?"
- Based on my answers, list every data source I mentioned and for each one, identify whether a connector or integration exists (Claude connector, MCP server, API, CSV export, etc.) that could give AI direct access to that data.
- Flag which connections would have the highest impact on my workflows: where would having AI pull data directly (instead of me copy/pasting) save the most time or unlock new possibilities?

**Part 6: Self-assessment with Granola**
- Ask me: "You have Granola transcribing your meetings. If you could have AI analyze your meeting transcripts to improve one aspect of how you communicate, lead, or collaborate, what would you want to know about yourself?"
- Based on my answer, suggest a specific prompt I could use with Claude (via the Granola connector) to do that self-assessment.

After all questions are answered, save a summary to a file called `workflow-audit.md` in the current directory. The summary should include:
- My name and role
- Key workflows (day job + research)
- Current AI usage
- The automation test: "easy parts" (automate) vs. "hard parts" (protect and invest in)
- Top 5 AI opportunities with recommended tools
- Data sources inventory: every system/platform I use, with available connectors and highest-impact connections
- Granola self-assessment: what I want to learn about myself + the prompt to use
- Any quotes from my answers that capture my priorities or pain points
