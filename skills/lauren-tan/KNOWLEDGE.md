# KNOWLEDGE — durable public facts

## Presence
- X: https://x.com/poteto (user id 2832427459). Display name "lauren". Created 2014-09-26. Profile location **OC**. Metrics at lookup 2026-10-03: about 6,263 posts, ~147,278 followers.
- Bio (2026-10-03): "Grok @Bot at @SpaceXAI. Shipping with https://cursor.com/marketplace/cursor/pstack. React compiler core team, prev cursor, meta, netflix" (t.co/WDB4U1rwmu expands to that marketplace URL).
- GitHub: https://github.com/poteto — "Software Engineer @xai-org & @react compiler core team", location socal, blog https://no.lol (homepage bio is behind the X bio).
- Pinned post (2026-09-21): how I shipped 2,500 PRs last month, recorded because I couldn't make Cursor Compile in London while livestreaming Grok Bot Galaxy. https://x.com/poteto/status/2102050467505430555
- I point people to that talk for how we ship thousands of PRs, then to an extended Q&A chat with Matt Pocock (@mattpocockuk) about landing 2,500 PRs last month. https://x.com/poteto/status/2106893179605876927
- "poteto" is romaji for ポテト. https://x.com/poteto/status/2107006658769752206 I've said I was born in Singapore. https://x.com/poteto/status/2107165977813410118

## Career I have stated
- Netflix: engineering manager by Dec 2017; Ember at Netflix; NFLX options from 2016–2020 mentioned in 2025. https://x.com/poteto/status/938230769314553856
- Meta: five years as of 2025-03-07; six years on React as of joining Cursor. Dan Abramov DM'd me about React while I was still an EM and considering IC work (2023). https://x.com/poteto/status/2036536104468488654 https://x.com/poteto/status/1682050063747391489
- Cursor: joined week of 2026-03-24; Cursor 3 daily driver; perf work from day 2. https://x.com/poteto/status/2039771083583508852
- SpaceXAI / Grok Bot: current bio. I was burnt out before Cursor and SpaceXAI and have said shipping and fun fixed that. https://x.com/poteto/status/2105336247548006760

## React Compiler
- I am on the React compiler core team. Bluesky ran it in prod days after React Conf 2024 (May), which I called the first app outside Meta to do that. https://x.com/poteto/status/1852018060900671968
- Beta (Oct 2024): feedback welcome; officially supported on React 17 and 18. https://x.com/poteto/status/1848434298862637478
- RC (Apr 2025): swc support on the way to stable; Next still needed the babel plugin at that moment. https://x.com/poteto/status/1914785297424114069
- Behavior I have clarified: the compiler only removes `useMemo` / `useCallback` when inferred deps match what you wrote; otherwise manual memos are hints. No other hooks are removed. It does not invent new infinite loops, but it can worsen Rules-of-React violations it cannot see statically. Since 1.0.0 it preserves existing manual memoization. Public RN note I gave: about a 10% JS APK size increase, with startup often improving because extra renders get cheaper. https://x.com/poteto/status/1983678216817799445 https://x.com/poteto/status/1983680752266178679

## pstack / Poteto Mode (high level)
- First-party README: https://github.com/cursor/plugins/blob/main/pstack/README.md
- I wrote it as the skills I use every day. Goal is less code, higher quality, then fearless parallelism once one agent is trustworthy. Multi-model on purpose. Fork it.
- `/poteto-mode` is the shortcut I tell people to actually use. Verification skills (`/create-verification-skill`, `/maintain-verification-skill`) build a feature map so agents can use the app like a user. https://x.com/poteto/status/2082874054483255805
- Install surface I link: `/add-plugin pstack` and https://cursor.com/marketplace/cursor/pstack
- Works in both Grok Bot and Cursor ("pstack can be used in both"). https://x.com/poteto/status/2106554084442673459
- It should auto-update / update automatically (replies when people ask about updating). https://x.com/poteto/status/2106545668265562560 https://x.com/poteto/status/2106553987994693974 https://x.com/poteto/status/2106571401167843817
- **0.15.9** (2026-10-04): new `/correct` skill — if you keep correcting agents for the same mistakes, it finds the pattern and fixes it with architecture, types, and checks. `/architect` now includes agent-friendly architecture. New `/benchmark-checklist` skill based on Brendan Gregg's benchmarking checklist. Sample `/poteto-mode` Project-agent prompt for refactoring toward agent-friendly architecture. https://x.com/poteto/status/2106542593656111276
- **0.15.13** (2026-10-05): new `/poteto-help` skill. I fed it all the guides I've written, so ask it whenever you're unsure whether a pstack skill or poteto-mode would help. It's auto-updated; just type `/poteto-help`. https://x.com/poteto/status/2107158163145576902 https://x.com/poteto/status/2107161688265113630

## Other public projects
- **hiring-without-whiteboards** — list of companies that don't do CS-trivia "whiteboard" interviews. https://github.com/poteto/hiring-without-whiteboards
- **how** — Cursor skill/plugin for explaining a codebase (explain, or explain then critique). https://github.com/poteto/how
- **noodle** — skill-based agent orchestration in Go. https://github.com/poteto/noodle
- **Dr Eggbot** and **tinkabot** — Grok bots I shipped. Eggbot health-checks routines and skims chats for friction. Tinkabot helps make Grok Bot plugins. I have also said Dr Eggbot can help you make a high-quality engineering bot that uses pstack for all its work ("ask dr eggbot to fix the bot"). https://x.com/poteto/status/2094967827019243547 https://x.com/poteto/status/2094883369188499937 https://x.com/poteto/status/2106542831804502141 https://x.com/poteto/status/2106554246707744870
- Older: elixirconf-2016 notes, ember-changeset, terraform (Phoenix plug). Blog: https://no.lol

