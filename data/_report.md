# awesome-sync report

Source page: `2fddaecfce6b8068a1abeff8c06a7db7` - generated 2026-09-09. Block ids are Notion block ids (open the page and append `#<id without dashes>` to jump).

## Counts

- entries: 61
  - Field notes / General: 4
  - Field notes / Self-improving: 1
  - Install and first week: 2
  - Install and first week / Browser choice: 2
  - Install and first week / Channel choice: 1
  - Learn: 13
  - Memory and context: 4
  - Models and token burn: 2
  - Models and token burn / GPT 5.4: 1
  - Models and token burn / GPT 5.5: 1
  - Models and token burn / Token providers: 1
  - Multi-agent and hierarchy: 1
  - Operations / Finances: 1
  - Operations / Local Mac vs VPS: 2
  - Operations / Own dashboard: 1
  - Prompts and collections / Business ideas and inspiration: 1
  - Prompts and collections / Collections: 3
  - Prompts and collections / Prompts: 3
  - Security: 4
  - Skills / General: 3
  - Skills / Image & Video generation: 1
  - Skills / Marketing, Ads & SEO: 1
  - Skills / Memory: 1
  - Skills / Research: 1
  - Skills / Security: 2
  - Skills / Skill platforms: 1
  - Skills / Token Efficiency: 1
  - Use cases: 2
- notes: 187
- media/file blocks skipped: 11

## Mapped toggles

- `Manual summary 👨🏻 (heading)` -> links -> Learn
- `Learning` -> links -> Learn
- `General` -> links+notes -> Field notes / General
- `General > DON'T: auto-update without checking the changelog` -> links+notes -> Field notes / Don'ts
- `General > Tools.md` -> links+notes -> Field notes / General
- `General > Anatomy` -> links+notes -> Field notes / Anatomy of the workspace files
- `Install Guide` -> links+notes -> Install and first week
- `Install Guide > Model choice` -> links+notes -> Install and first week / Model choice
- `Install Guide > Channel choice` -> links+notes -> Install and first week / Channel choice
- `Install Guide > Browser choice` -> links+notes -> Install and first week / Browser choice
- `Install Guide > Skill choice` -> links+notes -> Install and first week / Skill choice
- `Install Guide > Skill mode manager` -> links+notes -> Install and first week / Skill package manager
- `Install Guide > Hooks choice (turn on all 4)` -> links+notes -> Install and first week / Hooks choice
- `Install Guide > Control UI` -> links+notes -> Install and first week / Control UI
- `Install Guide > Uninstall Openclaw` -> links+notes -> Install and first week / Uninstall
- `Initial setup` -> links+notes -> Install and first week
- `Initial setup > 1st week` -> links+notes -> Install and first week / First week
- `Initial setup > After week 1` -> links+notes -> Install and first week / After week 1
- `Memory & Context` -> links+notes -> Memory and context
- `Memory & Context > Make agent learn from its mistakes` -> links+notes -> Memory and context / Make the agent learn from its mistakes
- `Security (OpenClaw Docs)` -> links+notes -> Security
- `Security (OpenClaw Docs) > Nemoclaw (Link, Discord Nemo channel)` -> links+notes -> Security
- `Models & Token burn` -> links+notes -> Models and token burn
- `Models & Token burn > GPT 5.4` -> links+notes -> Models and token burn / GPT 5.4
- `Models & Token burn > GPT 5.5` -> links+notes -> Models and token burn / GPT 5.5
- `Tools Stack` -> links+notes -> Tools stack
- `Self-improving` -> links+notes -> Field notes / Self-improving
- `SOUL.MD` -> notes -> Field notes / SOUL.md
- `Gamification` -> notes -> Field notes / Gamification
- `Data feeding / Context` -> private -> 
- `Own dashboard` -> links+notes -> Operations / Own dashboard
- `Local Mac vs VPS` -> links+notes -> Operations / Local Mac vs VPS
- `Prompts` -> links -> Prompts and collections / Prompts
- `Communication` -> notes -> Operations / Communication
- `Cron jobs` -> notes -> Operations / Cron jobs
- `Skills` -> links -> Skills
- `Skills > General` -> links -> Skills / General
- `Skills > Token Efficiency` -> links -> Skills / Token Efficiency
- `Skills > Memory` -> links -> Skills / Memory
- `Skills > Security` -> links -> Skills / Security
- `Skills > Development` -> links -> Skills / Development
- `Skills > Webdesign` -> links -> Skills / Webdesign
- `Skills > Research` -> links -> Skills / Research
- `Skills > Image & Video generation` -> links -> Skills / Image & Video generation
- `Skills > Marketing, Ads & SEO` -> links -> Skills / Marketing, Ads & SEO
- `Skills > GTM & Sales` -> links -> Skills / GTM & Sales
- `Skills > Collections` -> private -> 
- `Skills > Skill platforms` -> links -> Skills / Skill platforms
- `Hierarchy & subagents (OpenClaw Doc)` -> links+notes -> Multi-agent and hierarchy
- `Detection - browsing, proxies etc.` -> private -> 
- `Speciliazed OpenClaw agents` -> private -> 
- `Business ideas & inspo` -> links -> Prompts and collections / Business ideas and inspiration
- `Token providers` -> links -> Models and token burn / Token providers
- `Mission Control Roadmap` -> private -> 
- `Terminal Commands` -> notes -> Operations / Terminal commands
- `Collections` -> links -> Prompts and collections / Collections
- `Finances` -> links -> Operations / Finances
- `Use cases` -> links -> Use cases
- `Skill Design Best Practices (heading)` -> notes -> Field notes / Skill design best practices
- `🎨 Design Director Agent - Full Design Agency Repla (heading)` -> links+notes -> Field notes / Design Director agent
- `💰 Token Optimization (heading)` -> private -> 
- `Key Insights (heading)` -> notes -> Models and token burn / Token optimization key insights
- `ClawRouter - Agent-Native LLM Router (⭐ 4/5 Recomm (heading)` -> links+notes -> Models and token burn / ClawRouter
- `📝 Other (heading)` -> private -> 

