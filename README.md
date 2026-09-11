# OpenClaw handbook

72 entries · last verified 2026-09-09 · 72 links checked · 0 dead

One founder's handbook for running a company with an OpenClaw agent: the setup choices I made and why, the security rules I keep, the skills I install, the memory patterns that stuck, and the people worth learning from. It is not a directory of everything that exists - if something is here, it earned its place in real work. The longer notes live in [FIELD-NOTES.md](FIELD-NOTES.md). Suggest a link by opening an issue (see [CONTRIBUTING.md](CONTRIBUTING.md)).

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
- [Other useful lists](#other-useful-lists)
- [How this list is built](#how-this-list-is-built)
- [License](#license)

## Learn

Videos, threads and write-ups that taught me how OpenClaw actually behaves - start here if you have not installed it yet.

- [28 painful mistakes I made with OpenClaw so you don't have to (kloss on X)](https://x.com/kloss_xyz/status/2032011756890177552) - kloss's X article on 28 painful mistakes he made with OpenClaw in three weeks of importing other people's prompts, skills and memory systems into a working setup: words that trigger the wrong actions, agents that do everything, context lost in handoffs, rules set up in the wrong order, two agents on the same files, silent agents, five fixes at once, sessions that die with unsaved work, 'done'...
- [Build an entire OpenClaw agent in under a day (0xMarioNawfal on X, video)](https://x.com/roundtablespace/status/2044879754969387022) - repost of Julian Goldie's walkthrough of the build-your-own-openclaw tutorial repo: clone the lightweight agent repo, add an OpenRouter key, run the first chat loop locally, enable file and shell tools, then work through the 17 steps up to memory and concurrency control. No deep coding skills needed, the repo does the teaching.
- [build-your-own-openclaw](https://github.com/czl9707/build-your-own-openclaw) - The 17-step tutorial repo (MIT) the video walks through: from the first chat loop to tools, multi-layer prompts, agent dispatch, concurrency control and memory, so you understand what OpenClaw does under the hood (via @RoundtableSpace's post) · 1.9k stars · MIT · updated 2026-07
- [Claude Code as a personal OS - setup with Moritz Kremb (Peter Yang on LinkedIn)](https://www.linkedin.com/posts/petergyang_this-is-the-most-complete-setup-ive-seen-ugcPost-7459248459813064705-5eB4) - Peter Yang's video post with Moritz Kremb, captioned 'this is the most complete setup I've seen'. Filed under my OpenClaw learning material although the walkthrough is Claude Code as a personal OS.
- [clawchief](https://github.com/snarktank/clawchief) - Ryan Carson's executive-assistant layer for OpenClaw: skills, workspace files (HEARTBEAT.md, TOOLS.md, one canonical tasks.md), private context templates and cron jobs, installed on top of a working OpenClaw plus Google access (via @ryancarson's post) · 1.1k stars · updated 2026-04
- [From skeptic to true believer: How OpenClaw changed my life | Claire Vo](https://www.youtube.com/watch?v=DIa0MYJzM5I&t=1s) - Claire Vo is the host of our sister podcast, “How I AI,” a former product executive and engineer, and founder of an AI startup called ChatPRD.
- [Full Tutorial: Use OpenClaw to Build a Business That Runs Itself in 35 Min | Nat Eliason](https://www.youtube.com/watch?v=nSBKCZQkmYw) - Meet Felix: The OpenClaw bot building its own business.
- [How to set up Clawdbot for Google Ads and Meta Ads (get-ryze.ai)](https://www.get-ryze.ai/blog/clawdbot-google-meta-ads) - A practical guide for marketers who want an AI assistant managing their ad accounts: pull reports, analyze data and automate Google Ads and Meta Ads tasks over text messages. Clawdbot is OpenClaw's old name.
- [I fixed OpenClaw so it actually works (full setup)](https://www.youtube.com/watch?v=fd4k16REDOU) - I sit down with Moritz Kremb, an OpenClaw power user and agency builder based in Berlin, to break down how to actually make OpenClaw useful.
- [I rebuilt my entire life OS with OpenClaw (r/OpenClawUseCases)](https://www.reddit.com/r/OpenClawUseCases/comments/1rd9t8b/i_rebuilt_my_entire_life_os_with_openclaw_after) - Reddit write-up of the seven use cases from Matthew Berman's video on the 21 OpenClaw automations he runs daily: a self-updating personal CRM fed by Gmail and meeting transcripts, a nightly four-agent security council, an eight-expert business advisory council, a video idea research pipeline, a morning briefing to Telegram, cross-platform social stats and a food journal. The thread's own takeaway: scheduled skills plus Telegram notifications plus clean data pipelines, nothing magic.
- [OpenClaw optimized setup guide, the post-install checklist (Moritz Kremb on X)](https://x.com/moritzkremb/status/2029304864719667335) - Moritz Kremb's X article with the 30 to 60 minute hardening pass after a fresh install: personalise USER.md, IDENTITY.md and SOUL.md, make memory reliable with MEMORY.md plus daily files and a heartbeat rule that promotes learnings, set a primary model with fallbacks, move secrets out of the workspace and allowlist Telegram, add a Brave key and a managed browser profile, harden heartbeat and cron...
- [Setting up OpenClaw properly, not just install and chat (Corey Ganim on X)](https://x.com/coreyganim/status/2036103806975426779) - when I send this to all my friends and they finally understand how to perfectly set up OpenClaw not just "install and chat" a real workspace with memory, skills, and custom behavior.
- [The Claw native app studio (Ernesto Lopez on X)](https://x.com/ernestosoftware/status/2037187494530208029) - Ernesto Lopez's X article on his agentic app studio: have your OpenClaw agent validate the idea first by pulling the onboarding flows of the top three competitor apps on screensdesign.com and proposing a better one, build the app with Rork, then hand the agent every marketing angle from App Store screenshots to Apple Search Ads.
- [The ultimate guide to OpenClaw - 1 hour free masterclass (Greg Isenberg on X)](https://x.com/gregisenberg/status/2034778615464735000) - Greg Isenberg's thread: fix memory so it compounds (MEMORY.md plus daily logs, promote important learnings), then the rest of his one-hour masterclass.
- [Turn your OpenClaw into the world's best assistant (Ryan Carson on X)](https://x.com/ryancarson/status/2039786704731541903) - Ryan Carson's X article on running OpenClaw as a chief of staff: it schedules meetings, checks the inbox every 15 minutes and surfaces only what matters, chases unanswered emails, watches the calendar, keeps one canonical markdown task list and preps the day before he wakes up.

## Install and first week

The choices the installer asks you to make (model, channel, search, skills, package manager, hooks, Control UI) and how to survive the first week without breaking anything. My reasoning for each choice is in the notes.

- [If you installed OpenClaw this week, read this (r/clawdbot)](https://www.reddit.com/r/clawdbot/comments/1s270n0/if_you_installed_openclaw_this_week_read_this) - ShabzSparq's checklist after fixing 50+ OpenClaw setups, in order: switch the default model off Opus to Sonnet before the bill surprises you, bind the gateway to 127.0.0.1 and reach it over an SSH tunnel, read BOOTSTRAP.md and write a six-line SOUL.md before the first real task, and install no skills in week one because some loop silently and burn tokens. 559 upvotes, 64 comments.
- [OpenClaw setup guide: build your personal AI agent (Claire Vo, Lenny's Newsletter)](https://www.lennysnewsletter.com/p/openclaw-the-complete-guide-to-building) - I built a team of 9 AI agents that run my work and life. Here's how you can too.

### Channel choice

- [Telegram channel setup (OpenClaw docs)](https://docs.openclaw.ai/channels/telegram) - Telegram bot support status, capabilities, and configuration.

### Browser choice

- [Brave Search API](https://brave.com/search/api) - Enterprise-grade Web search API accessing an index of 40+ billion pages. Specialized endpoints to train models, power search, and more. Real-time indexing, low latencies, and flexible pricing.
- [Web search tools (OpenClaw docs)](https://docs.openclaw.ai/tools/web) - web_search, x_search, and web_fetch -- search the web, search X posts, or fetch page content.

My notes on this section: [Install and first week](FIELD-NOTES.md#install-and-first-week) (50 notes).

## Memory and context

How the agent remembers between sessions: the learnings-folder pattern, lossless context, memory plugins and what I still fight with.

- [Cognee](https://github.com/topoteretes/cognee) - Open-source memory platform that builds a knowledge graph from your agent's data, with an official OpenClaw integration in its docs (via @KSimback's post) · 30k stars · Apache-2.0 · updated 2026-09
- [Give your OpenClaw the memory it needs, full guide (Kevin Simback on X)](https://x.com/ksimback/status/2024180197910864182) - Kevin Simback's X article on why OpenClaw forgets: memory is never saved (the model decides what is worth writing), saved but never searched, or destroyed by context compaction mid-session.
- [Hindsight](https://github.com/vectorize-io/hindsight) - agent memory that learns - Hindsight: Agent Memory That Learns. · 23k stars · MIT · updated 2026-09
- [LCM](https://github.com/martian-engineering/lossless-claw) - Lossless Context Management (open-source plugin designed by Martian Engineering) to replace the default, lossy conversation-compaction system. · 4.9k stars · MIT · updated 2026-08
- [Mem0](https://github.com/mem0ai/mem0) - Drop-in memory layer for agents, the option Kevin reaches for when config-only memory is not enough; it has an OpenClaw write-up on its blog (via @KSimback's post) · 64k stars · Apache-2.0 · updated 2026-09
- [QMD](https://github.com/tobi/qmd) - Tobi Lutke's mini CLI search engine for notes and docs; local search over MEMORY.md and the daily files so the agent finds what it already wrote (via @KSimback's post) · 29k stars · MIT · updated 2026-08
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
- [Local heartbeat and 9 more OpenClaw lessons (Divyanshi Sharma on Instagram)](https://www.instagram.com/p/DVJPnoGkvnd?img_index=1) - Divyanshi Sharma's 18-slide carousel, ten things she wishes she knew before running OpenClaw: the agent makes 48 heartbeat calls a day by default, so route heartbeats to a local model (Ollama with llama3.2:1b) and keep the paid API for real work, stop model-hopping across free tiers and set automatic fallback models, install only trusted skills from ClawHub after reading SKILL.md, fight context...
- [Ollama](https://github.com/ollama/ollama) - Run llama3.2:1b or any small model locally so the OpenClaw heartbeat costs nothing and works offline, and keep the paid API for the real work (via @divyannshisharma's post) · 180k stars · MIT · updated 2026-09

### GPT 5.4

- [GPT 5.4 in OpenClaw: the settings to change (r/openclaw)](https://www.reddit.com/r/openclaw/comments/1sgpg8b/a_lot_of_the_new_gpt_54_sucks_in_openclaw_posts) - r/openclaw thread arguing that most 'GPT 5.4 sucks in OpenClaw' complaints are setup problems: update to at least OpenClaw 2026.4.5, turn reasoning on with thinking at medium or higher, use the openai-responses path, enable block streaming when the bot lives in Telegram, and keep enough recent context. The author still finds GPT 5.4 needs tighter steering than Opus 4.6, and prefers it that way.

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

- [arscontexta](https://github.com/agenticnotetaking/arscontexta) - Heinrich's Claude Code plugin from the Skill Graphs article: a 250-file skill graph that sets up a markdown knowledge system and fills it with /learn and /reduce, the worked example of the pattern (via @arscontexta's post) · 3.5k stars · MIT · updated 2026-02
- [Before you do anything with OpenClaw, install Kickstart (jordy on X)](https://x.com/jordymaui/status/2027067341280891204) - jordy's X article: before you chat with a fresh OpenClaw agent, run npx clawhub install kickstart and say 'run kickstart setup'. The free skill installs SOUL.md, USER.md and MEMORY.md templates, an anchor.md of non-negotiable rules that survives context compaction, model defaults that put heartbeats on Haiku instead of Opus, and a context bundle protocol so sub-agents get a real brief. The article explains each problem it solves.
- [find-skills (ClawHub)](https://clawhub.ai/JimLiuxinghai/skills/find-skills) - Auto-discovers and installs skills on demand.
- [Kickstart (ClawHub)](https://clawhub.ai/jordymaui/skills/kickstart) - The skill from jordy's article: one install that sets up memory files, personality, rules, cost-saving model defaults and automation scaffolding on a fresh OpenClaw (via @jordymaui's post)
- [Skill graphs beat one SKILL.md (Heinrich, @arscontexta on X)](https://x.com/arscontexta/status/2023957499183829467) - Heinrich's X article arguing that one SKILL.md file cannot hold real depth, so build a skill graph instead: many small markdown files with YAML descriptions the agent can scan, wikilinks written into prose so it follows the relevant paths, and maps of content that group clusters.

### Token Efficiency

- [qmd-skill](https://github.com/levineam/qmd-skill) - Token-efficiency skill; my note says it cuts token usage by 95%. The repository has no description of its own. · 696 stars · updated 2026-02

### Memory

- [openclaw-supermemory](https://github.com/supermemoryai/openclaw-supermemory) - Unlimited memory for the agent - long-term memory and recall for your OpenClaw agent through Supermemory. · 799 stars · updated 2026-09

### Security

- [dont-hack-me (ClawHub)](https://clawhub.ai/peterokase42/skills/dont-hack-me) - Security self-check: a quick audit of your config to catch dangerous misconfigurations such as an exposed gateway.
- [prompt-guard (ClawHub)](https://clawhub.ai/seojoonkim/skills/prompt-guard) - Advanced prompt injection defense - 650+ patterns covering prompt injection, supply chain injection, memory poisoning and more.

### Research

- [Last30days](https://github.com/mvanhorn/last30days-skill) - useful for content/marketing, researches topics across Reddit, X, YouTube, HN, and Polymarket from the last 30 days, then synthesizes findings and can generate copy-paste prompts. · 61k stars · MIT · updated 2026-09

### Image & Video generation

- [Larry (ClawHub)](https://clawhub.ai/OllieWazza/larry) - The free skill from Ollie Warren's article: one-shots the TikTok slideshow system his agent Larry runs daily, from hook formulas to the RevenueCat revenue loop (via @oliverhenry's post)
- [Larry (LarryBrain)](https://www.larrybrain.com) - Ollie Warren's TikTok slideshow skill for OpenClaw: his agent Larry took his apps to 8M views in a week, and the X article walks through the skill files, the hook formulas and the RevenueCat revenue loop. LarryBrain is the product site, LarryLoop the standalone app, and the ClawHub skill has its own entry. · also: [larryloop.com](https://www.larryloop.com) · also: [x.com](https://x.com/oliverhenry/status/2023776478446436696)

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

- [Design Director Agent](https://x.com/kloss_xyz/status/2023142088850944283) - kloss's system prompt that replaces a design agency with OpenClaw: a Design Director agent that inherits Claude Code's frontend-design skill, extracts 30 to 50 scored references from designer accounts and sites you like, turns them into tokens and principles, spawns eight sub-agents (visual identity, UI and UX, design systems, motion, creative direction, layout and typography, design research,...
- [frontend-design skill (anthropics/skills)](https://github.com/anthropics/skills/tree/main/skills/frontend-design) - Anthropic's frontend-design skill is the floor the Design Director prompt inherits from: design thinking, typography, motion and anti-slop rules, with your extracted design DNA layered on top (via @kloss_xyz's post) · 175k stars · updated 2026-09
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
- [self-improving-agent](https://github.com/pskoett/self-improving-agent) - The skill Corey's post is about: logs every error, correction and feature request to files in its learnings folder (.learnings/ERRORS.md, LEARNINGS.md and FEATURE_REQUESTS.md) so the agent stops repeating mistakes; 478k installs on ClawHub (via @coreyganim's post) · 748 stars · updated 2026-08

## Other useful lists

This list is deliberately short and opinionated. When you want the exhaustive version, these are the ones I actually open:

- [alvinreal/awesome-openclaw](https://github.com/alvinreal/awesome-openclaw) - the reference directory for the OpenClaw ecosystem: official projects, dashboards, deployment tooling, memory systems, alternative clients, plugins and channel integrations. Several hundred entries against the seventy or so here, so start there when you are looking for a category rather than a recommendation.
- [alvinreal/awesome-openclaw-tips](https://github.com/alvinreal/awesome-openclaw-tips) - thirty numbered tips on messages, Telegram, memory, reliability, cost, operations, automation and architecture, each with the failure it prevents and a prompt you can paste. The closest thing to this repo's field notes written by someone else, and it covers ground mine does not.
- [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) - 5,400+ skills filtered and categorised from the official registry. Use it as the index when you know the job you want done and need to find out whether a skill already exists.

The difference is intent, not quality: those are directories of what exists, this is a record of what I kept after using it. If a link appears in both, theirs will be more complete and mine will tell you whether it survived contact with real work.

## How this list is built

The source is a private Notion page where I keep notes while I work. A sync script in my workspace (`awesome-sync.py`, not in this repo) reads that page through the Notion API and keeps only the sections that are explicitly mapped as public - everything else stays private by default. It canonicalizes every URL (https only, tracking parameters dropped, `youtu.be` and `twitter.com` rewritten), drops links to private places (Notion, Google Drive, course platforms, local addresses), scans every string for secrets and private names, and writes three files: `data/links.csv` (one row per link), `data/notes.json` (the field notes) and `data/_report.md` (what was excluded and why).

From there everything is automated and reproducible from this repo alone:

- `tools/enrich.py` checks every link and writes `data/enrichment.json`: stars, license, last push and archive state from the GitHub API (renamed repositories are followed), titles from YouTube and X oEmbed, and a plain HTTP check with a browser user agent for everything else.
- `tools/build.py` renders this README and `FIELD-NOTES.md` from `data/` + `config/sections.json` + `templates/`. Links stay here, every note goes to the notes file, grouped by the same sections. Entries are sorted by name inside each section; the build is deterministic, so running it twice produces the same files.
- `tools/lint.py` fails on dead links, descriptions under 30 characters, duplicate names or URLs, non-https links, tracking parameters, links to private hosts, long dashes, placeholders, thin sections and broken table-of-contents anchors - in both files. Whatever it cannot fix on its own is listed under "Open decisions" in `data/_report.md`.
- A weekly GitHub Action (`.github/workflows/links.yml`) re-runs the checks and opens a pull request when either file changes. `data/_dead.md` lists what needs a human look.

Nothing in this README or in `FIELD-NOTES.md` is edited by hand. Fixes go to `data/overrides.json` (keyed by the entry id in `data/links.csv`, or by block id under `_notes` for a note) and the next build picks them up.

Current build: 72 entries in 12 sections, 157 field notes. Links checked: 72, dead: 0, last check: 2026-09-09. What the sync excluded and why is in `data/_report.md`. The field notes are rendered into `FIELD-NOTES.md` by the same build.

## License

The content of this list (README, FIELD-NOTES and the files in `data/`) is licensed under [CC BY 4.0](LICENSE) - share and adapt it with attribution. The scripts in `tools/` are MIT licensed ([LICENSE-CODE](LICENSE-CODE)).
