# AI Research and Practice - Weeks 11-16 Syllabus

**Course:** DBAD-7098-01, AI Research and Practice<br>
**Term:** Spring 2026<br>
**Instructor:** Greg Lontok | gregory.lontok@lmu.edu | [LinkedIn](https://linkedin.com/in/lontok)<br>
**Co-Instructor (Weeks 1-10):** Martin Kang, Ph.D.<br>
**Zoom:** https://lmula.zoom.us/my/lontok

---

## Course goal

Set up an AI-enabled environment that helps you do your best work, whether that's at your day job or in your research.

By the end of this section, you will have built a personalized AI workflow connected to your real data sources and demonstrated it to the class.

## What this section covers

Weeks 1-10 with Prof. Kang covered AI concepts, strategy, ethics, and governance through readings and discussion. This section shifts to hands-on practice. You will:

- Set up and use AI tools (Claude Code, Granola, Wispr Flow, connectors)
- Learn prompting workflows, spec writing, and context engineering
- Connect AI to your own data sources (meetings, documents, APIs)
- Build a workflow tailored to your dissertation research or your day job
- Demo your workflow and its output on Demo Day

## The automation test

A simple framework: AI is not making you irrelevant. It's making clear what only you can do.

- **Easy parts automated = good outcome.** Excel freed accountants from tallying numbers so they could focus on real problem solving.
- **Hard parts automated = displacement.** GPS replaced the expertise London taxi drivers spent years building.

Your job is to figure out which bucket your tasks fall into, then build accordingly.

Based on [MIT Sloan research](https://mitsloan.mit.edu/ideas-made-to-matter/a-new-look-how-automation-changes-value-labor) analyzing 300+ occupations over nearly 40 years.

---

## Schedule

| Week | Date | Format | Time | Topic |
|------|------|--------|------|-------|
| 11 | Fri Mar 27 | Zoom | 11:00 AM - 12:00 PM | Introductions, tool demo, context engineering |
| 12 | Mar 30 - Apr 3 | Async (Easter) | - | Setup: Claude Code, Wispr Flow, Granola connector. Assignment: Workflow audit |
| 13 | Fri Apr 10 | In person | 5:30 PM - 9:00 PM | Hands-on workshop: prompting, specs, data connectors |
| 14 | Apr 13-17 | 1-on-1 meetings | TBD | Individual coaching on your workflow project |
| 15 | Apr 20-24 | 1-on-1 meetings | TBD | Individual coaching on your workflow project |
| 16 | Apr 27 - May 1 | 1-on-1 meetings | TBD | Individual coaching on your workflow project |
| Finals | Fri May 8 | Zoom | 9:00 AM - 10:30 AM | Demo Day: present your workflow and output |

---

## Week-by-week detail

### Week 11: Introductions and context engineering (Mar 27)

Meet each other. See AI tools in action. Understand context engineering.

**In class:**
- Student introductions: who you are, your dissertation focus, your day job, where you see AI fitting in
- Live demo: [Clay.com](https://clay.com) for AI-powered research prep, [Granola](https://granola.ai) + [Claude connector](https://claude.ai/customize/connectors) for pulling meeting data into AI without copy/paste
- Walk-through: how to enable the [Granola connector in your Claude account](https://claude.ai/customize/connectors)
- Discussion: in your field, what does AI automate, the hard parts or the easy parts?

**Before next week:** Complete the setup tasks and workflow audit assignment (details distributed in class).

### Week 12: Setup and workflow audit (Mar 30 - Apr 3, async)

Get your tools running. Let AI interview you about your work to map where it can help.

**Setup tasks:**
1. Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code/overview) (see Week 12 assignment for install commands)
2. Install [Wispr Flow](https://wisprflow.ai) (voice-to-text input)
3. Enable the [Granola connector in Claude](https://claude.ai/customize/connectors)

**Assignment: Workflow audit**
Paste the provided prompt into Claude Code. AI will interview you one question at a time about your day job, your research, and your current AI usage. Use Wispr Flow to speak your answers.

Claude will save a summary file that includes:
- Your tasks categorized into "easy parts" (automate) vs. "hard parts" (protect and invest in)
- Your top 5 AI opportunities with recommended tools
- A map of your data sources with available connectors
- A Granola self-assessment prompt you can use to coach yourself from your own meeting transcripts

**Submit:** `workflow-audit.md` on Brightspace by Tuesday, April 7.

### Week 13: Hands-on workshop (Apr 10, in person)

Build together. This is a working session, not a lecture.

**Bring:** Your laptop with Claude Code and Wispr Flow installed.

**Topics:**
- Prompting workflows and spec writing
- Connecting to data sources (APIs, MCP servers, connectors)
- Working with agents
- Begin building your personalized workflow

### Weeks 14-16: 1-on-1 coaching (Apr 13 - May 1)

Individual meetings structured like consulting sessions. I'll review your workflow audit, understand your specific challenges, and help you build something that works for your job or research. You'll demo your progress and get feedback directly in these sessions.

**Requirements:**
- Each meeting is one hour
- You must meet with me at least twice during the three-week window
- Schedule via [Calendly](https://calendly.com/greg-lontok/dba-ai-1-on-1)

**What to have ready:**
- Your workflow audit
- A clear idea of what data sources you want to connect to
- Questions or blockers you've hit while building

### Finals: Demo Day (May 8, Zoom)

**Friday, May 8 | 9:00-10:30 AM | Zoom:** https://lmula.zoom.us/my/lontok

Present your workflow and its output to the class. Each student gets 12 minutes: 8 minutes to demo, 4 minutes for Q&A.

**Presentation order (alphabetical by first name):**
1. Duane Rutkowski
2. Edgard Asensio
3. Eric Custis
4. Ershen Ali
5. Hania Ahmar
6. Matt Stefl
7. Tony Gonzales

**Two deliverables:**

1. **Markdown summary** submitted to Brightspace by 9:00 AM May 8 (start of class). Use this template:

   ```
   # Workflow name

   One-sentence summary.

   ## Problem
   What you're trying to do better at work or in your research.

   ## Inputs
   Data sources, connectors, tools.

   ## Steps
   What the workflow does, in order.

   ## Output
   What it produces.

   ## What's next
   What you'd improve with more time.
   ```

2. **Live demo (8 minutes).** Walk us through your workflow. Running it live is great if you can, but not required. At minimum, pull up your inputs, show the steps, and show the output. You don't have to actually execute a script or run a prompt if it's risky.

**What "the output" means:**

Whatever your workflow produces. Common examples by professional context:

- Account plan, exec briefing, pipeline review
- Deal memo, comp analysis, market brief
- Investment memo, due-diligence brief
- Vendor or P&L analysis, store-ops report
- Troubleshooting playbook, knowledge base article
- Clinical protocol, patient education doc
- Lit review, methodology section, coded interview themes, syllabus draft

Pick whatever fits your work. Name it in the markdown summary.

**Tech check before May 8:**
- Zoom screen-share works on the device you'll present from
- Output file is open in a tab and ready to show
- Connectors and tools you plan to demo are signed in
- Have a screenshot or recorded clip ready in case a live step fails

**What I'm grading:**
- Clarity of the workflow story (problem, inputs, steps, output)
- Fit to your real work
- Not polish, not slide design

---

## Tools

You will use the following tools throughout this section. All are required unless noted otherwise.

| Tool | Purpose | Cost |
|------|---------|------|
| Claude Pro | AI assistant for research, building, workflows | $20/month |
| Claude Code | Terminal-based AI agent for building and automation | Included with Claude Pro |
| Granola | AI meeting note-taker and transcription | Free (Business trial for connector) |
| Wispr Flow | Voice-to-text input for faster AI interaction | Free |

## Grading

This section accounts for 25% of your overall course grade. Prof. Kang's section (Weeks 1-10) accounts for the remaining 75%.

| Component | Weight | When |
|-----------|--------|------|
| Workflow audit + environment setup | 30% | Week 12 |
| Workflow project progress (shown in 1-on-1s) | 30% | Weeks 14-16 |
| Demo Day presentation | 40% | Finals |

## Contact

Email: gregory.lontok@lmu.edu
Teams: Greg Lontok
Office hours: [Schedule here](https://calendly.com/greg-lontok)