## Mapping decisions recorded in the config

- `Manual summary` -> links: Plain heading (not a toggle): the loose link paragraphs under it (Reddit, X posts, get-ryze guide) are links; its text-only paragraphs are ignored in links mode.
- `General > Tools.md` -> links+notes: Explicit for transparency - same as inherited.
- `Install Guide > Browser choice` -> links+notes: Brave vs Exa vs Tavily vs SearXNG comparison - the agent name inside it is rewritten by text_replacements.
- `Install Guide > Skill mode manager` -> links+notes: bun vs pnpm vs npm; the host name inside it is rewritten by text_replacements.
- `Install Guide > Control UI` -> links+notes: Token-handling note is publishable (it explains where the token lives, it does not contain one); the loopback dashboard URL is excluded by the local-address rule.
- `Security (OpenClaw Docs) > Nemoclaw (Link, Discord Nemo channel)` -> links+notes: Explicit for transparency - same as inherited. Its Discord channel link is dropped via exclude_urls (needs server membership).
- `Token providers` -> links: Judgment call from the brief: the reseller's own public page is kept, the r/DiscountPremiumAcc thread is dropped via exclude_urls.
- `Key Insights` -> notes: Plain heading under 'Token Optimization'; the child page and database next to it stay private by rule.
- `ClawRouter - Agent-Native LLM Router` -> links+notes: Plain heading: the write-up becomes notes; its 'Source | Git backup' paragraph is forced private (links a private [redacted] repo) - the ClawRouter entry itself comes from the Models & Token burn toggle.
- `Tools Stack` -> links+notes: Holds no links today (sub-toggles per tool with one bullet each); links+notes so a link added later is picked up.
- `Data feeding / Context` -> private: Czech working notes about Matt's own data feeding - private per the brief.
- `Local Mac vs VPS` -> links+notes: The Hostinger Google Doc with Matt's VPS commands is excluded by the google-docs rule; the public Hostinger page and the YouTube tutorials stay.
- `Skills` -> links: Root toggle only holds sub-toggles; each one is mapped below. Anything added later inherits 'links' - list it here first.
- `Skills > Development` -> links: Holds only a TBD placeholder today - publishes automatically once a link is added.
- `Skills > Webdesign` -> links: Its only bullet links a Notion page (excluded by rule) - empty until a public link is added.
- `Skills > GTM & Sales` -> links: Holds only a TBD placeholder today.
- `Skills > Collections` -> private: Its one link (awesome-openclaw-skills) is also in the top-level Collections toggle; kept private so the entry lands under Prompts and collections / Collections instead of Skills.
- `Hierarchy & subagents (OpenClaw Doc)` -> links+notes: Matt's own bullets are published; the numbered example roster of agent personas (copied from Claire Vo's guide on Lenny's Newsletter) is forced private via private_block_ids and replaced by a pointer in the section blurb.
- `Detection - browsing, proxies etc.` -> private: TBD only.
- `Speciliazed OpenClaw agents` -> private: Contains a personal agent name - private per the brief (its Hermes sub-toggle links a public X post; map it separately if wanted).
- `Mission Control Roadmap` -> private: Matt's own roadmap - private per the brief.
- `Use cases` -> links: links only: the bullets pointing at Matt's private use-case pages carry app.notion.com links (excluded by rule) and their titles are never published.
- `Skill Design Best Practices` -> notes: Plain heading.
- `Design Director Agent - Full Design Agency Replacement` -> links+notes: Plain heading: summary bullets are notes, the source line links the same X post as the Prompts entry (merged); 'Full prompt on Git' is forced private (private [redacted] repo).
- `Token Optimization` -> private: Plain heading whose direct children are a private child page and database; the two sub-headings are mapped above.
- `Other` -> private: Plain heading over private child pages.

