# OpenClaw for founders

56 entries · last verified 2026-09-09 · 56 links checked · 0 dead

One founder's working list of what actually helps when you run a company with an OpenClaw agent: the setup choices I made and why, the security rules I keep, the skills I install, the memory patterns that stuck, and the people worth learning from. It is not a directory of everything that exists - if something is here, it earned its place in real work. The longer notes live in [FIELD-NOTES.md](FIELD-NOTES.md). Suggest a link by opening an issue (see [CONTRIBUTING.md](CONTRIBUTING.md)).

Descriptions are my own notes where I wrote one. Where I only saved a link, the description is the repository's or the post's own summary. Ratings like `(Matt: 8/10)` are my personal scores.

## Contents

- [Learn](#learn)
- [Install and first week](#install-and-first-week)
  - [Channel choice](#channel-choice)
  - [Browser choice](#browser-choice)
- [Memory and context](#memory-and-context)
- [Security](#security)
- [Models and token burn](#models-and-token-burn)
  - [GPT 5.4](#gpt-54)
  - [GPT 5.5](#gpt-55)
  - [Token providers](#token-providers)
- [Tools stack](#tools-stack)
- [Skills](#skills)
  - [General](#general)
  - [Token Efficiency](#token-efficiency)
  - [Memory](#memory)
  - [Security](#security-1)
  - [Research](#research)
  - [Image & Video generation](#image--video-generation)
  - [Marketing, Ads & SEO](#marketing-ads--seo)
  - [Skill platforms](#skill-platforms)
- [Multi-agent and hierarchy](#multi-agent-and-hierarchy)
- [Prompts and collections](#prompts-and-collections)
  - [Prompts](#prompts)
  - [Collections](#collections)
  - [Business ideas and inspiration](#business-ideas-and-inspiration)
- [Operations](#operations)
  - [Own dashboard](#own-dashboard)
  - [Local Mac vs VPS](#local-mac-vs-vps)
  - [Finances](#finances)
- [Use cases](#use-cases)
- [Field notes](#field-notes)
  - [General](#general-1)
  - [Self-improving](#self-improving)
- [How this list is built](#how-this-list-is-built)
- [License](#license)

## Learn

Videos, threads and write-ups that taught me how OpenClaw actually behaves - start here if you have not installed it yet.

- [Claude Code as a personal OS - setup with Moritz Kremb (Peter Yang on LinkedIn)](https://www.linkedin.com/posts/petergyang_this-is-the-most-complete-setup-ive-seen-ugcPost-7459248459813064705-5eB4) - Peter Yang's video post with Moritz Kremb, captioned 'this is the most complete setup I've seen'. Filed under my OpenClaw learning material although the walkthrough is Claude Code as a personal OS.
- [From skeptic to true believer: How OpenClaw changed my life | Claire Vo](https://www.youtube.com/watch?v=DIa0MYJzM5I&t=1s) - Claire Vo is the host of our sister podcast, “How I AI,” a former product executive and engineer, and founder of an AI startup called ChatPRD.
- [Full Tutorial: Use OpenClaw to Build a Business That Runs Itself in 35 Min | Nat Eliason](https://www.youtube.com/watch?v=nSBKCZQkmYw) - Meet Felix: The OpenClaw bot building its own business.
- [How to build an entire OpenClaw agent in less than one day (0xMarioNawfal on X)](https://x.com/roundtablespace/status/2044879754969387022) - Thread embedded under my Learning toggle: here's how to build an entire OpenClaw agent in less than one day.
- [How to set up Clawdbot for Google Ads and Meta Ads (get-ryze.ai)](https://www.get-ryze.ai/blog/clawdbot-google-meta-ads) - A practical guide for marketers who want an AI assistant managing their ad accounts: pull reports, analyze data and automate Google Ads and Meta Ads tasks over text messages. Clawdbot is OpenClaw's old name.
- [I fixed OpenClaw so it actually works (full setup)](https://www.youtube.com/watch?v=fd4k16REDOU) - I sit down with Moritz Kremb, an OpenClaw power user and agency builder based in Berlin, to break down how to actually make OpenClaw useful.
- [I rebuilt my entire life OS with OpenClaw (r/OpenClawUseCases)](https://www.reddit.com/r/OpenClawUseCases/comments/1rd9t8b/i_rebuilt_my_entire_life_os_with_openclaw_after) - Reddit thread by someone who rebuilt their whole personal 'life OS' on OpenClaw - the first link under my best-practices notes.
- [OpenClaw install checklist (Moritz Kremb on X)](https://x.com/moritzkremb/status/2029304864719667335) - Moritz Kremb's install checklist, posted on X - the post itself is just a link. The same Moritz as in the 'I fixed OpenClaw so it actually works' video.
- [Setting up OpenClaw properly, not just install and chat (Corey Ganim on X)](https://x.com/coreyganim/status/2036103806975426779) - when I send this to all my friends and they finally understand how to perfectly set up OpenClaw not just "install and chat" a real workspace with memory, skills, and custom behavior.
- [The ultimate guide to OpenClaw - 1 hour free masterclass (Greg Isenberg on X)](https://x.com/gregisenberg/status/2034778615464735000) - Greg Isenberg's thread: fix memory so it compounds (MEMORY.md plus daily logs, promote important learnings), then the rest of his one-hour masterclass.

## Install and first week

The choices the installer asks you to make (model, channel, search, skills, package manager, hooks, Control UI) and how to survive the first week without breaking anything. My reasoning for each choice is in the notes.

- [If you installed OpenClaw this week, read this (r/clawdbot)](https://www.reddit.com/r/clawdbot/comments/1s270n0/if_you_installed_openclaw_this_week_read_this) - Reddit thread addressed to people who installed OpenClaw this week - the bookmark sits next to my first-week notes.
- [OpenClaw setup guide: build your personal AI agent (Claire Vo, Lenny's Newsletter)](https://www.lennysnewsletter.com/p/openclaw-the-complete-guide-to-building) - I built a team of 9 AI agents that run my work and life. Here's how you can too.

### Channel choice

- [Telegram channel setup (OpenClaw docs)](https://docs.openclaw.ai/channels/telegram) - Telegram bot support status, capabilities, and configuration.

### Browser choice

- [Brave Search API](https://brave.com/search/api) - Enterprise-grade Web search API accessing an index of 40+ billion pages. Specialized endpoints to train models, power search, and more. Real-time indexing, low latencies, and flexible pricing.
- [Web search tools (OpenClaw docs)](https://docs.openclaw.ai/tools/web) - web_search, x_search, and web_fetch -- search the web, search X posts, or fetch page content.

My notes on this section: [Install and first week](FIELD-NOTES.md#install-and-first-week) (50 notes).

## Memory and context

How the agent remembers between sessions: the learnings-folder pattern, lossless context, memory plugins and what I still fight with.

- [Hindsight](https://github.com/vectorize-io/hindsight) - agent memory that learns - Hindsight: Agent Memory That Learns. · 23k stars · MIT · updated 2026-09
- [LCM](https://github.com/martian-engineering/lossless-claw) - Lossless Context Management (open-source plugin designed by Martian Engineering) to replace the default, lossy conversation-compaction system. · 4.9k stars · MIT · updated 2026-08
- [Supermemory](https://supermemory.ai) - Agents need memory. Supermemory is building the default engine for memory and continual learning for agents.

My notes on this section: [Memory and context](FIELD-NOTES.md#memory-and-context) (12 notes).

## Security

An agent with your credentials on a machine that is on all day. The exposure check first, then sandboxing, approvals and the managed alternatives.

- [Moltworker (Cloudflare)](https://github.com/cloudflare/moltworker) - Alternative to your own security setup: use DigitalOcean's managed deployment or Cloudflare's Moltworker - it handles the hard parts automatically. · 10k stars · Apache-2.0 · updated 2026-05 · also: [digitalocean.com](https://www.digitalocean.com/community/tutorials/how-to-run-openclaw)
- [NemoClaw (NVIDIA)](https://www.nvidia.com/en-us/ai/nemoclaw) - Policy-based privacy & local open model deployment.
- [NVIDIA GTC keynote 2026 (from 44:07)](https://www.youtube.com/watch?v=jw_o0xr8MWU&t=2647s) - Jensen Huang's GTC 2026 keynote, linked at 44:07 under my NemoClaw notes.
- [Security (OpenClaw docs)](https://docs.openclaw.ai/gateway/security) - The official security page: trust model, safe defaults and hardening guidance for running OpenClaw.

My notes on this section: [Security](FIELD-NOTES.md#security) (13 notes).

## Models and token burn

Which model runs what, how to switch, and how to stop the bill from growing: routers, token providers and the numbers I wrote down.

- [ClawRouter](https://github.com/BlockRunAI/ClawRouter) - Smart LLM routing to optimize token burn, if simple question = routing to cheap model, complex code - escalates to Opus or Sonnet. · 6.6k stars · MIT · updated 2026-09
- [Local heartbeat with a local model (Instagram post)](https://www.instagram.com/p/DVJPnoGkvnd?img_index=1) - Run the heartbeat locally with a local model - an Instagram post I saved under token burn; the platform shows crawlers nothing, my note on it is in the field notes.

### GPT 5.4

- [GPT 5.4 in OpenClaw: the settings to change (r/openclaw)](https://www.reddit.com/r/openclaw/comments/1sgpg8b/a_lot_of_the_new_gpt_54_sucks_in_openclaw_posts) - The r/openclaw thread behind the wave of 'GPT 5.4 sucks in OpenClaw' posts - when you switch, change the settings it lists.

### GPT 5.5

- [GPT 5.5: how to switch (Tak on X)](https://x.com/cherry_mx_reds/status/2047390468778901738) - if you're on latest openclaw just type: /models add openai-codex gpt-5.5 🦞🥔 if you're running into permissions issues running this then there are two ways to solve it. 👇 Do it yourself: send /whoami.

### Token providers

- [The Claw Bay](https://theclawbay.com) - Opus and Codex through one reseller key? (my open question) - their own pitch: one API key for GPT-6, Codex, Claude and Gemini access with low-latency EU and US routing.

My notes on this section: [Models and token burn](FIELD-NOTES.md#models-and-token-burn) (16 notes).

## Tools stack

What I connect the agent to and how far I let it go with each tool - Google, GitHub, web search, Linear, Obsidian, Manus.

My notes on this section: [Tools stack](FIELD-NOTES.md#tools-stack) (11 notes).

## Skills

The skills I install or keep an eye on, grouped by what they are for. Star counts and licenses come from GitHub and are refreshed weekly.

### General

- [find-skills (ClawHub)](https://clawhub.ai/JimLiuxinghai/skills/find-skills) - Auto-discovers and installs skills on demand.
- [Kickstart](https://x.com/jordymaui/status/2027067341280891204) - Skill that will implement the core things - an X post by @jordymaui (the post itself is a link).

### Token Efficiency

- [qmd-skill](https://github.com/levineam/qmd-skill) - Token-efficiency skill; my note says it cuts token usage by 95%. The repository has no description of its own. · 696 stars · updated 2026-02

### Memory

- [openclaw-supermemory](https://github.com/supermemoryai/openclaw-supermemory) - Unlimited memory for the agent - long-term memory and recall for your OpenClaw agent through Supermemory. · 799 stars · updated 2026-06

### Security

- [dont-hack-me (ClawHub)](https://clawhub.ai/peterokase42/skills/dont-hack-me) - Security self-check: a quick audit of your config to catch dangerous misconfigurations such as an exposed gateway.
- [prompt-guard (ClawHub)](https://clawhub.ai/seojoonkim/skills/prompt-guard) - Advanced prompt injection defense - 650+ patterns covering prompt injection, supply chain injection, memory poisoning and more.

### Research

- [Last30days](https://github.com/mvanhorn/last30days-skill) - useful for content/marketing, researches topics across Reddit, X, YouTube, HN, and Polymarket from the last 30 days, then synthesizes findings and can generate copy-paste prompts. · 61k stars · MIT · updated 2026-09

### Image & Video generation

- [Larry (LarryBrain)](https://www.larrybrain.com) - TikTok video-making skill on LarryBrain, now also a standalone app on LarryLoop - the X post is the announcement. · also: [larryloop.com](https://www.larryloop.com) · also: [x.com](https://x.com/oliverhenry/status/2023776478446436696)

### Marketing, Ads & SEO

- [7 OpenClaw skills for paid media (get-ryze.ai)](https://www.get-ryze.ai/blog/openclaw-google-meta-ads-guide) - Seven free OpenClaw skills that audit, report, and optimize your Google Ads and Meta Ads accounts.

### Skill platforms

- [ClawHub](https://clawhub.ai/skills?sort=downloads) - ClawHub - a fast skill registry for agents, with vector search.

## Multi-agent and hierarchy

Spawning more agents, giving each a narrow identity, and checking they really exist. The example roster that goes around (Polly the personal assistant, Finn the family manager and friends) is Claire Vo's, from her OpenClaw guide on Lenny's Newsletter listed under Install and first week - only my own notes are kept here.

- [Sub-agents (OpenClaw docs)](https://docs.openclaw.ai/tools/subagents) - The official page on sub-agents: spawn isolated background agent runs that announce results back to the requester chat.

My notes on this section: [Multi-agent and hierarchy](FIELD-NOTES.md#multi-agent-and-hierarchy) (9 notes).

## Prompts and collections

Prompt packs worth stealing from, the awesome-lists I go back to, and a few places that got me thinking about what an agent could earn.

### Prompts

- [Design Director Agent](https://x.com/kloss_xyz/status/2023142088850944283) - Full Design Agency Replacement (by @kloss_xyz)
- [Mission Control Dashboard](https://x.com/kloss_xyz/status/2022461932759060993) - JARVIS-style AI command center, plus the Jarvis initialization sequence: 8 prompts to configure your OpenClaw agent (both in the same post by @kloss_xyz).
- [OpenClaw implementation prompts (Matthew Berman's gist)](https://gist.github.com/mberman84/065631c62d6d8f30ecb14748c00fc6d9) - Each prompt is a self-contained brief you can hand to an AI coding assistant, or use as a project spec, to build that use case from scratch - it starts with a personal CRM.

### Collections

- [Awesome Openclaw](https://github.com/alvinreal/awesome-openclaw) - A curated list of the best OpenClaw resources: official projects, skills, plugins, dashboards, deployment tooling, memory systems, and guides. · 733 stars · CC0-1.0 · updated 2026-07
- [Awesome openclaw skills](https://github.com/VoltAgent/awesome-openclaw-skills) - The awesome collection of OpenClaw skills. 5,400+ skills filtered and categorized from the official OpenClaw Skills Registry.🦞. · 52k stars · MIT · updated 2026-09
- [Awesome Openclaw Tips](https://github.com/alvinreal/awesome-openclaw-tips#mem-01-make-your-agent-learn-from-its-mistakes) - Practical OpenClaw tips for memory, reliability, cost, automation, and multi-agent workflows. · 229 stars · updated 2026-05

### Business ideas and inspiration

- [Agent Side Hustle School](https://agentsidehustleschool.com) - A 28-day program that teaches your AI agent to earn enough to cover its own API costs. Real experiments, specific offers. Free to use until April 30.

## Operations

Running the thing day to day: where it lives (Mac mini or VPS), how I talk to it, the cron jobs, the terminal commands I keep forgetting, and money.

### Own dashboard

- [CLAW3D](https://www.claw3d.ai) - An open-source 3D virtual office for AI agents. Watch your AI workforce review code, run standups, and collaborate in real-time.

### Local Mac vs VPS

- [OpenClaw on a Hostinger VPS](https://www.hostinger.com/applications/openclaw) - The VPS route: KVM2 plan with Ubuntu 24.04 LTS, get in over SSH as root and install from there. Hostinger's page has a one-click Docker template; the video tutorial is linked as well. · also: [youtube.com](https://www.youtube.com/watch?v=BhjK2Gr0Ryc)
- [OpenClaw on Amazon EC2 - the cheapest and easiest setup (video)](https://www.youtube.com/watch?v=04wh2Hlgbds) - Ubuntu on a c7iflex.large instance with 30 GB - the video tutorial for the EC2 route ('ClawdBot is a 24/7 AI agent employee... here's how to set it up cheap and easy').

### Finances

- [Link for agents (Stripe)](https://link.com/en-cz/agents) - Wallet for agents by Stripe: let your agent pay online with one-time-use cards or machine payment protocols, and you approve every request. The tweet that announced it is linked too. · also: [x.com](https://x.com/_maxblade/status/2049604418354438487)

My notes on this section: [Operations](FIELD-NOTES.md#operations) (10 notes).

## Use cases

Public write-ups of what people actually run. My own use-case pages stay private, so this section is short on purpose.

- [awesome-openclaw-usecases](https://github.com/hesamsheikh/awesome-openclaw-usecases) - A community collection of OpenClaw use cases for making life easier. · 31k stars · MIT · updated 2026-03 · also: [x.com](https://x.com/meta_alchemist/status/2028606379486044290)
- [Morning brief (video chapter, from 9:32)](https://www.youtube.com/watch?v=04wh2Hlgbds&t=572) - The morning-brief chapter of the EC2 setup video, starting at 9:32 - saved as a use case.

## Field notes

Working rules I keep in Notion and refine as OpenClaw changes - the anatomy of the workspace files, what not to do, SOUL.md, self-improvement, skill design.

Everything I wrote down, grouped by section, lives in [FIELD-NOTES.md](FIELD-NOTES.md):

- [Install and first week](FIELD-NOTES.md#install-and-first-week) - 50 notes
- [Memory and context](FIELD-NOTES.md#memory-and-context) - 12 notes
- [Security](FIELD-NOTES.md#security) - 13 notes
- [Models and token burn](FIELD-NOTES.md#models-and-token-burn) - 16 notes
- [Tools stack](FIELD-NOTES.md#tools-stack) - 11 notes
- [Multi-agent and hierarchy](FIELD-NOTES.md#multi-agent-and-hierarchy) - 9 notes
- [Operations](FIELD-NOTES.md#operations) - 10 notes
- [Field notes](FIELD-NOTES.md#field-notes) - 36 notes

### General

- [Back up agent workspace](https://docs.openclaw.ai/concepts/agent-workspace) - Agent workspace: location, layout, and backup strategy.
- [Context7](https://context7.com) - Set up a help project with the OpenClaw documentation from Context7 so the agent reads current docs instead of guessing.
- [Environment variables (OpenClaw docs)](https://docs.openclaw.ai/help/environment) - Where to store API keys and secrets: give OpenClaw access to environment variables by putting them in .openclaw/.env.
- [Health check help](https://docs.openclaw.ai/gateway/health) - Health check commands and gateway health monitoring.

### Self-improving

- [Self-Improving Agent skill (Corey Ganim on X)](https://x.com/coreyganim/status/2035757428579389768) - How to make your OpenClaw agent learn from its mistakes: Install the Self-Improving Agent skill.

## How this list is built

The source is a private Notion page where I keep notes while I work. A sync script in my workspace (`awesome-sync.py`, not in this repo) reads that page through the Notion API and keeps only the sections that are explicitly mapped as public - everything else stays private by default. It canonicalizes every URL (https only, tracking parameters dropped, `youtu.be` and `twitter.com` rewritten), drops links to private places (Notion, Google Drive, course platforms, local addresses), scans every string for secrets and private names, and writes three files: `data/links.csv` (one row per link), `data/notes.json` (the field notes) and `data/_report.md` (what was excluded and why).

From there everything is automated and reproducible from this repo alone:

- `tools/enrich.py` checks every link and writes `data/enrichment.json`: stars, license, last push and archive state from the GitHub API (renamed repositories are followed), titles from YouTube and X oEmbed, and a plain HTTP check with a browser user agent for everything else.
- `tools/build.py` renders this README and `FIELD-NOTES.md` from `data/` + `config/sections.json` + `templates/`. Links stay here, every note goes to the notes file, grouped by the same sections. Entries are sorted by name inside each section; the build is deterministic, so running it twice produces the same files.
- `tools/lint.py` fails on dead links, descriptions under 30 characters, duplicate names or URLs, non-https links, tracking parameters, links to private hosts, long dashes, placeholders, thin sections and broken table-of-contents anchors - in both files. Whatever it cannot fix on its own is listed under "Open decisions" in `data/_report.md`.
- A weekly GitHub Action (`.github/workflows/links.yml`) re-runs the checks and opens a pull request when either file changes. `data/_dead.md` lists what needs a human look.

Nothing in this README or in `FIELD-NOTES.md` is edited by hand. Fixes go to `data/overrides.json` (keyed by the entry id in `data/links.csv`, or by block id under `_notes` for a note) and the next build picks them up.

Current build: 56 entries in 12 sections, 157 field notes. Links checked: 56, dead: 0, last check: 2026-09-09. What the sync excluded and why is in `data/_report.md`. The field notes are rendered into `FIELD-NOTES.md` by the same build.

## License

The content of this list (README, FIELD-NOTES and the files in `data/`) is licensed under [CC BY 4.0](LICENSE) - share and adapt it with attribution. The scripts in `tools/` are MIT licensed ([LICENSE-CODE](LICENSE-CODE)).
