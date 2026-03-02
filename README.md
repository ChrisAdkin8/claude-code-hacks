# Awesome Claude Code Hacks

> A curated list of productivity hacks, CLAUDE.md recipes, MCP server recommendations,
> prompt techniques, custom skills, and workflow patterns for [Claude Code](https://www.anthropic.com/claude-code).
>
> Maintained by the [`claude-hacks`](https://github.com/ChrisAdkin8/newsletter-ai-skill) skill · Contributions welcome via PR

---

## Contents

- [Setup & Configuration](#setup--configuration)
- [CLAUDE.md Recipes](#claudemd-recipes)
- [Prompt Techniques](#prompt-techniques)
- [MCP Servers & Tools](#mcp-servers--tools)
- [Custom Skills & Commands](#custom-skills--commands)
- [Agentic Workflows](#agentic-workflows)
- [IDE & Editor](#ide--editor)
- [CI/CD & Automation](#cicd--automation)
- [Video Tutorials](#video-tutorials)

---

## Setup & Configuration

Tips for initial setup, model selection, global config, and `.claude/` directory structure.

<!-- claude-hacks: setup-config -->

- [Claude Code Best Practices (Anthropic Official)](https://code.claude.com/docs/en/best-practices) — Anthropic's own guide covering project setup, CLAUDE.md configuration, model selection, and the recommended workflow loop.
- [Boris Cherny's Claude Code Setup](https://www.threads.com/@boris_cherny/post/DTBVlMIkpcm/im-boris-and-i-created-claude-code-lots-of-people-have-asked-how-i-use-claude) — The creator of Claude Code shows his surprisingly vanilla setup: Opus with thinking for everything, parallel terminal sessions, and minimal customisation.
- [45 Claude Code Tips (ykdojo)](https://github.com/ykdojo/claude-code-tips) — Comprehensive tip collection from basics to advanced including a custom status line script, cutting the system prompt in half, and using Gemini CLI as Claude Code's minion.
- [Claude Code Everything You Need to Know](https://github.com/wesammustafa/Claude-Code-Everything-You-Need-to-Know) — All-in-one guide covering setup, prompt engineering, commands, hooks, workflows, automation, MCP servers, and the BMAD method.

---

## CLAUDE.md Recipes

Specific CLAUDE.md patterns, instruction templates, and memory configurations that improve Claude Code's behaviour on your projects.

<!-- claude-hacks: claude-md -->

- [Claude Code Best Practice CLAUDE.md Template](https://github.com/shanraisshan/claude-code-best-practice) — A battle-tested CLAUDE.md template with architecture, code standards, key files, and build commands structured as onboarding docs for Claude.
- [CLAUDE.md Templates Collection](https://github.com/ruvnet/ruflo/wiki/CLAUDE-MD-Templates) — Multiple CLAUDE.md templates for different project types with auto-generation via a /custom-init command.
- [35 Claude Code Tips From Boris Cherny](https://www.anup.io/35-claude-code-tips-from-the-guy-who-built-it/) — Distilled tips from the creator including: update CLAUDE.md after every correction, keep it under 150 lines, and use @.claude on PR reviews to add learnings.
- [Claude Code Best Practices Site](https://rosmur.github.io/claudecode-best-practices/) — Structured guide to CLAUDE.md patterns, treating it like code: review when things go wrong, prune regularly, and observe whether Claude's behaviour shifts.

---

## Prompt Techniques

Prompting strategies, request phrasing patterns, and conversation management techniques that get better results from Claude Code.

<!-- claude-hacks: prompt-techniques -->

- [Common Workflows (Anthropic Official)](https://code.claude.com/docs/en/common-workflows) — Anthropic's official guide to effective prompting patterns including explore-plan-code-commit, using /clear between tasks, and @-mentioning files with line ranges.
- [10 Real Productivity Workflows for 2026](https://www.f22labs.com/blogs/10-claude-code-productivity-tips-for-every-developer/) — Ten concrete workflows including writing detailed specs before coding, using plan mode iteratively, and the two-step /create-plan pattern.
- [The Ultimate Guide to Claude Code Prompts](https://medium.com/@tonimaxx/the-ultimate-guide-to-claude-code-production-prompts-power-tricks-and-workflow-recipes-42af90ca3b4a) — Production prompts, power tricks, and workflow recipes including context priming and structured request patterns.

---

## MCP Servers & Tools

Model Context Protocol servers and tools that extend Claude Code's built-in capabilities.

<!-- claude-hacks: mcp-servers -->

- [Connect Claude Code to Tools via MCP (Official Docs)](https://code.claude.com/docs/en/mcp) — Anthropic's official MCP setup guide covering scoped configs (.mcp.json), environment variable expansion, and the stdio vs HTTP transport tradeoffs.
- [50+ Best MCP Servers for Claude Code](https://claudefa.st/blog/tools/mcp-extensions/best-addons) — Curated list of production-ready MCP servers organised by category: filesystem, database (PostgreSQL, SQLite), browser (Playwright), GitHub, and more.
- [Docker MCP Toolkit for Claude Code](https://www.docker.com/blog/add-mcp-servers-to-claude-code-with-mcp-toolkit/) — Run MCP servers in Docker containers for isolation and reproducibility, with one-command setup for common servers.
- [22 Best MCP Servers (Desktop Commander)](https://desktopcommander.app/blog/2025/11/25/best-mcp-servers/) — Ranked list including GitHub, Filesystem, Desktop Commander, Notion, Supabase, and Brave Search with installation guides.

---

## Custom Skills & Commands

Custom slash commands, SKILL.md files, and repeatable workflow patterns you can install into Claude Code.

<!-- claude-hacks: custom-skills -->

- [Claude Skills Are Awesome (Simon Willison)](https://simonwillison.net/2025/Oct/16/claude-skills/) — Willison argues Claude Skills may be a bigger deal than MCP — folders with instructions, scripts, and resources that Claude loads on demand for repeatable workflows.
- [Awesome Claude Code](https://github.com/hesreallyhim/awesome-claude-code) — Curated list of skills, hooks, slash-commands, agent orchestrators, and plugins for Claude Code with more components than just CLAUDE.md files.
- [Claude Code Showcase](https://github.com/ChrisWiles/claude-code-showcase) — Comprehensive example project demonstrating hooks, skills, agents, commands, and GitHub Actions workflows in a single reference repo.
- [Build a YouTube Research Agent with Slash Commands](https://creatoreconomy.so/p/claude-code-tutorial-build-a-youtube-research-agent-in-15-min) — Step-by-step tutorial building a custom research agent as a Claude Code slash command in 15 minutes.

---

## Agentic Workflows

Multi-step autonomous workflows, subagent patterns, plan mode strategies, and orchestration techniques.

<!-- claude-hacks: agentic-workflows -->

- [Parallel Coding Agent Lifestyle (Simon Willison)](https://simonwillison.net/2025/Oct/5/parallel-coding-agents/) — Willison's guide to running 3–5 Claude Code sessions in parallel across git worktrees, each tackling independent tasks simultaneously.
- [Boris Cherny's Team Workflow Tips](https://www.threads.com/@boris_cherny/post/DUMZr4VElyb/im-boris-and-i-created-claude-code-i-wanted-to-quickly-share-a-few-tips-for) — Tips from the Claude Code team: start in plan mode, iterate until the plan is right, then switch to auto-accept edits mode for execution.
- [Solving Agent Context Loss with Beads](https://news.ycombinator.com/item?id=46471286) — HN discussion on using Beads to handle context as state in Claude Code sessions, preventing information loss across long agentic workflows.
- [Agent-Rules for Claude Code](https://news.ycombinator.com/item?id=47177580) — Show HN: opinionated rules and workflow configurations for Claude Code agentic sessions with pre-built verification patterns.

---

## IDE & Editor

VS Code, Cursor, JetBrains, and other editor integrations, keyboard shortcuts, and settings.

<!-- claude-hacks: ide-editor -->

- [Use Claude Code in VS Code (Official Docs)](https://code.claude.com/docs/en/vs-code) — Official setup guide: Cmd+Esc to summon, in-IDE diff view, @-mention files with line ranges, multiple conversation tabs, and auto-accept edits mode.
- [Claude Code IDE Integration Guide](https://www.vibesparking.com/en/blog/ai/claude-code/ide/2025-08-24-claude-code-ide-integration-vscode-cursor-jetbrains/) — Covers VS Code, Cursor, and JetBrains setup with tips like running /config → diff tool auto, using /ide from external terminals, and fixing the JetBrains ESC key conflict.
- [How I Use Every Claude Code Feature (Simon Willison)](https://simonwillison.net/2025/Nov/2/how-i-use-every-claude-code-feature/) — Comprehensive walkthrough of every Claude Code feature from terminal basics to IDE integration, with practical examples for each.

---

## CI/CD & Automation

Running Claude Code in GitHub Actions, scheduled automation, headless usage with `claude -p`, and non-interactive patterns.

<!-- claude-hacks: cicd -->

- [Claude Code GitHub Actions (Official)](https://code.claude.com/docs/en/github-actions) — Anthropic's official guide to the claude-code-action for automated PR reviews, issue triage, code changes from @claude mentions, and scheduled automation.
- [anthropics/claude-code-action](https://github.com/anthropics/claude-code-action) — Official GitHub Action for running Claude Code in CI: answers questions, implements code changes, and detects when to activate based on workflow context.
- [Claude Code Scheduled Automation Guide](https://smartscope.blog/en/generative-ai/claude/claude-code-scheduled-automation-guide/) — Complete guide to scheduled Claude Code execution via GitHub Actions including secret management, error handling, and the -p flag for headless mode.
- [Headless Mode and CI/CD Cheatsheet](https://institute.sfeir.com/en/claude-code/claude-code-headless-mode-and-ci-cd/cheatsheet/) — Quick reference for claude -p (single prompt), programmatic multi-turn sessions, and common CI/CD patterns.

---

## Video Tutorials

Walkthroughs, demos, and screencasts covering Claude Code features and workflows.

<!-- claude-hacks: video-tutorials -->

- [Best Claude Code YouTube Videos Ranked (2026)](https://medium.com/@rentierdigital/i-watched-25-claude-code-youtube-videos-so-you-dont-have-to-the-definitive-ranking-550aa6863840) — Watched and ranked 25 Claude Code videos from Boris Cherny's official walkthroughs to deep-dive tutorials, sorted by usefulness.
- [24 Claude Code Tips: Advent Calendar (Dev.to)](https://dev.to/oikon/24-claude-code-tips-claudecodeadventcalendar-52b5) — Daily Claude Code tips from December 2025 covering setup, workflows, slash commands, and advanced patterns — one for each day.
- [Claude Code Transcript Extractor (Simon Willison)](https://simonwillison.net/2025/dec/25/claude-code-transcripts/) — Python CLI tool to convert Claude Code transcripts to detailed HTML pages for reviewing and sharing agentic session logs.

---

*Curated by [claude-hacks](https://github.com/ChrisAdkin8/newsletter-ai-skill) · Last updated: 2026-03-02*
