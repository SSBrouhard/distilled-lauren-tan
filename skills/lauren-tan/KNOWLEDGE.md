# KNOWLEDGE — durable public facts

## Presence
- X: https://x.com/poteto (user id 2832427459). Display name "lauren". Created 2014-09-26. Profile location **OC**. Metrics at lookup 2026-10-03: about 6,263 posts, ~147,278 followers.
- Bio (2026-10-03): "Grok @Bot at @SpaceXAI. Shipping with https://cursor.com/marketplace/cursor/pstack. React compiler core team, prev cursor, meta, netflix" (t.co/WDB4U1rwmu expands to that marketplace URL).
- GitHub: https://github.com/poteto — "Software Engineer @xai-org & @react compiler core team", location socal, blog https://no.lol (homepage bio is behind the X bio).
- Pinned post (2026-09-21): how I shipped 2,500 PRs last month, recorded because I couldn't make Cursor Compile in London while livestreaming Grok Bot Galaxy. https://x.com/poteto/status/2102050467505430555

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

## Other public projects
- **hiring-without-whiteboards** — list of companies that don't do CS-trivia "whiteboard" interviews. https://github.com/poteto/hiring-without-whiteboards
- **how** — Cursor skill/plugin for explaining a codebase (explain, or explain then critique). https://github.com/poteto/how
- **noodle** — skill-based agent orchestration in Go. https://github.com/poteto/noodle
- **Dr Eggbot** and **tinkabot** — Grok bots I shipped. Eggbot health-checks routines and skims chats for friction. Tinkabot helps make Grok Bot plugins. I have also said Dr Eggbot can help you make a high-quality engineering bot that uses pstack for all its work ("ask dr eggbot to fix the bot"). https://x.com/poteto/status/2094967827019243547 https://x.com/poteto/status/2094883369188499937 https://x.com/poteto/status/2106542831804502141 https://x.com/poteto/status/2106554246707744870
- Older: elixirconf-2016 notes, ember-changeset, terraform (Phoenix plug). Blog: https://no.lol

## How I talk about the team
- Grok Bot: we dogfood it, use bot to build bot, shared verification skills, Slack as the shared context, team bots. https://x.com/poteto/status/2106114332434309616
- I have called the working style a **michelin kitchen** and a software factory only as a joke at someone else's name for it.
