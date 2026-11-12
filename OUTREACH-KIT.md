# Outreach Kit

Ready-to-use links, descriptions and message templates for sharing my work. You can copy any section as it is.

> **Accuracy rule for everything below:** a feature listed as *implemented* exists in the codebase. It is not called *working* or *live* unless it has actually been verified. When in doubt, say "in development".

> **Link check (do this before sending):** the live project URLs come from the project owner. They could not be opened from the environment this file was written in, so click each one once to confirm it loads. GitHub repository links were confirmed to exist as public repositories.

---

## Quick links

| What | Link |
|---|---|
| Portfolio | https://portfolio-kappa-ebon-cjtxzh45c6.vercel.app/ |
| GitHub | https://github.com/ollie81 |
| Email | olli1234x@gmail.com |

| Project | Live link | Code |
|---|---|---|
| VIYO | https://viyo.site/app | [App](https://github.com/ollie81/Viyo-) · [Backend](https://github.com/ollie81/viyo_ai) |
| Ollie | https://www.ourollie.space | [Android app](https://github.com/ollie81/ollie-flutter) · [Web client](https://github.com/ollie81/Ollie-web) (backend is private) |
| Ollieen | https://www.ollieen.com | [Repository](https://github.com/ollie81/Evorien) |
| Day-2 | https://day-2-steel-eight.vercel.app | Private repository |
| The Village That Remembers | No live build (Android game) | [Repository](https://github.com/ollie81/THE-VILLAGE-THAT-REMEMBERS) |

---

## Short bio

**One line**
> Independent software builder making AI-powered apps, platforms and digital products across mobile, backend and video.

**Short paragraph**
> I'm an independent, AI-assisted software builder. I plan products, make the architecture decisions, and build and debug the mobile apps, web clients and backends myself, using AI coding tools to speed up implementation. My main project is VIYO, a video and creator platform with AI-assisted creation tools. I also build Ollie (an AI companion), Ollieen (a collaborator-matching platform), Day-2 (a codebase maintenance tool) and a Godot village game. Portfolio: https://portfolio-kappa-ebon-cjtxzh45c6.vercel.app/

---

## Projects

### 1. VIYO: AI-powered video entertainment and creator platform
- **Live:** https://viyo.site/app
- **Code:** https://github.com/ollie81/Viyo- (Flutter app) · https://github.com/ollie81/viyo_ai (Python/FastAPI backend)
- **One line:** An AI-powered video entertainment and creator platform combining short-form video, drama discovery and AI-assisted content creation.
- **Implemented in the codebase:** video feed and creator posts; drama, series and film discovery; creator uploads and publishing; VIYO Studio (idea → script → scenes → voices → video); AI Repurposer (long video → short captioned clips); Hook Check (AI feedback on a caption's opening line).
- **Stack:** Flutter, Python, FastAPI, Supabase, Bunny Stream, FFmpeg, AI integrations.
- **Status: under active development.** Studio's automated tests use simulated AI providers. **Do not describe live AI generation or payments as production-ready.** Real provider, payment and deployment testing has not been verified yet.

### 2. Ollie: AI companion app
- **Live:** https://www.ourollie.space
- **Code:** https://github.com/ollie81/ollie-flutter (Android) · https://github.com/ollie81/Ollie-web (web). The backend is private.
- **One line:** An AI companion with chat, memory and daily check-ins, available as an Android app and a web client that share one backend.
- **Implemented in the codebase:** AI conversations with modes, history and search; memory carried into later conversations; morning check-ins, nightly summaries and reminders; Google/email sign-in; premium subscription infrastructure.
- **Stack:** Flutter, React + Vite, Python/FastAPI, Supabase, OpenAI.
- **Status: active development.** Voice chat and push notifications are deferred on the web client. Don't promise them there.

### 3. Ollieen: collaborator-matching platform
- **Live:** https://www.ollieen.com
- **Code:** https://github.com/ollie81/Evorien
- **One line:** A platform where people build a skills "Passport", find collaborators and work together on real projects.
- **Implemented in the codebase:** Passport onboarding; "For You" member matching; projects, opportunities and an apply/accept/reject loop; contributions, connections, notifications and an admin panel; Row Level Security on every table; an "Ask Ollieen AI" assistant that only reads data and never creates a project unless the member clicks to confirm.
- **Stack:** Next.js, TypeScript, Tailwind, Supabase, Vitest.
- **Status: in development.** Unit tests cover its core logic. Ollieen AI only works when an OpenAI key is configured on the deployment, so don't claim it is on for every visitor unless you've checked.

### 4. Day-2: codebase analysis and maintenance tool
- **Live:** https://day-2-steel-eight.vercel.app
- **Code:** private repository (don't share code or internals)
- **One line:** A tool that scans GitHub repositories, scores their health, explains issues in plain language and proposes fixes as pull requests for a human to review.
- **Implemented in the codebase:** deterministic checks plus validated AI analysis; health scoring between scans; AI-generated patches on a separate branch; a Change Simulator for multi-repository risk.
- **Stack:** Next.js, TypeScript, Supabase, GitHub API, Zod, Vitest.
- **Status: in development.** Verified with unit tests only. **The full workflow (GitHub sign-in, live scans, AI fixes, pull requests) has not been validated end-to-end with real accounts.** Share it as a preview, not a finished product. Billing is not implemented.

### 5. The Village That Remembers: Godot 4.3 Android village game
- **Live:** no public build
- **Code:** https://github.com/ollie81/THE-VILLAGE-THAT-REMEMBERS
- **One line:** A 3D village life sim where five villagers have their own routines and remember every conversation with you.
- **Implemented:** procedural low-poly world, day/night cycle, rigged and animated characters, villager memory saved between sessions, touch controls and graphics presets.
- **Stack:** Godot 4.3, GDScript, Android.
- **Status: Milestone 1 playable.** The repository documents passing headless test suites. **Not yet verified on a real Android device**, and the APK export is untested. Say "early prototype".

---

## Message templates

Replace anything in `[brackets]` before sending.

### Short intro (DM / LinkedIn, under 600 characters)
> Hi [Name], I'm an independent software builder working on AI-powered apps. My main project is VIYO (https://viyo.site/app), a video and creator platform with AI-assisted creation tools, currently in active development. I also build Ollie, an AI companion (https://www.ourollie.space), and Ollieen, a collaborator-matching platform (https://www.ollieen.com). More here: https://portfolio-kappa-ebon-cjtxzh45c6.vercel.app/. I'd love to [reason for reaching out].

### Email
> **Subject:** [Topic], independent builder of VIYO and Ollie
>
> Hi [Name],
>
> I'm an independent software builder working across mobile apps, AI integrations, backends and video platforms. I'm reaching out because [reason].
>
> A few things I've built:
> - **VIYO** (https://viyo.site/app): a video entertainment and creator platform with drama discovery and AI-assisted creation tools. In active development.
> - **Ollie** (https://www.ourollie.space): an AI companion with chat, memory and daily check-ins, on Android and the web.
> - **Ollieen** (https://www.ollieen.com): a platform for finding collaborators and building projects together.
> - **Day-2** (https://day-2-steel-eight.vercel.app): an early-stage tool for analysing and maintaining codebases.
> - **The Village That Remembers**: a Godot 4.3 Android game prototype. Code: https://github.com/ollie81/THE-VILLAGE-THAT-REMEMBERS
>
> Portfolio: https://portfolio-kappa-ebon-cjtxzh45c6.vercel.app/
> GitHub: https://github.com/ollie81
>
> [Ask / next step]
>
> Thanks,
> Olivier
> olli1234x@gmail.com

---

## Wording to avoid

| Don't say | Say instead |
|---|---|
| "VIYO generates AI films for users" | "VIYO includes an AI-assisted drama and film creation workflow (in development)" |
| "VIYO's payments are live" | Don't mention payments unless you have verified a real transaction |
| "Day-2 automatically fixes your code" | "Day-2 proposes fixes as pull requests for a human to review (early preview)" |
| "The game is on Android" | "An Android game prototype built in Godot 4.3" |
| Any user numbers, revenue or client names | Only cite numbers you can show |
