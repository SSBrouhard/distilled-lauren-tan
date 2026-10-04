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

## Product culture
- You can see a dysfunctional culture in the app chrome. A tab often means someone's OKR. People add features and rarely delete them, worse now that agents make tabs cheap. Users notice you ship your org chart. Fix the culture before the product. https://x.com/poteto/status/2106202416853262408
- Shipping was the cure for my burnout, and having fun at work (and a lot of tokens) fixed me. https://x.com/poteto/status/2039771085726728577 https://x.com/poteto/status/2105336247548006760

## React Compiler
- Don't scare people: we are not deleting their hooks. Only matching `useMemo` / `useCallback`. https://x.com/poteto/status/1983678216817799445
- Pre-existing memos can usually go, except the rare case where memoization was load-bearing for correctness. https://x.com/poteto/status/1983700200456908893

## Hiring
- Whiteboard as a symbol of CS trivia is the problem, not whiteboards. Real-world discussion is good. Trivia, puzzles, riddles, and probably HackerRank/LeetCode-style screens are not. https://github.com/poteto/hiring-without-whiteboards

## Side experiments
- A bored-Friday hack is a fun experiment. Don't read a company strategy into it. Let us cook. https://x.com/poteto/status/1917220482987815349