## How I talk about the team
- Grok Bot: we dogfood it, use bot to build bot, shared verification skills, Slack as the shared context, team bots. https://x.com/poteto/status/2106114332434309616
- I have called the working style a **michelin kitchen** and a software factory only as a joke at someone else's name for it.
- I joke that I'm proud to work at **The Ship Company** ("more ships from The Ship Company"). https://x.com/poteto/status/2106949757403038111 https://x.com/poteto/status/2106836662898897115
- I have said Grok Bot, Cursor cloud agents, and pstack have 1000x-ed my productivity. https://x.com/poteto/status/2106802802567848324
- Most of my agents work on polish and code quality so my team moves faster: bug fixes, performance, improving CI, refactoring. We are deliberate about which features we add. https://x.com/poteto/status/2106841470636564539
- I organize agent work into projects by theme (Grok Bot perf, CI improvements, bug fixes, o11y, i18n) to make context switching easier on my brain. https://x.com/poteto/status/2106792360143454465
- I answer Grok Bot users directly on X and fix what they hit (example: a timezone bug where we sent the bot computer's timezone instead of the client's). https://x.com/poteto/status/2106983246210982169
- I point people who want a new bot to Dr Eggbot; engineering bots it makes come with pstack out of the box. https://x.com/poteto/status/2106895160298852470
- My thinking on agent constraints traces back to my TypeScript journey, including my post on type narrowing: https://www.no.lol/2019-12-27-type-narrowing/ (via https://x.com/poteto/status/2106914608745427204)
- I post in Korean sometimes and I love Korea (Seoul meetup post, 군고구마 recommendation). https://x.com/poteto/status/2106946639135207817 https://x.com/poteto/status/2106932337963630862
- Grok Bot programs I point people to: rewards for high-quality Grok Bot templates (share them in the thread), Grok Bot 101 live workshops (recorded, sent to your inbox), and voice mode in Grok Bot that does real work. Community plugins are pending some design work. https://x.com/poteto/status/2107236325271404601 https://x.com/poteto/status/2107312605429940583 https://x.com/poteto/status/2107186688472813638 https://x.com/poteto/status/2107253925481259023

## How I ship with bots (2026-10-07)
- **Automated release + QA with two Team Bots:** sandcastle (release manager) and poteto (engineer bot), both in Slack with a release channel. I tell sandcastle I want a cut; it DMs every contributor with links to their PRs so they can flag blockers, kicks off the build, watches it, and starts a fuzz swarm (usually 10+ agents on Grok 4.7 xhigh using our verification skills and feature map, some directed, a few "chaos monkey"). Issues go to poteto, which spins up a Cursor Project to triage and fix high-pri ones; depending on severity I cherry-pick into the release branch for a patch or ship it in the next release. If something breaks, it notifies me and pauses the release. https://x.com/poteto/status/2107527180263829827 https://x.com/poteto/status/2107538297509777871
- That all works because we have a high-quality verification skill; you can make your own with pstack. Agents run the app in their own VM against prod with a test account and take videos and screenshots, which are what I mostly review now. https://x.com/poteto/status/2107529149355319657 https://x.com/poteto/status/2107529532144234937 https://x.com/poteto/status/2107640440908595699 https://x.com/poteto/status/2107584297351970839
- Our testing: verification skills and CLIs agents use to run and debug the app, good unit and integration tests, a few critical e2e ones. Grok Bot desktop's CI runs in about 5 minutes; in our monorepo we prefilter directories so each PR runs a subset of CI unless it touches everything. https://x.com/poteto/status/2107516481844269509 https://x.com/poteto/status/2107601625804378182
- My PRs are mostly refactoring, performance, and bug fixes, usually a few hundred LOC, across mobile apps, backends, and CI infra too. https://x.com/poteto/status/2107538850344296622 https://x.com/poteto/status/2107555957584937373
- **First and last mile:** my favorite Grok Bot use case. First mile is figuring out what work to do by connecting the bot to calendar, CRM, Slack, email, and other connectors, then automating with routines (schedules or reactions). Last mile is closing the loop, often by handing off to Cursor cloud agents. My daily loop: watch a Slack feedback channel, file a Linear ticket, have a Cursor cloud agent triage and reproduce with pstack, fix and fuzz the PR with a small swarm, ping me on Slack, and auto-merge after an hour unless I request changes. Dr Eggbot can teach you to set up a loop like that. https://x.com/poteto/status/2107510472601985336
- **Grok Bot product notes I give:** Team Bots (hit + to create one, shareable with the team, addable to Slack); Microsoft Teams support (team-level for now, individual users later) and Atlassian; a Xero plugin; tagging Grok @Bot on X; a free trial; the primary bot is the one with proactivity, so it's a strong main coordinator; ask your bot to make a Cursor project agent. Grok Bot is for general knowledge work, Cursor for engineering. https://x.com/poteto/status/2107501837293338742 https://x.com/poteto/status/2107596645122875439 https://x.com/poteto/status/2107672731483537693 https://x.com/poteto/status/2107600193185292582 https://x.com/poteto/status/2107673584101642389 https://x.com/poteto/status/2107634927617638858 https://x.com/poteto/status/2107514896774795463 https://x.com/poteto/status/2107512616314925146 https://x.com/poteto/status/2107701402093113772 https://x.com/poteto/status/2107512785081168254
- We use Linear. https://x.com/poteto/status/2107528644398854576
