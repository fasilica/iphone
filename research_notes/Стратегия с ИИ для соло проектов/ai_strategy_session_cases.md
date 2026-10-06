# Real-world cases of founders, solo entrepreneurs, executives and small teams running strategy sessions "1:1 with AI" (RU + EN), with recurring patterns, failure modes and mitigations

> **Research conditions (read first).** Date of research: 2026-10-06.
> - The network egress proxy blocked direct page reads for YouTube, Telegram (t.me), vc.ru, Habr, Substack, Every.to, Lenny's Newsletter, Medium, X/Twitter, Reddit, Fast Company, tgstat and most vendor blogs. Full-page reads were only possible for **GitHub** and **platform.claude.com**.
> - So for most cases, the details come from **search-engine result summaries**, not from reading the full page. These are marked **[SS]**. Treat [SS] details as leads and check them against the original before quoting them publicly. Items marked **[FULL]** were read in full from the primary source.
> - The web-search budget is shared across parallel research agents, and it ran out partway through this task. Reddit, Hacker News, LinkedIn, YC founder posts and Anthropic/OpenAI customer stories were therefore **not covered** (see Gaps).
> - Details of the trigger video come from the coordinator's brief, based on the user watching it. They were not verified independently, because YouTube could not be reached.

## Q1. Who is the author of the trigger video (youtube.com/watch?v=r5kc7AMTEJE), and are his guide, prompt, slides or a write-up public?

### Takeaway
I could not identify the author ("Kirill"), his company or his Telegram channel. YouTube and every mirror tried were blocked, and searches on the video ID and on distinctive phrases returned nothing relevant. No public guide, prompt or slides were found. The video does name two components, Ivan Zamesin's Next Move Theory skills and obra/superpowers' brainstorming skill, and both are public on GitHub. They are summarised below.