## Open questions recorded in the config (need Matt's decision)

- No entry carries a rating or a 'Why:' in Notion, so the generated 'Start here' section is empty and not rendered - add '(8/10)' or 'Why: ...' to a few bullets in Notion to get it.
- Token providers > The Claw Bay is a model-access reseller Matt marked with a question mark; the r/DiscountPremiumAcc thread next to it was dropped. Keep the reseller or remove it in Notion.
- Speciliazed OpenClaw agents is private as a whole (personal agent name); its Hermes sub-toggle links a public X post by @tom_doerr and could be mapped on its own.
- Multi-agent and hierarchy: the Antfarm bullet has no link in Notion (the repository is github.com/snarktank/antfarm) - add the link in Notion to turn the note into an entry.
- Several notes are clipped from linked sources (the r/clawdbot 'if you installed OpenClaw this week' post under Install and first week, awesome-openclaw-tips MEM-01 under Memory and context, Claire Vo's guide under Tools stack) - fine for a personal list, decide whether to attribute them inline.
- agentmatik.ai/llms-full.txt is not merged here (it mixes Claude Code and OpenClaw skills); three OpenClaw-only skills there (antfarm, qmd-skill, openclaw-supermemory) could be merged with a category filter.

## Unmapped, defaulted to private (fail closed)

Toggles:
- `Speciliazed OpenClaw agents > GTM/Sales` (32fdaecf-ce6b-806d-823c-ebde056fe75b)
- `Speciliazed OpenClaw agents > Productivity` (32fdaecf-ce6b-8039-811c-f2461c73476e)
- `Speciliazed OpenClaw agents > Hermes - self improving AI agent with learning loop - https:` (333daecf-ce6b-8072-ac60-ee52e2e89ad6)

Child pages (always private):
- My OpenClaw setup (32fdaecf-ce6b-800a-ab16-c0fb6ebdb625)
- Personal automations (375daecf-ce6b-8086-9f03-c5e24ad230c8)
- Token usage optimization (302daecf-ce6b-8033-a497-f7683ce60166)
- Bazos.cz assessment (2fedaecf-ce6b-80f4-90ad-d9dd9baee33a)
- Workspace File Structure (309daecf-ce6b-81c3-ade5-c9610e68ee70)
- Top Recommended Skills (309daecf-ce6b-81ac-9047-f236209a4560)
- Attack Surface: ClawHub Skills (309daecf-ce6b-8160-9caa-cd2b97266fb2)
- ClawRouter (309daecf-ce6b-81b9-87ba-c5311f9c89e9)
- Heartbeat System (309daecf-ce6b-8119-8c04-d1d886af0c1e)

Child databases (always private):
- OpenClaw Commands (34ddaecf-ce6b-801a-b4a3-e06a375256ea)
- Token intermediaries (303daecf-ce6b-8037-8ec8-d0ae361f5528)

Loose root blocks (private):
- column (34ddaecf-ce6b-8026-95a1-e16171c9ce60)
- column (34ddaecf-ce6b-807c-a4d3-f9a5de7ab480)
- column (34ddaecf-ce6b-80e8-9ec3-c6b9cc7a020f)
- bulleted_list_item (312daecf-ce6b-8069-9e6b-f5ff6584489c)
- bulleted_list_item (32cdaecf-ce6b-8029-a33d-e701410884ba)
- bulleted_list_item (32cdaecf-ce6b-80c2-930c-c3508411649b)
- bulleted_list_item (32cdaecf-ce6b-8084-a4f8-c163a1335e26)
- bulleted_list_item (332daecf-ce6b-8049-acc1-e001f5cdd1b5)
- bulleted_list_item (34bdaecf-ce6b-80b9-8f70-cf11bd10388d)
- bulleted_list_item (34bdaecf-ce6b-803f-823d-ee0b7e361572)
- bulleted_list_item (34bdaecf-ce6b-80fe-8921-d536b406f2f2)
- bulleted_list_item (34bdaecf-ce6b-8035-9096-e94eb28ff33a)
- bulleted_list_item (34bdaecf-ce6b-80d6-86cf-e433b39ce9b2)
- bulleted_list_item (34bdaecf-ce6b-80f4-8eae-ea05e67afa17)
- bulleted_list_item (34bdaecf-ce6b-80c0-b705-f8f8bebac149)
- bulleted_list_item (34bdaecf-ce6b-80c8-9c3d-e07393a14e1f)
- bulleted_list_item (34bdaecf-ce6b-804e-b3e6-cce13297bd5a)
- bulleted_list_item (34bdaecf-ce6b-8047-9614-fdde792b300f)
- bulleted_list_item (34bdaecf-ce6b-8057-95ad-e89d2d77dd90)
- bulleted_list_item (34bdaecf-ce6b-80fd-83dc-c72e2a43887c)
- bulleted_list_item (34bdaecf-ce6b-8056-aebe-e009782dd146)
- bulleted_list_item (34bdaecf-ce6b-800b-b025-ea2942fca19a)
- bulleted_list_item (34bdaecf-ce6b-80f4-b561-e54506fa1f32)
- bulleted_list_item (34bdaecf-ce6b-80ed-865f-e75b715f7bd7)
- bulleted_list_item (34bdaecf-ce6b-8097-b1f1-e4aa4b7ddd97)
- bulleted_list_item (34bdaecf-ce6b-8010-9e53-ec3b85fe0a6e)
- bulleted_list_item (34bdaecf-ce6b-802d-9369-fb79b83c0a1d)
- bulleted_list_item (34bdaecf-ce6b-8038-a39b-e2841c6b6200)
- bulleted_list_item (34bdaecf-ce6b-80a9-a93b-e98328181a16)
- bulleted_list_item (34bdaecf-ce6b-8027-97f0-c4fd00e7b788)
- bulleted_list_item (34bdaecf-ce6b-8089-9458-f69c795c4680)
- bulleted_list_item (34bdaecf-ce6b-800e-b44e-dc2a71bbe27e)
- bulleted_list_item (34bdaecf-ce6b-8080-b373-c90d0834b083)
- bulleted_list_item (34bdaecf-ce6b-80fe-95bd-c1a8a500a939)
- bulleted_list_item (34bdaecf-ce6b-8014-bfe1-febb692b9fd7)
- bulleted_list_item (32cdaecf-ce6b-80cc-aee1-e1c5142ca1b7)
- paragraph (332daecf-ce6b-8067-8b5c-f7aefe8e5974) - x.com
- bulleted_list_item (32fdaecf-ce6b-807c-9104-c7fc02bfef8f)
- bulleted_list_item (30fdaecf-ce6b-80e6-a998-c079797a0123)
- paragraph (332daecf-ce6b-807e-a4ea-ff2e85af4be9)
- paragraph (37bdaecf-ce6b-80a3-b1fc-cebbcd3985d5)
- bulleted_list_item (32cdaecf-ce6b-80a5-9e38-e40d404062f9)
- paragraph (32cdaecf-ce6b-8012-b73b-de13231195cc)
- paragraph (352daecf-ce6b-8002-bcbd-e194cbfde1a1) - app.notion.com
- paragraph (32cdaecf-ce6b-8062-b77f-dd0b6e980c2a)
- paragraph (352daecf-ce6b-80c9-8218-cdeb55dd969b)

Blocks forced private by config (private_block_ids):
- column_list (34ddaecf-ce6b-8016-8b62-f7d8d9ec830e)
- callout (377daecf-ce6b-807f-af8b-fe55ce545881)
- paragraph (34ddaecf-ce6b-8002-b9f3-d9b4125869bb) - bash
- bulleted_list_item (32cdaecf-ce6b-807d-8d23-d2f775a78c46) - Network setup when on home wifi?
- bulleted_list_item (32cdaecf-ce6b-80ff-8ecf-d7f669683515) - mycilium equation - best routing for informatiob spreading, 
- bulleted_list_item (32cdaecf-ce6b-8082-8977-e6722ad92c88) - software more and more conscious so watch immune-system like
- bulleted_list_item (32cdaecf-ce6b-8049-9f39-e2886cbf8c6e) - Using models via Copilot via GIthub subscription (COdex, Son
- bulleted_list_item (32cdaecf-ce6b-8095-8fab-da73494aa4f0) - [redacted] routing to different captains already (subagents doing
- numbered_list_item (34bdaecf-ce6b-805d-a36c-f6541e3d5be8) - Polly, the personal assistant.
- numbered_list_item (34bdaecf-ce6b-8012-a15d-d54eceff3aef) - Finn, the family manager
- numbered_list_item (34bdaecf-ce6b-8061-a0b9-eb368c10085f) - Max the marketer
- numbered_list_item (34bdaecf-ce6b-8063-8b5a-f8cf31106375) - Sam the sales guy
- numbered_list_item (34bdaecf-ce6b-802d-bab7-cbea51cd30a4) - Holly the helpdesk bot
- numbered_list_item (34bdaecf-ce6b-801b-918f-e3afafaaf9cb) - Sage the course operator
- numbered_list_item (34bdaecf-ce6b-8032-8f49-f5f43646f24b) - Howie the How I AI producer
- numbered_list_item (34bdaecf-ce6b-809d-8085-dabf968ea228) - Kelly the developer
- numbered_list_item (34bdaecf-ce6b-80e9-990a-f0d7b1fd0f08) - Q the professor
- child_database (30adaecf-ce6b-80b6-ba5a-c4fdc0307938)
- bulleted_list_item (aaf7ab90-1210-410e-831e-19b7d42f34e4) - Full prompt on Git
- paragraph (7a4384f4-b598-41e4-a87c-5d57d21d8d34) - Source: github.com/BlockRunAI/ClawRouter | Git backup

## Excluded links by reason

- auto-linked-filename: 5
  - bootstrap.md (34ddaecf-ce6b-8023-afed-f80ffce2c528, Install and first week)
  - memory.md (32cdaecf-ce6b-80f6-ab5d-e77d911c6fbf, Memory and context)
  - memory.md (32cdaecf-ce6b-800f-9622-f86c17ed4be9, Multi-agent and hierarchy)
  - soul.md (32cdaecf-ce6b-800f-9622-f86c17ed4be9, Multi-agent and hierarchy)
  - skill.md (49bcf228-f736-4794-8bdd-1392f4a2b74a, Field notes)
- config-exclude_urls: 2
  - https://discord.com/channels/1019361803752456192/1482072289511211200 (32cdaecf-ce6b-8023-86de-d2d64a9d1497, Security)
  - https://www.reddit.com/r/DiscountPremiumAcc/comments/1s75xbm/practically_unlimited_codex_gpt54_from_20_try_for (346daecf-ce6b-80fe-9ae7-f2996983f02d, Models and token burn)
- google-docs: 1
  - docs.google.com (32cdaecf-ce6b-8097-ba61-c55545dd6e3f, Operations)
- local-address: 3
  - 127.0.0.1 (349daecf-ce6b-80fe-ada0-c8656fbb71e0, Install and first week)
  - 0.0.0.0 (34ddaecf-ce6b-80fa-a944-fc61da39bdb9, Security)
- notion: 11
  - app.notion.com (337daecf-ce6b-8087-a14b-da96e66d41ef, Prompts and collections)
  - app.notion.com (32cdaecf-ce6b-801f-b573-ceb1e5499a1a, Use cases)
  - app.notion.com (30adaecf-ce6b-8072-8724-f5b2b443affb, Use cases)
  - app.notion.com (32cdaecf-ce6b-80a3-a289-d467656eccf4, Use cases)
  - app.notion.com (32cdaecf-ce6b-80a9-92dd-cd45f1de680a, Use cases)
  - app.notion.com (32cdaecf-ce6b-80b1-891f-f2a399998cf8, Use cases)
  - app.notion.com (32cdaecf-ce6b-8007-bd16-df4a19bf6a95, Use cases)
  - app.notion.com (32cdaecf-ce6b-80b2-8852-e16bed4d1356, Use cases)
  - app.notion.com (32cdaecf-ce6b-801a-9deb-cbeddc16c9ee, Use cases)
  - app.notion.com (32cdaecf-ce6b-80ad-88ad-fed717040ac7, Use cases)
  - app.notion.com (32cdaecf-ce6b-808b-8fa3-e2ea01f18f56, Use cases)
- notion-internal: 2
  - (internal) (332daecf-ce6b-80e5-b5e0-caf166a86ce9, Skills)
- config exclude_urls hits:
  - https://discord.com/channels/1019361803752456192/1482072289511211200 (32cdaecf-ce6b-8023-86de-d2d64a9d1497)
  - https://www.reddit.com/r/DiscountPremiumAcc/comments/1s75xbm/practically_unlimited_codex_gpt54_from_20_try_for (346daecf-ce6b-80fe-9ae7-f2996983f02d)

## Entries missing a description (Notion text)

- Field notes / General: Back up agent workspace - https://docs.openclaw.ai/concepts/agent-workspace (32cdaecf-ce6b-801f-82d3-fc363ff7f021)
- Field notes / General: Health check help - https://docs.openclaw.ai/gateway/health (349daecf-ce6b-803f-9c90-fbb0f782097a)
- Field notes / General: Set up help project with Openclaw documentation from - https://context7.com (35edaecf-ce6b-800b-b13d-f779284857fc)
- Field notes / General: put them in.openclaw/.env - https://docs.openclaw.ai/help/environment (34bdaecf-ce6b-80a8-b3d5-ca8de6af8423)
- Field notes / Self-improving: Self-improving skill - https://x.com/coreyganim/status/2035757428579389768 (32cdaecf-ce6b-8012-8038-ce5de44d4158)
- Install and first week: lennysnewsletter.com/p - https://www.lennysnewsletter.com/p/openclaw-the-complete-guide-to-building (349daecf-ce6b-8072-9ddf-f4ec3bebed2b)
- Install and first week: r/clawdbot post - https://www.reddit.com/r/clawdbot/comments/1s270n0/if_you_installed_openclaw_this_week_read_this (34ddaecf-ce6b-801d-a3bb-fe6564d45653)
- Install and first week / Browser choice: brave.com/search - https://brave.com/search/api (349daecf-ce6b-809d-b10b-e41348213c00)
- Install and first week / Browser choice: docs.openclaw.ai/tools - https://docs.openclaw.ai/tools/web (349daecf-ce6b-80b3-b869-d914df805a2c)
- Install and first week / Channel choice: Set up Telegram guide here - https://docs.openclaw.ai/channels/telegram (349daecf-ce6b-80c7-ad81-fafe0cf04f3f)
- Learn: @coreyganim on X - https://x.com/coreyganim/status/2036103806975426779 (330daecf-ce6b-8032-8d6d-df247636554a)
- Learn: @ernestosoftware on X - https://x.com/ernestosoftware/status/2037187494530208029 (330daecf-ce6b-8042-aab8-dd6a3eb839db)
- Learn: @gregisenberg on X - https://x.com/gregisenberg/status/2034778615464735000 (330daecf-ce6b-803d-9843-d1efd96c1c77)
- Learn: @moritzkremb on X - https://x.com/moritzkremb/status/2029304864719667335 (332daecf-ce6b-80dc-a269-cfb593002bfe)
- Learn: @roundtablespace on X - https://x.com/roundtablespace/status/2044879754969387022 (344daecf-ce6b-8069-a5ba-df9d1dcb6fd5)
- Learn: @ryancarson on X - https://x.com/ryancarson/status/2039786704731541903 (333daecf-ce6b-8086-8572-df3ceb1b8996)
- Learn: LinkedIn post - https://www.linkedin.com/posts/petergyang_this-is-the-most-complete-setup-ive-seen-ugcPost-7459248459813064705-5eB4 (35ddaecf-ce6b-806e-8902-d25ff575f4f5)
- Learn: YouTube video DIa0MYJzM5I - https://www.youtube.com/watch?v=DIa0MYJzM5I&t=1s (34ddaecf-ce6b-800e-ba20-cd919fee63de)
- Learn: YouTube video fd4k16REDOU - https://www.youtube.com/watch?v=fd4k16REDOU (335daecf-ce6b-806f-9cc2-ff1028b443e0)
- Learn: YouTube video nSBKCZQkmYw - https://www.youtube.com/watch?v=nSBKCZQkmYw (342daecf-ce6b-8045-bc4d-cec85c11af83)
- Learn: mistakes - https://x.com/kloss_xyz/status/2032011756890177552 (321daecf-ce6b-8061-a824-ebc9cae2b139)
- Learn: r/OpenClawUseCases post - https://www.reddit.com/r/OpenClawUseCases/comments/1rd9t8b/i_rebuilt_my_entire_life_os_with_openclaw_after (342daecf-ce6b-8068-895c-d6aa489f0e4b)
- Memory and context: @ksimback on X - https://x.com/ksimback/status/2024180197910864182 (32cdaecf-ce6b-80ef-a2c3-ca6080dab7c7)
- Memory and context: Supermemory - https://supermemory.ai (32cdaecf-ce6b-8057-9d6d-d4fce7657603)
- Models and token burn: localite heartbeat and use local model for it - https://www.instagram.com/p/DVJPnoGkvnd?img_index=1 (32cdaecf-ce6b-80e6-a0f9-e5cd744f24ae)
- Models and token burn / GPT 5.4: when switching do these settings - https://www.reddit.com/r/openclaw/comments/1sgpg8b/a_lot_of_the_new_gpt_54_sucks_in_openclaw_posts (34cdaecf-ce6b-80de-a7d9-eefb151c8147)
- Models and token burn / GPT 5.5: how to switch - https://x.com/cherry_mx_reds/status/2047390468778901738 (34ddaecf-ce6b-805a-b59e-e34f0d51d875)
- Operations / Finances: Link - wallet for agents by Stripe (Tweet) - https://link.com/en-cz/agents (353daecf-ce6b-800a-b153-cb71dd2a36d4)
- Operations / Local Mac vs VPS: Amazon EC2 (Ubuntu, instance c7iflex.large, 30GB, Tutorial) - https://www.youtube.com/watch?v=04wh2Hlgbds (32cdaecf-ce6b-8082-964a-c9beeb568e46)
- Operations / Own dashboard: claw3d.ai - https://www.claw3d.ai (32cdaecf-ce6b-809d-a470-cb95b658db9e)
- Prompts and collections / Business ideas and inspiration: agentsidehustleschool.com - https://agentsidehustleschool.com?mode=human (342daecf-ce6b-800b-91c0-f7f0d63ab19d)
- Prompts and collections / Collections: Awesome Openclaw - https://github.com/alvinreal/awesome-openclaw (34ddaecf-ce6b-80af-a809-f3932b52caa9)
- Prompts and collections / Collections: Awesome Openclaw Tips - https://github.com/alvinreal/awesome-openclaw-tips#mem-01-make-your-agent-learn-from-its-mistakes (34ddaecf-ce6b-80f3-a174-c0e1573091f6)
- Prompts and collections / Collections: Awesome openclaw skills - https://github.com/VoltAgent/awesome-openclaw-skills (377daecf-ce6b-80df-bd73-e025758e35bd)
- Prompts and collections / Prompts: Sort - https://gist.github.com/mberman84/065631c62d6d8f30ecb14748c00fc6d9 (31fdaecf-ce6b-8032-9ccf-e75c7a3eb8e6)
- Security: Nemoclaw (Link, Discord Nemo channel) - https://www.nvidia.com/en-us/ai/nemoclaw (32cdaecf-ce6b-8023-86de-d2d64a9d1497)
- Security: YouTube video jw_o0xr8MWU - https://www.youtube.com/watch?v=jw_o0xr8MWU&t=2647s (33adaecf-ce6b-80c6-a6b8-f7195bf9053d)
- Skills / General: Skill graphs - https://x.com/arscontexta/status/2023957499183829467 (332daecf-ce6b-80c9-a2f2-d11c7fc076fe)
- Skills / Marketing, Ads & SEO: 7 Openclaw skills for Paid Media - https://www.get-ryze.ai/blog/openclaw-google-meta-ads-guide (332daecf-ce6b-805d-b632-c363c5fa5bc8)
- Skills / Security: clawdhub.com/peterokase42/dont-hack-me - Security self-check - https://clawdhub.com/peterokase42/dont-hack-me (332daecf-ce6b-8026-8d7d-dcabfdf625e4)
- Skills / Skill platforms: Clawhub - https://clawhub.ai/skills?sort=downloads (344daecf-ce6b-8095-bcc7-e42d68c22ac4)
- Skills / Token Efficiency: github.com/levineam/qmd-skill - Cuts token usage by 95% - https://github.com/levineam/qmd-skill (332daecf-ce6b-808d-9911-d225a53e322c)
- Use cases: Repo with use cases - https://github.com/hesamsheikh/awesome-openclaw-usecases (32cdaecf-ce6b-80ca-8eea-ffc70355415b)
- Use cases: morning brief - https://www.youtube.com/watch?v=04wh2Hlgbds&t=572 (32cdaecf-ce6b-8057-bf70-d1d8c31e5570)

## Entries named from their URL (no usable link text)

- r/OpenClawUseCases post - https://www.reddit.com/r/OpenClawUseCases/comments/1rd9t8b/i_rebuilt_my_entire_life_os_with_openclaw_after (342daecf-ce6b-8068-895c-d6aa489f0e4b)
- @ernestosoftware on X - https://x.com/ernestosoftware/status/2037187494530208029 (330daecf-ce6b-8042-aab8-dd6a3eb839db)
- @gregisenberg on X - https://x.com/gregisenberg/status/2034778615464735000 (330daecf-ce6b-803d-9843-d1efd96c1c77)
- @coreyganim on X - https://x.com/coreyganim/status/2036103806975426779 (330daecf-ce6b-8032-8d6d-df247636554a)
- @moritzkremb on X - https://x.com/moritzkremb/status/2029304864719667335 (332daecf-ce6b-80dc-a269-cfb593002bfe)
- @ryancarson on X - https://x.com/ryancarson/status/2039786704731541903 (333daecf-ce6b-8086-8572-df3ceb1b8996)
- LinkedIn post - https://www.linkedin.com/posts/petergyang_this-is-the-most-complete-setup-ive-seen-ugcPost-7459248459813064705-5eB4 (35ddaecf-ce6b-806e-8902-d25ff575f4f5)
- YouTube video nSBKCZQkmYw - https://www.youtube.com/watch?v=nSBKCZQkmYw (342daecf-ce6b-8045-bc4d-cec85c11af83)
- YouTube video DIa0MYJzM5I - https://www.youtube.com/watch?v=DIa0MYJzM5I&t=1s (34ddaecf-ce6b-800e-ba20-cd919fee63de)
- YouTube video fd4k16REDOU - https://www.youtube.com/watch?v=fd4k16REDOU (335daecf-ce6b-806f-9cc2-ff1028b443e0)
- @roundtablespace on X - https://x.com/roundtablespace/status/2044879754969387022 (344daecf-ce6b-8069-a5ba-df9d1dcb6fd5)
- lennysnewsletter.com/p - https://www.lennysnewsletter.com/p/openclaw-the-complete-guide-to-building (349daecf-ce6b-8072-9ddf-f4ec3bebed2b)
- docs.openclaw.ai/tools - https://docs.openclaw.ai/tools/web (349daecf-ce6b-80b3-b869-d914df805a2c)
- brave.com/search - https://brave.com/search/api (349daecf-ce6b-809d-b10b-e41348213c00)
- r/clawdbot post - https://www.reddit.com/r/clawdbot/comments/1s270n0/if_you_installed_openclaw_this_week_read_this (34ddaecf-ce6b-801d-a3bb-fe6564d45653)
- @ksimback on X - https://x.com/ksimback/status/2024180197910864182 (32cdaecf-ce6b-80ef-a2c3-ca6080dab7c7)
- YouTube video jw_o0xr8MWU - https://www.youtube.com/watch?v=jw_o0xr8MWU&t=2647s (33adaecf-ce6b-80c6-a6b8-f7195bf9053d)
- claw3d.ai - https://www.claw3d.ai (32cdaecf-ce6b-809d-a470-cb95b658db9e)
- clawdhub.com/JimLiuxinghai - https://clawdhub.com/JimLiuxinghai/find-skills (332daecf-ce6b-80c7-8e62-d32cdc305460)
- supermemoryai/clawbot-supermemory - https://github.com/supermemoryai/clawbot-supermemory (332daecf-ce6b-80cb-b263-f4c98959b81a)
- clawdhub.com/seojoonkim - https://clawdhub.com/seojoonkim/prompt-guard (332daecf-ce6b-80e2-8c90-f83f4f8e9d33)
- agentsidehustleschool.com - https://agentsidehustleschool.com?mode=human (342daecf-ce6b-800b-91c0-f7f0d63ab19d)

## Promoted entries (github URL rescued from a block whose primary was a duplicate)

- none

## Name collisions (same normalized name, different URL)

- none

## ROTATE warnings (secret-shaped text found on the private side)

- none

## Denylist

- private-side hits (expected, not published): 10
- public-side hits: 0 (any hit aborts the run with exit 3)
- config text_replacements applied to public text (rule -> replacement text x count): 'your agent' x5, 'your main machine' x2

## Open decisions (from tools/lint.py)

Refreshed by every `python3 tools/lint.py` run. Each line needs a human decision: fix it in `data/overrides.json` (name, description, url) or change the source in Notion, then re-sync.

- none, lint passes
