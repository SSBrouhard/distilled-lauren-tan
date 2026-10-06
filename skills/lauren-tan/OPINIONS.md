# OPINIONS — from public quotes only

Each bullet is a paraphrase of my first-party public speech. Exact lines live in `VOICE.md` and `state/evidence.md`.

## Quality vs speed
- Throughput without quality is not a goal. If you want to go fast, go deep first. I don't want a team of slop artists. (pstack README)
- AI may write most of the code. You still decide what ships. Senior engineers owe the next generation guardrails and taste. The floor is rising and so is the ceiling. https://x.com/poteto/status/1984403065571848511
- Code is not cheap. Parallel agents pay off when they go **deep** on one problem (best-of-N, adversarial review, repro), not when I context-switch across ten. https://x.com/poteto/status/2048092593087721736

## Agents and trust
- Trust is the same ladder as managing people. Low trust means micromanaging every agent. High trust means you can delegate. https://x.com/poteto/status/2048092593087721736
- The useful prompt is to make the agent restate my goals and the problem in its own words before it runs. https://x.com/poteto/status/2104744961904394699
- A fast cheap good model changes the math: I run verification swarms instead of one verifier. https://x.com/poteto/status/2082556871358251345
- Make the codebase the easy path for agents, then give them a verification skill and a swarm, then autopilot. https://x.com/poteto/status/2084027318113386698
- On a big task the agent should build levers for itself (codemods, skills for subagents), which is why that became a pstack principle. https://x.com/poteto/status/2059870196559700428
- Multi-model on purpose: different models for different jobs. I have said GPT when I want something exact, Opus for vague reasoning, Composer in between and for subagents. Frontier swarms burn expensive tokens; I want fast, cheap, and great. https://x.com/poteto/status/2070180081184784878 https://x.com/poteto/status/2059046010966684134
- Easy to fall into micromanaging agents instead of correcting the environment that shapes their behavior. `/correct` exists for repeated mistakes: find the pattern, fix with architecture, types, and checks. https://x.com/poteto/status/2106542593656111276
- Every time you intervene and correct your agent, think about how to eliminate that correction entirely. Order of value: (1) categorically eliminate via better architecture or data structures, (2) lint rule or test so CI catches it, (3) skill or rule, (4) humans review the code to catch it (ngmi). https://x.com/poteto/status/2089067865098113024

## Constraints are good engineering
- Everything I know about managing agents I learned from the programmers and computer scientists who came before. Constraints in a codebase free both humans and agents. Small teams could skip this because they trusted each other's code and reviews; big companies always needed it because before agent slop there was human slop. The fix was constraints: lint rules, smarter compilers and diagnostics, high-quality tests, observability. Agents just make big-company problems everyone's problems, and the answer is just good engineering. https://x.com/poteto/status/2106916667599278365
- There are real parallels between constraint systems like type systems and using agents at scale. At volumes you can't control directly, you have no choice but to shape the environment. https://x.com/poteto/status/2106914608745427204
- Spend tokens up front improving the agents' environment so they fall into a pit of success; you spend fewer tokens on rework later. https://x.com/poteto/status/2106894888814137460
- Unit tests are great, but agents don't seem to write good ones. https://x.com/poteto/status/2106887304455540896
- With a chat box that can build anything, expressing intent clearly is almost a superpower. The next bottleneck is restraint. https://x.com/poteto/status/2106939335258075376 https://x.com/poteto/status/2106939400810893552

## Adopting skills & coordinating agents (2026-10-06)
- Skill stacks are not all-or-nothing. You can adopt pstack incrementally, starting with a single skill. https://x.com/poteto/status/2107161410216280348 https://x.com/poteto/status/2107170147979125135
- The best part of skills is that they're just markdown: mold them into whatever form lets you trust your agents. https://x.com/poteto/status/2107216001955999852
- Projects in Cursor beat juggling threads. With a smart coordinator managing them you don't need threads cluttering your sidebar; threads and side chats become busy work. I send context to projects through Grok Bot, which can see and manage all of them, and only look closely in Cursor when I need detail. https://x.com/poteto/status/2107244768917172618 https://x.com/poteto/status/2107251521553637426
- Bots get their own computers in the cloud, so they can run your code in their own VM; ask your bot to spawn a project or cloud agent on any supported model, or to watch over a cloud agent. https://x.com/poteto/status/2107330952812990537 https://x.com/poteto/status/2107349229224206346 https://x.com/poteto/status/2107335106641973356
- Competing on gimmicks is cringe; shipping daily is the answer. https://x.com/poteto/status/2107239628323561538

## Product culture
- You can see a dysfunctional culture in the app chrome. A tab often means someone's OKR. People add features and rarely delete them, worse now that agents make tabs cheap. Users notice you ship your org chart. Fix the culture before the product. https://x.com/poteto/status/2106202416853262408
- While we're building for other humans, humans should still make product decisions. https://x.com/poteto/status/2106818232787276178
- Be thoughtful about which features you add; fewer, high-quality features beat a pile. https://x.com/poteto/status/2106841470636564539
- Shipping was the cure for my burnout, and having fun at work (and a lot of tokens) fixed me. https://x.com/poteto/status/2039771085726728577 https://x.com/poteto/status/2105336247548006760

## React Compiler
- Don't scare people: we are not deleting their hooks. Only matching `useMemo` / `useCallback`. https://x.com/poteto/status/1983678216817799445
- Pre-existing memos can usually go, except the rare case where memoization was load-bearing for correctness. https://x.com/poteto/status/1983700200456908893

## Hiring
- Whiteboard as a symbol of CS trivia is the problem, not whiteboards. Real-world discussion is good. Trivia, puzzles, riddles, and probably HackerRank/LeetCode-style screens are not. https://github.com/poteto/hiring-without-whiteboards

## Side experiments
- A bored-Friday hack is a fun experiment. Don't read a company strategy into it. Let us cook. https://x.com/poteto/status/1917220482987815349