### Cited Findings
- **The video, as described in the coordinator's brief (not independently verified).** A solo founder called Kirill, ex-corporate, about 1.5 years as a founder, runs an AI services/agency business with no co-founder. He argues that external facilitators lack "skin in the game" (Taleb) and that teams suffer from subordination bias, so he ran a multi-day strategy session 1:1 with Claude ("Fable 5" at max effort). His setup:
  - a project folder plus a "state file";
  - a starting prompt casting Claude as a "McKinsey senior partner with 20 years of experience" who asks many questions to design the session;
  - Zamesin's Next Move Theory canon/skills and the obra/superpowers brainstorming skill;
  - connections to Bitrix CRM, ERP, bank and payroll;
  - about 1.5 years of sales-call transcripts analysed by parallel agents;
  - a Miro board for artifacts.

  The session ran in seven stages (diagnostics → anti-crisis stress test → segments and jobs → challenge map and hypotheses → scenarios → bets → synthesis), 1–3 days per stage at about an hour a day. His rule was that AI never makes judgment-heavy decisions. He describes mitigations against the AI fitting his pet ideas, losing context, tiring him out and jumping to solutions. He promised a guide, prompt and slides via a Telegram bot. — [YouTube video](https://www.youtube.com/watch?v=r5kc7AMTEJE) (content per brief)
- Searches for the video ID `r5kc7AMTEJE` returned no indexed pages that mention it. — [search attempt, no hit](https://www.youtube.com/watch?v=r5kc7AMTEJE)
- "Claude Fable 5" is a real Anthropic model in 2026. Russian coverage exists on Habr ("Claude Fable 5: разработчикам важны не только бенчмарки…", "Как правильно заLOOPить Fable 5", "как Mythos стал Fable 5"), and vc.ru reported "Доступ к Fable 5 продлён, лимит 50% от сессии" [SS]. — [Habr 1046736](https://habr.com/ru/articles/1046736/); [Habr 1046451](https://habr.com/ru/articles/1046451/); [Habr 1045814](https://habr.com/ru/articles/1045814/); [vc.ru](https://vc.ru/typespace/3024262-dostup-k-fable-5-prodljon)
- Anthropic's own prompting guide says Fable 5 "is particularly effective at end-to-end work that takes a person hours, days, or weeks", sustains "multiday, goal-directed runs with strong instruction retention", and is "significantly more dependable at dispatching and sustaining parallel subagents". This supports the feasibility of Kirill's multi-day, parallel-agent setup. The guide compares Fable 5 with Opus 4.8. It does not mention an "Opus 5", so the brief's "Opus 5" label may be a mis-hearing. [FULL] — [Prompting Claude Fable 5, Anthropic docs](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5)
- **Component 1: Next Move Theory Canon & Skills (Ivan Zamesin).** A Claude Code/Codex plugin with seven user-invocable skills:
  - `nmt-chat`: an advisor for "product, strategy, segmentation, value, pricing, growth, positioning, B2B" questions, grounded in the canon;
  - `nmt-diagnose`: risks and growth points of a live product;
  - `nmt-market-research`: sizes markets and scores segments with GO/NARROW/PIVOT verdicts;
  - `nmt-craft-value-proposition`;
  - `nmt-product-requirements`;
  - `nmt-craft-go-to-market`;
  - `nmt-analyze-interviews`: extracts AJTBD structure from interview files;
  - plus `nmt-update`.

  The repo had 403 stars and 120 forks, and was at "v0.6 toward 1.0". Install is a one-line curl script. [FULL] — [GitHub zamesin/Next-Move-Theory-Canon-and-Skills](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills)
- Next Move Theory is built on Advanced JTBD and is described as giving "step-by-step algorithms for any product tasks", to "see all tactical and strategic moves available" and choose the best strategy [SS]. — [README](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills/blob/main/README.md)
- **Component 2: obra/superpowers `brainstorming` skill.** Its rules:
  - "Only one question per message";
  - "Prefer multiple choice questions when possible";
  - a "Hard Gate": no implementation before the chosen path's prerequisites are done and approved;
  - three paths (Spike / Bounded / Architectural);
  - the validated design is written to a dated spec file, then self-reviewed for "placeholders, contradictions, scope, and ambiguity" before user review.

  [FULL] — [obra/superpowers brainstorming SKILL.md](https://raw.githubusercontent.com/obra/superpowers/main/skills/brainstorming/SKILL.md)

### Inferences
- Kirill's stack (state file + domain-method skills + a questioning skill with a hard gate + parallel subagents) matches what Anthropic recommends for Fable 5. The guide advises giving the model a memory file, delegating to subagents, and checking claims against tool results. This looks like a deliberate, tool-literate setup, not ad-hoc chatting.
- The Next Move Theory skills explain part of his stage design. The stages "segments and jobs from interviews" and "challenge map and hypotheses" map onto `nmt-analyze-interviews`, `nmt-market-research` and `nmt-diagnose`. The stages "scenarios", "bets" and the anti-crisis stress test seem to be his own additions or the "McKinsey partner" persona's.

### Gaps
- Author's surname, company, Telegram channel/bot and publication date are unknown. YouTube, noembed, Invidious and t.me were all blocked by egress, and search did not index the video. **Recommendation:** open the video description manually and follow the Telegram-bot link to get the guide, prompt and slides.
- It is unknown whether the promised guide, prompt and slides have been released.

## Q2. Other Russian-language cases (Telegram, vc.ru, Habr, YouTube, 2025–2026) of founders/CEOs doing strategy, стратсессия, diagnostics or planning with Claude/ChatGPT

### Takeaway
I found no other public Russian-language write-up of a solo founder's full multi-day strategy session with AI comparable to Kirill's. What exists falls into four groups:
1. builder and founder posts on Habr/vc.ru showing the building blocks: state files, `/insights` self-diagnosis, two-model strategy debates, agent teams with strategy kept in files;
2. facilitators using ChatGPT to prepare or critique human strategy sessions;
3. one-off ChatGPT participation in a company workshop;
4. a growing commercial market of "стратсессия с ИИ" offerings and prompt packs.

### Cited Findings
- **vc.ru, "«2 988 команд и 0 стратегии»: Как Claude Code «прожарил» мой стиль работы и почему это важно для YC" (founder; author not identified).** The founder ran Claude Code's `/insights` analysis over their own usage logs. Its verdict: "2 988 вызовов bash-команд. Почти ноль стратегических сессий" and "Ты используешь Claude как руки на максимум. Но как мозг — на минимум". The article frames this as the "Executor trap" (Manager → Manual Laborer) and as relevant to a YC application [SS]. — [vc.ru 2752858](https://vc.ru/ai/2752858-kak-claude-code-izmenil-moy-podhod-k-rabote)
- **Habr, "Одна AI-голова — хорошо, а две — от разных вендоров лучше. Как заставить Claude и Codex спорить между собой"** (author's GitHub handle: biyachuev).
  - Habr summary [SS]: the `/strategy-debate` skill has Claude and Codex form positions independently, then attack each other's weak points in cross-critique rounds. Each round requires concrete counter-arguments, and a user-chosen finaliser summarises. It is recommended for business strategy and planning.
  - Repo [FULL]: three skills, `strategy-debate`, `creator-critic` and `options-challenge`. Example: `/strategy-debate Topic: Should we target SMB or enterprise first? Constraints: team of 6, need fast feedback loops.` Rationale: "Different training data, different blind spots, structured disagreement that surfaces what one model alone would miss."

  — [Habr 1019494](https://habr.com/ru/articles/1019494/); [GitHub biyachuev/claude-debate-skills](https://github.com/biyachuev/claude-debate-skills)
- **Habr, "Команда агентов в Claude Code: от задачи до релиза".** A solo builder runs a 12-role agent team. Strategy, the hypothesis backlog and weekly reports drive a weekly cycle, and strategy "lives in files": decisions not written to files do not exist for the next cycle. As of September 2026 the repo held 14 role-based agent teams, 73 ADRs, 37 failure-diagnosis ("грабли") files, 331 test cases, 110 analysed bugs and **6 weekly business-cycle reports** [SS]. — [Habr 1086832](https://habr.com/ru/articles/1086832/)
- **Habr, "Как Claude Code раскопал моё кладбище пет-проектов" (about late September 2026).** A developer with 20 years' experience had about ten neglected projects. Claude Code cut work that took a week to a day. Between sessions, a **state file** records the current task, branch and next step, and is passed to Claude with recent commits at the start of each session [SS]. — [Habr 1084508](https://habr.com/ru/articles/1084508/)
- **vc.ru, "Как я использую ИИ — апдейт спустя три года" (personal experience).** The author narrowed to one tool, Claude at $20/month, and says the hard part is choosing which tasks to bring AI into, not choosing the tool. Their workflow: dictate ideas via voice-to-text (Whisper/Wispr Flow), then have Claude structure, rephrase and "analyze for missing points" [SS]. — [vc.ru 2808426](https://vc.ru/life/2808426-ispolzovanie-ii-v-rabote-opyt-za-dva-goda)
- **Sergey Bulaev (vc.ru).** He connected Claude Code to **Bitrix** and built a BI report on sales conversion; the agent diagnosed problems and implemented a fix without extra instructions. He also describes Claude Code extending its own tools through MCP (Linear) [SS]. — [vc.ru Bulaev](https://vc.ru/sergiobulaev/2214023-claude-code-agent-samostoyatelno-razvivaet-sebya)
- **Ivan Zamesin's Telegram.** A post describes using Claude Code to refine his methodology quickly. His GitHub repo turns the methodology into strategy and product skills (see Q1) [SS]. — [t.me/s/zamesin](https://t.me/s/zamesin?before=2522)
- **Telegram "Нестыдная фасилитация" (facilitator community) and vc.ru/Habr facilitation posts.** Facilitators use ChatGPT as a working tool: they send screenshots of Miro session plans and ask it to find weak spots and risks from a facilitation standpoint. In one case ChatGPT saved time preparing a team session, including an express brief for the client [SS]. — [t.me/s/no_shame_facilitation](https://t.me/s/no_shame_facilitation?before=829)
- **HR Bazaar case, "Миссия и ценности компании: кейс нейросетей".** ChatGPT took part in a session alongside company employees. It produced a broader and deeper target-audience analysis, with categories the owners had not mentioned [SS]. — [hrbazaar.ru](https://hrbazaar.ru/articles/missiya-i-czennosti-kompanii-kejs-nejrosetej/)
- **vc.ru, "Claude как бизнес-советник: 6 промптов для основателя стартапа".** A prompt set covering idea validation, first customers, pricing, cold outreach, planning and decision-making [SS]. — [vc.ru 2966616](https://vc.ru/ai/2966616-claude-kak-biznes-sovetnik-prompty-dlya-osnovatelya-startapa)
- **YouTube masterclass, "Стратегическая сессия: как подготовить и провести (+с помощью ИИ) / Формула прорыва" (2024 festival; speaker not verified).** — [YouTube](https://www.youtube.com/watch?v=1ONW1xqRDEY)
- **RBC Style, "Claude: как применяют ИИ в бизнесе".** Denis Kulik, owner of a construction company with no IT background, built a budgeting portal in two days: project managers enter plans and finance sees the summary. This is a data foundation for planning, not a strategy session [SS]. — [style.rbc.ru](https://style.rbc.ru/life/69d609399a7947241b81d7c0)
- **Russian commercial offerings (market signals, not cases):**
  - "Стратегическая сессия с ИИ за 1 день" (Minsk, Aug 2026): a day with an expert and an AI producing 15+ strategy documents, "strategy for a year in one day instead of months" (vendor claim) [SS] — [strateg.aipeople.by](https://strateg.aipeople.by/)
  - [neiroseti.ai/strat_session](https://neiroseti.ai/strat_session)
  - [support-partners.ru course](https://support-partners.ru/courses/ai-strategy-sessions/)
  - OKR Academy, "ИИ на стратегических сессиях: как использовать ИИ, не потеряв лидерство и здравый смысл" — [okr-academy.ru](https://okr-academy.ru/ai_strategic_sessions)
  - CEO annual-strategy prompt generator — [edugusarov.com](https://edugusarov.com/ru/prompty-dlya-generalnogo-direktora-strategiya-kompanii/)
  - "Ваша стратегия на 2025 год с ChatGPT" — [vc.ru 1739214](https://vc.ru/chatgpt/1739214-vasha-strategiya-na-2025-god-s-chatgpt)
- **HSE Graduate School of Business strategy session on AI.** It produced 190+ hypotheses on how AI will affect industries. This is a human strategy session about AI, not clearly one facilitated by AI [SS]. — [gsb.hse.ru](https://gsb.hse.ru/news/945273140.html)

### Inferences
- Russian-language material is strong on **tooling and engineering practice**: state files, skills, two-vendor debate, agent teams. It is weak on **documented strategy-session outcomes**. Kirill's video looks unusual in combining methodology (Next Move Theory) with business-system integration (Bitrix, ERP, bank) and a staged session design.
- Bitrix + Claude Code integration is already practised in the Russian market (Bulaev). Kirill's "AI connected to Bitrix CRM" is therefore reproducible for clients, not exotic.
- The commercial "стратсессия с ИИ за 1 день" offerings sell speed (a year's strategy in a day). That runs against Kirill's slow cadence (an hour a day, over weeks), which is a positioning opportunity for a facilitator.

### Gaps
- Telegram channels could not be read directly (egress). No tgstat search was possible. Channels likely to hold cases were not checked: AI Mindset, Ilya Krasinsky, product/founder channels.
- No Russian podcast case was found.
- Author identities for the vc.ru "2 988 команд" and Habr 1084508/1086832 pieces were not extracted.

## Q3. English-language cases: founders/CEOs using AI as strategy partner, AI board of advisors, AI co-founder, personal operating system, pre-mortems and red-teaming

### Takeaway
English-language practice has settled into a few reusable patterns:
- **AI boardrooms / advisory panels** (Allie K. Miller's `/boardroom`, persona-file "Decision Panels");
- **forcing-question office-hours skills** (Garry Tan's gstack `/office-hours`, `/plan-ceo-review`);
- **thinking-partner agents that are forbidden to write drafts** (Noah Brier / Alephic, on Every's podcast);
- **folder + CLAUDE.md "CEO operating systems"** with plan-first gates and weekly review rituals;
- **mass analysis of sales-call transcripts** (Matt Britton, Suzy).

Pre-mortem prompting dates back to Ethan Mollick's 2023 GPT-4 prompt. Documented outcomes are rarely reported beyond anecdotes.

### Cited Findings
- **Allie K. Miller (AI advisor; X post, 11 Feb 2026).** She built a `/boardroom` Claude Code slash command (`~/.claude/commands/boardroom.md`). It spins up six agents, each role-playing a business leader whose strategic thinking she admires.
  - Round 1: advisors write positions in parallel (about 2 minutes).
  - Round 2: they read each other's actual arguments and debate. "The pricing person attacks the product person… Someone even changes their mind in Round 2."
  - It costs about $5–8 in compute per run and loads her context automatically, so nothing has to be re-explained.
  - Afterwards she reviews the tensions, extracts the conditions, then decides herself.

  She published the full prompt in a follow-up post the same day [SS]. — [X post](https://x.com/alliekmiller/status/2021578555034149188); [prompt post](https://x.com/alliekmiller/status/2021584631082922032); [Steffi Kieffer write-up](https://steffikieffer.substack.com/p/how-to-build-an-ai-boardroom-in-claude); [Fast Company profile](https://www.fastcompany.com/91532032/how-one-worlds-top-ai-voices-uses-claude-code-run-her-day)
- **Noah Brier (co-founder of Alephic, an AI-first strategy consultancy), on Every's "AI & I" podcast with Dan Shipper.**
  - Setup: Claude Code runs on a self-hosted mini-PC (in his basement, behind a VPN) over an Obsidian vault of about 1,500 markdown files, reachable from his phone over SSH.
  - His "Thinking Partner" sub-agent "is explicitly instructed never to produce a draft, outline, or artifact — its job is to ask clarifying questions and log insights". The point is to keep the AI in "thinking mode" rather than writing mode.
  - He argues that LLMs' greatest capability is reading, not writing.

  [SS] — [Every podcast page](https://every.to/podcast/how-to-use-claude-code-as-a-thinking-partner); [transcript](https://every.to/podcast/transcript-how-to-use-claude-code-as-a-thinking-partner); [Apple Podcasts](https://podcasts.apple.com/us/podcast/claude-code-can-be-your-second-brain/id1719789201?i=1000725911151)
- **Dan Shipper (CEO, Every).** Every is described as an AI-native company where "every employee, not just engineers, uses Codex and Claude Cowork as their primary work environment". Shipper's maxim: "Every agent needs a human who cares about it" (Lenny's Podcast, summarised 4 June 2026). On strategy prompting, he advises asking the model to apply a *specific* named framework instead of asking for general strategy advice, which yields generic answers [SS]. — [Gokul Rajaram summary on X](https://x.com/gokulr/status/2062638283100930085); [Section AI, Dan Shipper's 5 best ways](https://www.sectionai.com/blog/5-best-ways-to-use-ai); [Every, Head of Consulting automated her job](https://every.to/podcast/transcript-everys-head-of-consulting-just-automated-her-job)
- **Garry Tan (President & CEO, Y Combinator): gstack (2026, MIT licence, about 135K GitHub stars).**
  - `/office-hours`: "product interrogation before code". In startup mode it asks six forcing questions covering "demand reality, status quo, specificity, narrowest wedge, observation, and future-fit". It then runs a **Premise Challenge** before any solution ("Is this the right problem? What happens if we do nothing?…"), generates three alternative approaches, and writes a design doc.
  - Rules: "One question at a time. Never batch multiple questions"; an anti-sycophancy rule ("premise challenge before solutions… even 'clearly winning' approaches require explicit user approval"); every session ends with a mandatory concrete "assignment"; completion states are DONE / DONE_WITH_CONCERNS / NEEDS_CONTEXT.
  - `/plan-ceo-review` rethinks a plan in four scope modes: Expansion, Selective Expansion, Hold Scope, Reduction.

  [FULL] — [GitHub garrytan/gstack](https://github.com/garrytan/gstack); [office-hours SKILL.md](https://raw.githubusercontent.com/garrytan/gstack/main/office-hours/SKILL.md)
- **Ethan Mollick (Wharton, 12 Oct 2023).** He shared a GPT-4 prompt that "walk[s] you through the process of conducting a pre-mortem", calling decision and management support "one of the biggest opportunities for LLMs". On 2 Oct 2026 he posted that many senior leaders "are absolutely getting AI", but "changing a company is a longer process" [SS]. — [X pre-mortem post](https://x.com/emollick/status/1712488528364396953); [X, Oct 2026](https://x.com/emollick/status/2106097018129227918)
- **"The CEO's Claude Code Setup: A Plan-First, Audit-Ready Operating System" (Medium; author handle "haris", identity unverified).** A CEO made Claude Code their main thinking partner for three months. A top-level `CLAUDE.md` holds rules every session sees: a "plan-first gate", where code lives, **where strategy lives**, a **Friday review ritual**, and a number-reporting rule [SS]. — [Medium](https://haris-31479.medium.com/the-ceos-claude-code-setup-a-plan-first-audit-ready-operating-system-you-can-copy-it-in-30-60fe9bff5e65)
- **Iwo Szapar, "Claude Code for Founders" guide.** It calls planning "the highest-ROI workflow" and has Claude Code write each plan to a named, dated file, so that "six months later you can point Claude at it". A related founder setup keeps an `HQ/` directory with its own `CLAUDE.md` to "run their week, not just their repo". It is unclear whether the `HQ/` setup belongs to this guide or to the Medium "chief of staff" article [SS]. — [iwoszapar.com guide](https://www.iwoszapar.com/resources/claude-code-founder-guide); [Medium, "I turned Claude Code into my chief of staff"](https://medium.com/data-science-collective/i-turned-claude-code-into-my-chief-of-staff-one-folder-6-skills-7a8797ddca25)
- **Matt Britton (CEO, Suzy), on Lenny's "How I AI" with Claire Vo.** He turned "25,000 hours of sales calls into a self-learning GTM engine" [SS; episode details not read]. — [Lenny's Newsletter](https://www.lennysnewsletter.com/p/this-week-on-how-i-ai-0-to-1-ai-guide)
- **AI advisory board / "Decision Panel" write-ups (2026).**
  - A "Decision Panel" is built as a custom Claude skill with **eight experts**, each defined by a detailed persona file (about 40 lines) covering worldview, priorities, the questions they ask, "where they'd push back, and where they might be wrong for your specific situation".
  - Example personas: Paul Graham ("allergic to bullshit"); Brené Brown (values and boundaries).
  - Caveat in the same material: "this setup isn't a replacement for a real board, real mentors, or real advisors".
  - Attribution among the three sources (George Fox University blog June 2026, ProductMindLab, Nikki Cochrane) is uncertain [SS].

  — [George Fox Univ. "How to Build an AI Board of Advisors"](https://www.georgefox.edu/bruin-blog/posts/2026/06/ai-board-of-advisors/index.html); [ProductMindLab](https://productmindlab.substack.com/p/building-an-ai-powered-advisory-board); [Nikki Cochrane, "My AI advisory board met without me"](https://nikcochrane.substack.com/p/my-ai-advisory-board-met-without)
- **Dave Hutch.** A Claude skill runs every content idea through a five-seat board of AI advisors before he records. It acts as a stand-in for friends who give "brutal, unflinching honesty" [SS]. — [nowbam.com](https://nowbam.com/this-claude-skill-builds-you-a-5-seat-board-of-advisors-before-you-hit-record/)
- **Claude Cowork as an executive "chief of staff".** One mid-sized-company executive runs Cowork with 15 scheduled background tasks, 11 function-specific sub-agents dispatched through a "delegation matrix", and about 200 curated markdown memories. Vendor blogs claim CEOs recover 15–20 hours a week, with the executive keeping "full control over strategy and judgment". These are consultancy marketing claims of low reliability, and the named executive was not identified [SS]. — [claudeimplementation.com](https://claudeimplementation.com/blog/claude-cowork-ceo-workflows); [shno.co](https://www.shno.co/blog/claude-cowork-use-cases)
- **Tom's Guide test.** A journalist invented a hula-hoop company and tested ChatGPT, Claude and Gemini as business advisors to see which they would "hire". This is a comparative test, not a real business [SS; verdict not read]. — [Tom's Guide](https://www.tomsguide.com/ai/i-created-a-fake-hula-hoop-company-to-test-chatgpt-claude-and-gemini-heres-the-one-id-actually-hire)
- **Lenny's "How I AI" leads not read in full:** "How a solo founder used Codex & ChatGPT to launch a fashion brand without engineers" and "How this PM uses Claude to handle 70% to 80% of his workday". — [solo founder episode](https://www.lennysnewsletter.com/p/how-i-ai-how-a-solo-founder-used); [PM episode](https://www.lennysnewsletter.com/p/how-i-ai-how-this-pm-uses-claude)
- **Anthropic's open-source `knowledge-work-plugins` for Cowork/Claude Code** (about 26.2K stars) includes Product Management, Sales, Data and Finance plugins with connectors (HubSpot, Close, Fireflies, Snowflake, Notion and others). It has **no dedicated founder, executive or strategy plugin**. [FULL] — [GitHub anthropics/knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins)

### Inferences
- The English-speaking ecosystem has turned "strategy with AI" into **reusable skills and commands** (`/boardroom`, `/office-hours`, `/plan-ceo-review`, `/strategy-debate`) rather than one-off sessions. A facilitator product could package a staged session the same way, as a skill pack plus a state file.
- No vendor plugin targets founder or strategy work, and a YC-backed skill (gstack) aims at *product* scoping rather than company strategy. Company-level strategy for solo and small AI-native teams therefore looks under-served in packaged form.
- Of all the English cases found, Matt Britton's (Suzy) is the closest analogue to Kirill's "1.5 years of sales calls via parallel agents".

### Gaps
- Reddit (r/ClaudeAI, r/Entrepreneur, r/startups), Hacker News, LinkedIn, Indie Hackers and YC founder threads were not reached (search budget/egress). Personal "I ran our annual plan with Claude" stories from those communities are missing.
- Anthropic/OpenAI customer stories about executive strategy use were not checked.
- Few English cases report *business outcomes* (revenue, decisions kept or reversed). Most report process and time saved.

## Q4. Case catalog with per-case details

### Takeaway
There are 24 entries below. About 10 are substantive cases with process detail: RU-1, RU-3, RU-4, RU-5, RU-6, EN-1, EN-2, EN-4, EN-7, EN-10. The rest are tooling or prompt patterns, facilitator-side uses, or leads. Reported outcomes are scarce everywhere. Confidence tags: [FULL] means read in full; [SS] means from a search summary; [BRIEF] means from the coordinator's brief.

### Cited Findings
**Russian-language**

| # | Who / date | Context | Tools & data | Process / prompts / roles | Artifacts & outcomes | Problems & lessons | Source |
|---|---|---|---|---|---|---|---|
| RU-1 | "Kirill", solo founder; 2026 [BRIEF] | Services/AI agency, no co-founder, ex-corporate, about 1.5 years in | Claude (Fable 5, max effort); Bitrix CRM, ERP, bank, payroll; about 1.5 years of call transcripts processed by parallel agents; Miro | Folder + state file; "McKinsey senior partner, 20 yrs" persona that designs the session by questioning; 7 stages, 1–3 days each, about 1 h/day; NMT skills + superpowers brainstorming | Miro board of artifacts; promised guide, prompt and slides | Mitigations against fitting to pet ideas, context loss, fatigue, solution-first; AI never makes judgment calls | [YouTube](https://www.youtube.com/watch?v=r5kc7AMTEJE) |
| RU-2 | Ivan Zamesin; 2025–26 [FULL] | Product/strategy methodologist (AJTBD → Next Move Theory) | Claude Code/Codex plugin; interview files | `nmt-chat` advisor, `nmt-diagnose`, `nmt-market-research` (GO/NARROW/PIVOT), `nmt-analyze-interviews` | 403★/120 forks; v0.6 | Each skill reads the canon at runtime to ground output in the method (canon-grounding) | [GitHub](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills) |
| RU-3 | Founder applying to YC; vc.ru [SS] | Builder-founder | Claude Code `/insights` over own logs | AI audits *how the founder uses AI* | Verdict: "2 988 bash calls, almost zero strategy sessions" | "Executor trap": AI used as hands, not brain | [vc.ru](https://vc.ru/ai/2752858-kak-claude-code-izmenil-moy-podhod-k-rabote) |
| RU-4 | biyachuev; Habr [SS] + GitHub [FULL] | Builder; example "team of 6" | Claude Code + Codex plugin | `/strategy-debate` (independent positions → cross-critique rounds → finaliser); `/creator-critic`; `/options-challenge` | Synthesis by the chosen finaliser | Two vendors means different blind spots | [Habr](https://habr.com/ru/articles/1019494/); [GitHub](https://github.com/biyachuev/claude-debate-skills) |
| RU-5 | Habr author; to Sept 2026 [SS] | Solo human + 12-role agent team | Claude Code agent teams | Weekly cycle driven by strategy file + hypothesis backlog + weekly report | 6 weekly business-cycle reports; 73 ADRs; 37 failure ("грабли") files | "Decisions not written to files don't exist for the next cycle" | [Habr 1086832](https://habr.com/ru/articles/1086832/) |
| RU-6 | Habr author (20-yr developer); about Sept 2026 [SS] | About 10 neglected pet projects | Claude Code | State file (task, branch, next step) + recent commits loaded at session start | Week→day, day→hour speed-up | Session memory carried in a file | [Habr 1084508](https://habr.com/ru/articles/1084508/) |
| RU-7 | vc.ru author; 2025–26 [SS] | Individual professional | Claude ($20) + voice dictation | Dictate theses → Claude structures them and finds missing points | n/a | Choosing the tasks matters more than choosing the tool | [vc.ru](https://vc.ru/life/2808426-ispolzovanie-ii-v-rabote-opyt-za-dva-goda) |
| RU-8 | Sergey Bulaev; vc.ru [SS] | Consultant/entrepreneur | Claude Code + Bitrix, Linear MCP | Agent builds a conversion BI report and self-diagnoses issues | BI report | Precedent for CRM-connected diagnostics | [vc.ru](https://vc.ru/sergiobulaev/2214023-claude-code-agent-samostoyatelno-razvivaet-sebya) |
| RU-9 | Facilitators ("Нестыдная фасилитация"); 2025–26 [SS] | Human-team strategy sessions | ChatGPT + Miro screenshots | AI critiques the session plan for weak spots and risks; drafts the client brief | Time saved in preparation | AI as the facilitator's sparring partner, not the facilitator | [Telegram](https://t.me/s/no_shame_facilitation?before=829) |
| RU-10 | HR Bazaar case [SS] | Company mission/values workshop | ChatGPT | ChatGPT takes part alongside employees | Broader target-audience categories than the owners had named | AI widens the option space (divergence) | [hrbazaar.ru](https://hrbazaar.ru/articles/missiya-i-czennosti-kompanii-kejs-nejrosetej/) |
| RU-11 | vc.ru prompt pack [SS] | Startup founders | Claude | 6 prompts: validation, first customers, pricing, outreach, planning, decisions | n/a | Prompt-pack genre | [vc.ru](https://vc.ru/ai/2966616-claude-kak-biznes-sovetnik-prompty-dlya-osnovatelya-startapa) |
| RU-12 | Denis Kulik; RBC Style [SS] | Construction company owner | Claude | Built a budgeting portal in 2 days | Plan/actuals visible to finance | A data foundation for planning | [RBC Style](https://style.rbc.ru/life/69d609399a7947241b81d7c0) |

**English-language**

| # | Who / date | Context | Tools & data | Process / prompts / roles | Artifacts & outcomes | Problems & lessons | Source |
|---|---|---|---|---|---|---|---|
| EN-1 | Allie K. Miller; 11 Feb 2026 [SS] | Solo AI advisor/business | Claude Code slash command; her context files | `/boardroom`: 6 personas of admired leaders; round 1 parallel, round 2 debate | Explicit tensions and conditions; she decides; about $5–8 per run | Personas really disagree and change minds; the human makes the final call | [X](https://x.com/alliekmiller/status/2021578555034149188) |
| EN-2 | Noah Brier, Alephic; 2025 (exact date uncertain) [SS] | Founder of a strategy consultancy | Claude Code + Obsidian (about 1,500 notes), mini-PC, SSH from phone | "Thinking Partner" sub-agent: questions only, logs insights, never drafts | Insight log | Keep AI in "thinking mode"; reading over writing | [Every](https://every.to/podcast/how-to-use-claude-code-as-a-thinking-partner) |
| EN-3 | Dan Shipper, Every; 2025–26 [SS] | AI-native media/software company | Codex, Claude Cowork as primary environment | Ask for named frameworks, not generic advice | n/a | "Every agent needs a human who cares about it" | [Section AI](https://www.sectionai.com/blog/5-best-ways-to-use-ai); [X](https://x.com/gokulr/status/2062638283100930085) |
| EN-4 | Garry Tan, YC; 2026 [FULL] | Founder/builder toolkit | Claude Code skills (gstack) | `/office-hours`: 6 forcing questions → premise challenge → 3 alternatives → design doc → assignment; `/plan-ceo-review` with 4 scope modes | Design docs; completion states | Anti-sycophancy: premise challenge before solutions | [GitHub](https://github.com/garrytan/gstack) |
| EN-5 | Jesse Vincent, obra/superpowers [FULL] | Builder skill library (used by RU-1) | Claude Code skill | One question per message; multiple-choice; hard gate; dated spec + self-review | Spec file | Stops jumping to implementation | [GitHub](https://raw.githubusercontent.com/obra/superpowers/main/skills/brainstorming/SKILL.md) |
| EN-6 | Ethan Mollick; 12 Oct 2023 [SS] | Academic/educator | GPT-4 prompt | AI-guided pre-mortem (prospective hindsight) | n/a | Makes concerns safe to voice | [X](https://x.com/emollick/status/1712488528364396953) |
| EN-7 | "CEO" (Medium, haris); 2026 [SS] | CEO, company not named | Claude Code + CLAUDE.md | Plan-first gate; a "where strategy lives" folder; Friday review; number-reporting rule | Audit-ready plans | Rituals plus rules in CLAUDE.md | [Medium](https://haris-31479.medium.com/the-ceos-claude-code-setup-a-plan-first-audit-ready-operating-system-you-can-copy-it-in-30-60fe9bff5e65) |
| EN-8 | Iwo Szapar guide; 2026 [SS] | Founders | Claude Code | Planning as highest-ROI workflow; dated plan files; `HQ/` folder (attribution uncertain) | Plan files | Retrievable decision history | [iwoszapar.com](https://www.iwoszapar.com/resources/claude-code-founder-guide) |
| EN-9 | Matt Britton, CEO Suzy; 2026 [SS] | Market-research company | AI over 25,000 hours of sales calls | Self-learning GTM engine | n/a (not read) | Closest analogue to RU-1's transcript mining | [Lenny's](https://www.lennysnewsletter.com/p/this-week-on-how-i-ai-0-to-1-ai-guide) |
| EN-10 | AI advisory-board authors; 2026 [SS] | Founders/professionals | Claude skill/Project + persona files | 8-expert "Decision Panel"; about 40-line personas including "where they might be wrong for you" | n/a | "Not a replacement for a real board" | [George Fox](https://www.georgefox.edu/bruin-blog/posts/2026/06/ai-board-of-advisors/index.html); [Cochrane](https://nikcochrane.substack.com/p/my-ai-advisory-board-met-without) |
| EN-11 | Dave Hutch; 2026 [SS] | Content creator/business | Claude skill | 5-seat board vets each idea | n/a | "Brutal honesty" proxy | [nowbam.com](https://nowbam.com/this-claude-skill-builds-you-a-5-seat-board-of-advisors-before-you-hit-record/) |
| EN-12 | Unnamed mid-size-company exec; 2026 [SS] | Executive | Claude Cowork: 15 scheduled tasks, 11 sub-agents, about 200 memories | Chief-of-staff delegation matrix | Claimed 15–20 h/week saved (vendor) | Low reliability; unverified | [claudeimplementation.com](https://claudeimplementation.com/blog/claude-cowork-ceo-workflows) |

### Inferences
- Across sources, a fully documented "multi-day 1:1 strategy session with outcomes" is rare. Kirill's video is one of the few end-to-end examples. Most of the public record is made of **reusable components**.
- Personas in use fall into two kinds. One is a **single senior-consultant persona as session designer** (RU-1's "McKinsey partner"). The other is a **multi-persona panel as critic** (EN-1, EN-10, EN-11, RU-4). A product could combine them: one designer persona plus a critic panel at the convergence points.

### Gaps
- Two further leads could not be filled with checked details: Every's "Head of Consulting automated her job" and the Lenny's solo-founder fashion-brand episode.
- No case reports a strategy chosen with AI and then a measured business outcome six or more months later.

## Q5. Recurring workflow patterns

### Takeaway
Eight patterns recur across RU and EN cases:
1. folder + state/memory file;
2. CLAUDE.md and skills that encode a methodology;
3. connectors to business systems;
4. parallel agents over transcripts or interviews;
5. question-first session design (one question at a time);
6. persona panels and cross-model debate for critique;
7. explicit gates that separate divergence/diagnosis from convergence/solutions;
8. multi-day cadence with weekly review rituals and decisions written to dated files.

### Cited Findings
- **Folder + state/memory file:**
  - RU-1's state file [BRIEF];
  - a state file with task, branch and next step loaded each session — [Habr 1084508](https://habr.com/ru/articles/1084508/);
  - "strategy lives in files" — [Habr 1086832](https://habr.com/ru/articles/1086832/);
  - Anthropic advises "Provide a place to write notes, as simple as a Markdown file… Store one lesson per file… delete notes that turn out to be wrong" — [Anthropic Fable 5 guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **CLAUDE.md as rulebook:** a plan-first gate, where strategy lives, a Friday review — [Medium CEO setup](https://haris-31479.medium.com/the-ceos-claude-code-setup-a-plan-first-audit-ready-operating-system-you-can-copy-it-in-30-60fe9bff5e65); Boris Cherny's (creator of Claude Code) habit of telling Claude to "update CLAUDE.md so this mistake doesn't repeat" [SS] — [vc.ru tips](https://vc.ru/ai/2856744-sovety-ot-osnovatelya-claude-code).
- **Methodology-as-skills:** each Next Move Theory skill "reads the canon at runtime" — [GitHub NMT](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills); gstack chains skills (office-hours writes docs that plan-ceo-review reads) — [gstack](https://github.com/garrytan/gstack).
- **Connectors to business systems:**
  - Bitrix, ERP, bank and payroll in RU-1 [BRIEF];
  - Bitrix BI via Claude Code — [vc.ru Bulaev](https://vc.ru/sergiobulaev/2214023-claude-code-agent-samostoyatelno-razvivaet-sebya);
  - Anthropic's Cowork plugins ship connectors for HubSpot, Close, Fireflies (call transcripts), Snowflake and others — [knowledge-work-plugins](https://github.com/anthropics/knowledge-work-plugins).
- **Parallel agents over transcripts or interviews:**
  - RU-1 [BRIEF];
  - `nmt-analyze-interviews` — [GitHub NMT](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills);
  - 25,000 hours of sales calls — [Lenny's](https://www.lennysnewsletter.com/p/this-week-on-how-i-ai-0-to-1-ai-guide);
  - Fable 5 is "significantly more dependable at dispatching and sustaining parallel subagents" — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Question-first, one question at a time:**
  - superpowers ("Only one question per message", multiple choice preferred) — [SKILL.md](https://raw.githubusercontent.com/obra/superpowers/main/skills/brainstorming/SKILL.md);
  - gstack ("Never batch multiple questions") — [office-hours](https://raw.githubusercontent.com/garrytan/gstack/main/office-hours/SKILL.md);
  - RU-1's "ask me many questions to design the session" [BRIEF];
  - Brier's question-only Thinking Partner — [Every](https://every.to/podcast/how-to-use-claude-code-as-a-thinking-partner).
- **Personas and panels:**
  - "McKinsey senior partner" [BRIEF];
  - the 6-leader `/boardroom` — [X](https://x.com/alliekmiller/status/2021578555034149188);
  - the 8-expert Decision Panel with persona files — [George Fox](https://www.georgefox.edu/bruin-blog/posts/2026/06/ai-board-of-advisors/index.html);
  - a Claude vs Codex debate — [GitHub biyachuev](https://github.com/biyachuev/claude-debate-skills);
  - McKinsey-persona prompt packs are a common genre (e.g. "McKinsey in 360 Claude Prompts", "The 10 McKinsey Skills, Rebuilt as Claude Prompts") [SS] — [Gumroad](https://kumail.gumroad.com/l/360C); [Substack](https://morsebridge.substack.com/p/the-10-mckinsey-skills-rebuilt-as).
- **Divergence/convergence separation and gates:**
  - the superpowers "Hard Gate" — [SKILL.md](https://raw.githubusercontent.com/obra/superpowers/main/skills/brainstorming/SKILL.md);
  - gstack's Premise Challenge before alternatives, and design docs only — [office-hours](https://raw.githubusercontent.com/garrytan/gstack/main/office-hours/SKILL.md);
  - the boardroom's Round 1 (independent) → Round 2 (debate) — [X](https://x.com/alliekmiller/status/2021578555034149188).
- **Boards and visual artifacts:** Miro in RU-1 [BRIEF]; facilitators feed Miro plan screenshots to ChatGPT for critique [SS] — [Telegram](https://t.me/s/no_shame_facilitation?before=829). Fable 5 interprets dense images and screenshots "with substantially higher accuracy" — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Cadence and rituals:**
  - 1–3 days per stage, an hour a day [BRIEF];
  - weekly business cycle reports — [Habr 1086832](https://habr.com/ru/articles/1086832/);
  - Friday review — [Medium CEO](https://haris-31479.medium.com/the-ceos-claude-code-setup-a-plan-first-audit-ready-operating-system-you-can-copy-it-in-30-60fe9bff5e65);
  - dated plan files retrievable months later — [iwoszapar.com](https://www.iwoszapar.com/resources/claude-code-founder-guide).
- **Mandatory next action:** every gstack office-hours session "ends with a concrete next action… not 'go build it'" — [office-hours](https://raw.githubusercontent.com/garrytan/gstack/main/office-hours/SKILL.md).

### Inferences
- Taken together, these patterns form a de facto "AI strategy session kit". It has four layers: a **memory layer** (state file, CLAUDE.md, dated decision files), a **method layer** (skills such as NMT or office-hours), a **data layer** (CRM, finance and transcript connectors) and a **dialectic layer** (persona panel or cross-model debate). A facilitator's product could be sold as a configured kit plus a human checkpoint at each convergence gate.
- The divergence/convergence split that facilitators know from S3 and classic facilitation is already in these tools (Hard Gate, Premise Challenge, Round 1/Round 2). It is enforced by prompts, though, not by a neutral party, and that is where a human facilitator's role could sit.

### Gaps
- No source compared cadences (one long sitting vs. daily hour-long sessions) for quality of outcome.
- Notion/FigJam use in strategy sessions with AI was not found in the material reached.

## Q6. Reported failure modes and mitigations

### Takeaway
The failure modes named most often are:
- sycophancy / fitting to the founder's preferences;
- generic, framework-free advice;
- context loss across long or multi-day work;
- fabricated status or data in long runs;
- solution-first behaviour;
- over-reliance (AI as decider, or the opposite "AI as hands only" trap).

Mitigations are mostly structural (gates, adversarial panels, memory files, verification against tool results, the human keeping the final judgment) rather than prompt wording. Fatigue was named only in Kirill's video.

### Cited Findings
- **Sycophancy / fitting to pet ideas:**
  - gstack's explicit "Anti-Sycophancy Rule": premise challenge before solutions, and even "clearly winning" approaches need explicit approval — [office-hours](https://raw.githubusercontent.com/garrytan/gstack/main/office-hours/SKILL.md);
  - cross-vendor debate because the models have "different blind spots" — [GitHub biyachuev](https://github.com/biyachuev/claude-debate-skills);
  - multi-persona panels whose personas really disagree — [X Allie Miller](https://x.com/alliekmiller/status/2021578555034149188);
  - persona files that state "where they might be wrong for your specific situation" [SS] — [George Fox](https://www.georgefox.edu/bruin-blog/posts/2026/06/ai-board-of-advisors/index.html);
  - "brutal honesty" boards — [nowbam.com](https://nowbam.com/this-claude-skill-builds-you-a-5-seat-board-of-advisors-before-you-hit-record/).
- **Generic advice:** ask the model to apply a *specific* framework, since the general question yields "a generic way to think about it" [SS] — [Section AI / Shipper](https://www.sectionai.com/blog/5-best-ways-to-use-ai). Ground the model in a methodology canon — [NMT](https://github.com/zamesin/Next-Move-Theory-Canon-and-Skills). Full automation of business plans yields superficial documents, so use ChatGPT as an assistant, not a replacement. The search summary did not say which of these two pages it came from [SS] — [foundor.ai (RU)](https://foundor.ai/ru/blog/can-chatgpt-write-business-plan); [vc.ru 1739214](https://vc.ru/chatgpt/1739214-vasha-strategiya-na-2025-god-s-chatgpt).
- **Context loss across sessions:**
  - state files — [Habr 1084508](https://habr.com/ru/articles/1084508/);
  - "decisions not written to files don't exist" — [Habr 1086832](https://habr.com/ru/articles/1086832/);
  - dated plan files — [iwoszapar.com](https://www.iwoszapar.com/resources/claude-code-founder-guide);
  - Anthropic's memory-file guidance, and bootstrapping memory by having subagents review past sessions — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).

  Anthropic also documents that deep into long sessions Fable 5 can occasionally state an intention without acting, pause for permission it doesn't need, or offer to "summarize and hand off" when the harness shows a remaining-token countdown. The fix is a short "continue" instruction or reassurance text — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Hallucinated or fabricated data and progress:** Anthropic: "Before reporting progress, audit each claim against a tool result from this session… In Anthropic's testing, this nearly eliminated fabricated status reports". It also notes "Separate, fresh-context verifier subagents tend to outperform self-critique" — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Solution-first / premature convergence:**
  - superpowers' Hard Gate — [SKILL.md](https://raw.githubusercontent.com/obra/superpowers/main/skills/brainstorming/SKILL.md);
  - gstack produces design docs only, with Premise Challenge ("What happens if we do nothing?") — [office-hours](https://raw.githubusercontent.com/garrytan/gstack/main/office-hours/SKILL.md);
  - Brier's Thinking Partner "never produce[s] a draft, outline, or artifact" — [Every](https://every.to/podcast/how-to-use-claude-code-as-a-thinking-partner);
  - Anthropic: "When the user is describing a problem… or thinking out loud… the deliverable is your assessment. Report your findings and stop" — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Over-reliance / AI as decider:**
  - Kirill's rule that AI never makes judgment-heavy decisions [BRIEF];
  - Allie Miller extracts conditions, then decides herself — [X](https://x.com/alliekmiller/status/2021578555034149188);
  - "Every agent needs a human who cares about it" — [X/Gokul](https://x.com/gokulr/status/2062638283100930085);
  - an AI board "isn't a replacement for a real board" [SS] — [George Fox](https://www.georgefox.edu/bruin-blog/posts/2026/06/ai-board-of-advisors/index.html).
- **Under-use / "Executor trap":** "2 988 bash calls, almost zero strategy sessions"; "Claude as hands to the maximum, as brain to the minimum" [SS] — [vc.ru](https://vc.ru/ai/2752858-kak-claude-code-izmenil-moy-podhod-k-rabote).
- **Over-planning / re-litigating settled decisions** (relevant to multi-day sessions): Anthropic's suggested instruction: "Do not re-derive facts already established… re-litigate a decision the user has already made… If you are weighing a choice, give a recommendation, not an exhaustive survey" — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Unrequested actions:** Fable 5 "can occasionally take unrequested actions (drafting an email when none was asked for…)"; mitigate with explicit boundaries — [Anthropic guide](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-fable-5).
- **Bias toward one's own thinking style in persona choice (implied):** Allie Miller picks advisors she *admires* — [X](https://x.com/alliekmiller/status/2021578555034149188). This is a possible echo-chamber risk; no source states it explicitly. See Inferences.

### Inferences
- Gates, panels and memory files are all structure, and every prompt-based mitigation is still self-policed by the same model that is being policed. A neutral human (facilitator) or a different-vendor model at the convergence gates is the strongest independent check available. That points to a role for the consultant: a "gatekeeper" at stage transitions rather than a full-time facilitator.
- Choosing panel personas from people the founder admires may recreate the founder's own biases. A facilitator could add deliberately dissonant personas (e.g. a customer, a CFO, a competitor).
- Fatigue ("overtiring") is a human-side failure mode that tool-centred sources ignore. Kirill's one-hour-a-day cadence is the only mitigation seen.

### Gaps
- Academic evidence (field experiments on AI business advice, LLMs evaluating strategic decisions, sycophancy research) was not gathered in this pass. Defer to the science/risk researcher.
- No source quantified how often AI strategy advice was later judged wrong.

## Q7. AI-native teams (small human teams + agents) running team strategy sessions with AI as facilitator

### Takeaway
No public case was found of AI acting as the *lead facilitator* of a human team's strategy session. What exists:
- AI-native teams where agents run a weekly business cycle from a human-owned strategy file (Habr 1086832);
- companies where the whole staff works inside Claude Cowork/Codex (Every);
- AI as a participant or idea-widener in a company workshop (HR Bazaar);
- AI as a sparring partner to the human facilitator before the session (Нестыдная фасилитация).

This is a visible gap, and an opening for an S3 facilitator.

### Cited Findings
- A solo human runs a 12-role agent team on a weekly business cycle (strategy file → hypothesis backlog → weekly report), with 6 weekly cycle reports as of September 2026 [SS] — [Habr 1086832](https://habr.com/ru/articles/1086832/).
- Every: "every employee, not just engineers, uses Codex and Claude Cowork as their primary work environment" [SS] — [Gokul Rajaram on Shipper](https://x.com/gokulr/status/2062638283100930085); [Section AI](https://www.sectionai.com/blog/5-best-ways-to-use-ai).
- ChatGPT took part alongside employees in a mission/values session and widened the audience categories [SS] — [hrbazaar.ru](https://hrbazaar.ru/articles/missiya-i-czennosti-kompanii-kejs-nejrosetej/).
- Facilitators use ChatGPT to critique Miro session plans and prepare client briefs [SS] — [Telegram Нестыдная фасилитация](https://t.me/s/no_shame_facilitation?before=829).
- `/strategy-debate` example framed for a "team of 6" choosing SMB vs enterprise — [GitHub biyachuev](https://github.com/biyachuev/claude-debate-skills).
- A search for "we used Claude to facilitate our company offsite strategy retreat" returned only generic offsite-facilitation guides, with no AI-facilitated cases — [search result example: Ask a Chief of Staff](https://askachiefofstaff.substack.com/p/issue-30-how-to-leverage-strategic).
- Commercial RU offerings pair "an expert + a neural network" for one-day company sessions. This is a hybrid human-facilitator model, not AI-led [SS] — [strateg.aipeople.by](https://strateg.aipeople.by/); [okr-academy.ru](https://okr-academy.ru/ai_strategic_sessions).

### Inferences
- In AI-native teams, "strategy" is becoming a **living file** that agents read every cycle (Habr 1086832), not an annual offsite deck. S3 artifacts (drivers, domains, agreements, review dates) fit naturally as such files, which agents and humans can both read.
- Kirill's subordination-bias argument against team sessions has a counterpart in solo AI sessions: the AI's own deference to the founder (sycophancy). A hybrid helps with both. AI handles divergence and evidence (transcripts, CRM). A human facilitator, or S3 consent-based decision-making with real stakeholders, handles convergence. This is an inference, not a documented case.

### Gaps
- No documented case was found of an AI-native small team (2–10 humans + agents) running a *joint* strategy session with AI as facilitator, nor of S3/sociocracy practice combined with AI facilitation. Reddit, LinkedIn and Anthropic customer stories, the likeliest places for such a case, could not be searched (budget/egress).
