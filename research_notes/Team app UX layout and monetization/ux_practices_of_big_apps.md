# UX practices of big, well-loved apps: evidence, data, and fit for SubOne (team workspace for school racing teams, ages ~11-19, plus teachers/mentors)

Research-status note (read first). Compiled 25 Sep 2026. In this session web search was unavailable (session search budget exhausted) and the network egress proxy blocked most primary domains (nngroup.com, ico.org.uk, europa.eu, ftc.gov, web.dev, w3.org, chameleon.io, userpilot.com, lennysnewsletter.com, research.duolingo.com and others). Only github.com and raw.githubusercontent.com were reachable. Verification therefore used GitHub-hosted primary documents (GitHub Primer, GOV.UK Design System, IBM Carbon, Mailchimp style guide, MDN, Google's web-vitals library, GitHub Docs, an archived copy of the Lenny's Newsletter Duolingo article, paper abstracts) and GitHub code search for verbatim copies of primary sources. Every item carries a tag:
- **[V]** = verified this session against the primary text itself.
- **[C]** = corroborated this session via one or more secondary copies/quotations of the named primary source (primary page not reachable); figures matched prior knowledge.
- **[R]** = recalled from well-established literature/product knowledge; primary URL could not be fetched this session. Verify before quoting publicly.
Evidence type is labelled in brackets (experiment, field study, vendor benchmark, company retrospective, regulator text, design-system guidance/opinion). "Implication for SubOne" lines are the researcher's application of the finding.

## 1. Onboarding and activation: sample data vs blank start, templates, checklists vs tours, progressive onboarding, "aha" and time-to-value

### Takeaway
The best-evidenced practices are: let people see value before committing (sample workspace, no forced registration), keep guided tours very short and user-triggered, teach in context (empty states, first-use hints) rather than with long upfront tutorials, and define activation as a concrete *team* behaviour that predicts retention (Slack's "2,000 messages" is the archetype). Vendor benchmarks put average SaaS activation around 37.5% and average product-tour completion around 61%, but these are correlational vendor numbers, not causal evidence that tours improve activation.

### Cited Findings
- [Vendor benchmark; ~15 million tour interactions] Average product-tour completion is **61%**; completion drops steeply with length (about **72% for 3-step vs 16% for 7-step** tours, values shown in a chart); tours longer than 5 steps lose more than half of users — [Chameleon, Product Tour Benchmarks highlights (2025 restatement of its 15M-interaction dataset)](https://www.chameleon.io/blog/product-tour-benchmarks-highlights) [C]. An independent verification note found only the 61% in the article text; the 72%/16% figures appear only in a chart image — [Vibe-Walk research note](https://github.com/estevanhernandez-stack-ed/Vibe-Walk) [C].
  - Implication for SubOne: cap each guided-tour "chapter" at about 3 steps; offer tours per area (Season, Build, Runs, Sponsors, Portfolio) rather than one long tour.
- [Vendor benchmark] User-triggered ("self-serve") tours launched from a help menu, checklist item or "Show me how" button reached **~67% completion, reported as 123% higher than auto-launched tours** — Chameleon data as summarised in [tour-kit docs](https://github.com/domidex01/tour-kit) [C]. Completion is not activation, and no causal (holdout) test was published.
  - Implication for SubOne: launch tours from the onboarding checklist and a "Show me how" link in each empty state; never auto-play on first load. Judge the tour by whether tour-takers' *teams* activate more, using a small holdout.
- [Vendor benchmark; 547 SaaS companies, 2024] Average new-user activation rate **37.5%** (healthcare products 23.8%). Each company defines "activation" itself, so cross-company comparison is weak — [Userpilot benchmark](https://userpilot.com/blog/healthcare-product-metrics-benchmark-report/) [C].
  - Implication for SubOne: don't benchmark against generic SaaS. Define team activation precisely and track SubOne's own cohort trend by season.
- [Company retrospective, correlational] Slack's founder: "any team that has exchanged 2,000 messages in its history has tried Slack — really tried it"; "after 2,000 messages, 93% of those customers are still using Slack today". He also said "Slack works with just 2 people, but it takes 3 to make it really work" — [First Round Review interview with Stewart Butterfield](https://review.firstround.com/from-0-to-1b-slacks-founder-shares-their-epic-launch-strategy/) [C]. Many retellings add "within the first week", which is not in the quote.
  - Implication for SubOne: pick a team-level activation threshold, e.g. within 14 days ≥3 members joined, a season plan with the competition date, ≥1 car version or part logged, and ≥1 "Today" move completed. Then check against real data which early behaviours predict teams still active at their first competition.
- [Case study, 2009, anecdotal] Replacing a forced "Register" step before checkout with a "Continue" option reportedly raised purchases **45%** ($15M in the first month, $300M in the first year) — [Jared Spool, "The $300 Million Button"](https://articles.centercentre.com/three_hund_million_button/) [R].
  - Implication for SubOne: the no-account sample workspace is well-founded. Ask for an account only when the user wants to save, invite or create their real team.
- [Guidance from qualitative research] Upfront "deck-of-cards" onboarding tutorials are often skipped, quickly forgotten and don't reliably improve task performance; contextual, just-in-time help works better — [NN/g, Onboarding Tutorials vs. Contextual Help](https://www.nngroup.com/articles/onboarding-tutorials/) [R].
  - Implication for SubOne: prefer first-use hints inside each area (e.g., first visit to Runs: "Log your first run: it takes 30 seconds") over a long front-loaded tour.
- [Design-system guidance, GitHub] First-use empty states should "convey the intention of the feature in a way that sounds welcoming and human", offer one primary action, and optionally link to learning resources; secondary text should let users "understand what steps they might take next" — [GitHub Primer, Empty states](https://github.com/primer/design/blob/main/content/ui-patterns/empty-states.mdx) [V]. NN/g likewise says empty states should communicate system status, provide learning cues and give direct pathways to key tasks — [NN/g, Designing Empty States in Complex Applications](https://www.nngroup.com/articles/empty-state-interface-design/) [R].
  - Implication for SubOne: every empty area (no sponsors yet, no runs yet) should say what it is for in racing terms, with one action and a link to a 1-minute example from the sample team.
- [Field experiment; car-wash loyalty cards] Endowed progress: a 10-stamp card with 2 stamps pre-filled was completed by **34%**, against **19%** for an 8-stamp card with none (8 purchases needed in both cases) — [Nunes & Drèze 2006, Journal of Consumer Research](https://doi.org/10.1086/500480) [R].
  - Implication for SubOne: the team setup checklist should start with the items already done ("Team created ✓", "Competition chosen ✓"). Keep it team-shared and task-based, not a badge collection.
- [Company practice] Canva, Notion and Figma make template galleries the default starting point rather than a blank canvas, and Canva and Figma are free for K-12 education — [Canva templates](https://www.canva.com/templates/), [Notion templates](https://www.notion.com/templates), [Canva for Education](https://www.canva.com/education/), [Figma for Education](https://www.figma.com/education/) [R].
  - Implication for SubOne: offer season templates by competition and class (e.g., a regional→national→world-finals timeline with default milestones for portfolio, judged talk and car build), with blank as a secondary option.

### Inferences
- The sample workspace should convert, not just demo. A "Start my team from this template" action should copy the sample's *structure* (milestones, checklists, sponsor pipeline stages) without its data.
- Team products have a two-sided activation problem. The teacher or captain sets up, but value appears only when ≥3 students contribute. Onboarding should therefore push early invitations (class code / invite link), and "Today" should give invitees a concrete first move within their first session.
- Candidate SubOne "aha moments" to test: (a) seeing the car's version history and run results together; (b) the first "since you were last here" summary showing teammates' progress; (c) the race-engineer AI answering a question using the team's own logged runs.
- For 11-13-year-olds, shorter copy and teacher-led setup (teacher creates the team, students join by code) reduce friction and also support under-13 consent requirements (see §2 COPPA).

### Gaps
- Could not verify current first-run flows of Linear, Notion, Figma and Canva (e.g., use-case questions at signup, Linear's seeded "welcome" issues, Notion's "Getting Started" checklist page). These are recalled only, because the product sites were blocked.
- Found no public controlled experiment comparing sample-data vs blank-start activation. The evidence is practitioner consensus plus adjacent findings (Spool, endowed progress).
- Userpilot's widely quoted "average time-to-value" figure, Pendo feature-adoption benchmarks and Appcues checklist data could not be verified.
- Duolingo's reported retention gain from letting learners start a lesson before signup ("gradual engagement") could not be verified.

## 2. Habit and retention without manipulation: the Hook model and critiques, Duolingo's streak/notification experiments, humane-tech frameworks, what regulators forbid or discourage, and which mechanisms are healthy

### Takeaway
Streaks, leaderboards and loss-framed reminders measurably raise engagement: Duolingo's leaderboards added 17% learning time. That power is exactly why regulators now expect such features to be off by default for minors (EU DSA Art. 28 guidelines) and why the UK Children's Code tells services not to use children's data to "incentivise children to stay engaged". Healthy alternatives with better evidence for a school team are progress visibility ("small wins"), concrete next actions with when/where plans, batched recaps, and reminders tied to real team commitments. SubOne's choice of no streaks, points or leaderboards is aligned with regulation and with the motivation research.

### Cited Findings
- [Company retrospective, A/B-tested features] Duolingo (Jorge Mazal, former CPO, Nov 2022):
  - Leaderboards raised "overall learning time... by 17%", and highly engaged learners (≥1 hour/day, 5 days/week) "tripled"; D1/D7 retention improved "with statistical significance". Users "were automatically opted in".
  - Over four years CURR (current-user retention rate) rose **21%**, "a reduction in the daily churn of our best users by over 40%"; together with other bets this produced **4.5x DAU**.
  - The share of DAU with a 7+ day streak rose almost 3x, to more than half of DAU.
  - Source: [Lenny's Newsletter, "How Duolingo reignited user growth"](https://www.lennysnewsletter.com/p/how-duolingo-reignited-user-growth), verified via the [archived text in LennysNewsletter/lennys-newsletterpodcastdata](https://github.com/LennysNewsletter/lennys-newsletterpodcastdata) [V].
  - Implication for SubOne: the mechanics work because they exploit competition and loss aversion. Take the lesson of *designing for existing active users* (a CURR-like "retained active team" metric) without the competitive mechanics.
- [Company practice] Duolingo's notification team could optimise "timing, templates, images, copy, localization... but they could not increase the quantity of notifications without strong justification and CEO approval" — [same article, archived text](https://github.com/LennysNewsletter/lennys-newsletterpodcastdata) [V].
  - Implication for SubOne: adopt a hard per-user notification budget (e.g., ≤1 push/day for students, digest-first) that can only be raised by an explicit, documented product decision.
- [Published algorithm, KDD 2020] Duolingo's notification system is a "sleeping, recovering" bandit. It picks among message templates and applies a recency penalty because repeated messages lose novelty; success is a lesson completed within 2 hours of the notification. Duolingo also analysed ~200M reminders — [Yancey & Settles, KDD 2020](https://research.duolingo.com/papers/yancey.kdd20.pdf) and [Duolingo blog, "Hi, it's Duo: the AI behind the meme"](https://blog.duolingo.com/hi-its-duo-the-ai-behind-the-meme/), both corroborated via a [replication repo](https://github.com/jakemaz66/RecoveringSleepingBandit) [C]. The replication's +1.52% reward over random is the replicator's own result, not Duolingo's.
  - Implication for SubOne: repetition kills attention. Vary digest content and lead with what changed for *this* team; SubOne doesn't need ML for this.
- [Company practice] After repeated ignored reminders, Duolingo sends "These reminders don't seem to be working. We'll stop sending them for now." — [quoted in several teardown documents, e.g., cd-agency case study](https://github.com/adedayoagarau/cd-agency) [C]. The copy is guilt-tinged by design.
  - Implication for SubOne: auto-pause reminders after N ignored ones, but with neutral copy ("We've paused reminders. Turn them back on anytime").
- [Framework and critique] Nir Eyal's Hook model runs Trigger → Action → Variable Reward → Investment; his own "Manipulation Matrix" asks whether the product materially improves users' lives and whether the maker would use it — [Nir Eyal, Hooked](https://www.nirandfar.com/hooked/) [R]. Critics, notably the Center for Humane Technology, argue that variable-reward loops borrow from slot-machine design and that engagement-maximising design harms attention and wellbeing — [Center for Humane Technology](https://www.humanetech.com/) [R].
  - Implication for SubOne: keep the "Investment" part (the team's data compounds in value) and "Triggers" tied to real events; drop variable rewards.
- [Meta-analysis, 128 experiments] Expected tangible rewards contingent on doing, completing or performing a task undermined free-choice intrinsic motivation. Positive verbal feedback enhanced it among college students, but not reliably among children — [Deci, Koestner & Ryan 1999, Psychological Bulletin](https://doi.org/10.1037/0033-2909.125.6.627) [R].
  - Implication for SubOne: supports the no-points design. Give informational feedback about the work ("drag down 4% since v3", "portfolio 80% drafted") rather than rewards.
- [Meta-analysis] Gamification in learning shows small-to-medium average effects (cognitive g≈0.49, motivational g≈0.36, behavioural g≈0.25), moderated by design and context — [Sailer & Homner 2020, Educational Psychology Review](https://doi.org/10.1007/s10648-019-09498-w) [R]. So gamification is not useless, but effects depend on context and are not free of side effects.
- [Diary study; ~12,000 daily diary entries, 238 knowledge workers, 7 companies] Making progress in meaningful work was the most important day-to-day booster of motivation and positive emotion ("the progress principle") — [Amabile & Kramer, "The Power of Small Wins", HBR 2011](https://hbr.org/2011/05/the-power-of-small-wins) [R].
  - Implication for SubOne: "since you were last here" and weekly recaps should lead with team progress (parts made, runs logged, sponsor replies, portfolio pages drafted).
- [Meta-analysis; 94 independent tests] Forming implementation intentions ("if-then", when/where plans) had a medium-to-large effect on goal attainment (d≈0.65) — [Gollwitzer & Sheeran 2006](https://doi.org/10.1016/S0065-2601(06)38002-1) [R].
  - Implication for SubOne: the "one next move per person" on Today is evidence-aligned; add an optional "when" ("Thursday after school") and let the owner pick it.
- [fMRI experiment; n=32 adolescents aged 13-18] Photos shown with more "likes" were more likely to be liked and activated reward circuitry (nucleus accumbens) — [Sherman et al. 2016, Psychological Science](https://doi.org/10.1177/0956797616645673) [R].
  - Implication for SubOne: avoid like counts and individual rankings; if kudos exist, keep them team-internal and without counts.
- [Public-health guidance] The US Surgeon General's advisory (May 2023) calls adolescence (10-19) a highly sensitive period of brain development and flags engagement-maximising design features (e.g., push notifications, autoplay, infinite scroll, like counts) — [HHS advisory PDF](https://www.hhs.gov/sites/default/files/sg-youth-mental-health-social-media-advisory.pdf) [R]. The APA's May 2023 advisory recommends that adolescents' use not interfere with sleep and physical activity and that social comparison be limited — [APA Health Advisory](https://www.apa.org/topics/social-media-internet/health-advisory-adolescent-social-media-use) [R].
- [Regulator text, UK] The ICO Children's Code (Age Appropriate Design Code) has 15 standards, covers services "likely to be accessed" by under-18s, and conformance has been expected since 2 Sep 2021 — [ICO Children's Code](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/age-appropriate-design-a-code-of-practice-for-online-services/) [R].
  - Standard 13 (Nudge techniques): "Do not use nudge techniques to lead or encourage children to provide unnecessary personal data or weaken or turn off their privacy protections." [C/R: the opening phrase was matched in [mukul975/Privacy-Data-Protection-Skills](https://github.com/mukul975/Privacy-Data-Protection-Skills); one secondary copy ends "...or turn off privacy protections", so check the exact ending on ico.org.uk]
  - Standard 5 (Detrimental use of data) guidance says services should: "avoid using personal data in a way that incentivises children to stay engaged"; "present options to continue playing or otherwise engaging with your service neutrally without suggesting that children will lose out if they don't"; "avoid features which use personal data to automatically extend use instead of requiring children to make an active choice"; and "introduce mechanisms such as pause buttons" [C: quoted in [mandyMooreFan/docket, docs/childrens-code.md](https://github.com/mandyMooreFan/docket)].
  - Other standards include high privacy by default (7), data minimisation (8), geolocation off by default (10), parental controls with an obvious sign to the child when monitored (11), and profiling off by default (12) [R].
  - Implication for SubOne: no loss-framed student messaging ("your team will fall behind!"), no auto-extending sessions, and students told clearly what teachers can see (the analogue of standard 11).
- [Regulator text, EU]
  - DSA Art. 25 bars online platforms from interfaces that "deceive or manipulate" users or "materially distort or impair" their free and informed decisions — [Regulation (EU) 2022/2065](https://eur-lex.europa.eu/eli/reg/2022/2065/oj) [R].
  - Art. 28(1) requires platforms accessible to minors to ensure "a high level of privacy, safety, and security of minors" [C].
  - The Commission's guidelines on Art. 28 (14 July 2025) recommend private-by-default accounts for minors, no profiling-based ads to minors, and features that drive excessive use (streaks, autoplay, push notifications) **off by default** for minors, plus age assurance and better reporting tools. They also address AI chatbots integrated into platforms — [European Commission, guidelines on protection of minors](https://digital-strategy.ec.europa.eu/en/library/commission-publishes-guidelines-protection-minors); [Taylor Wessing analysis](https://www.taylorwessing.com/en/insights-and-events/insights/2025/07/rd-european-commission-guidelines-on-protection-of-minors-under-the-digital-services-act) [C: consistent across [secure-agentic-framework use case](https://github.com/secure-agentic-framework/saf-agentic-use-cases), [victorsole/brubru guide](https://github.com/victorsole/brubru) and [mattcree/kidnix research](https://github.com/mattcree/kidnix)].
  - Implication for SubOne: SubOne's defaults (no streaks, no public feed) already meet this bar; also default students' push to off-until-opted-in, with quiet hours.
- [Regulator report and enforcement, US]
  - The FTC staff report "Bringing Dark Patterns to Light" (Sep 2022) groups dark patterns into design elements that (1) induce false beliefs, (2) hide or delay material information, (3) lead to unauthorised charges, and (4) obscure or subvert privacy choices — [FTC report](https://www.ftc.gov/reports/bringing-dark-patterns-light) [R].
  - A 2024 FTC/ICPEN/GPEN review of **642** subscription websites/apps found **76%** used at least one possible dark pattern and **67%** used several — [FTC press release, July 2024](https://www.ftc.gov/news-events/news/press-releases/2024/07/ftc-icpen-gpen-announce-results-review-use-dark-patterns-affecting-subscription-services-privacy) [C].
  - In Dec 2022 Epic Games agreed to pay **$245M** over dark patterns that caused unwanted purchases, plus a **$275M** COPPA penalty that included default-on voice/text chat for children — [FTC press release](https://www.ftc.gov/news-events/news/press-releases/2022/12/fortnite-video-game-maker-epic-games-pay-more-half-billion-dollars-over-ftc-allegations) [C for $245M; R for $275M and chat defaults].
  - Implication for SubOne: never show Pro upsells to students; make pricing, renewal and cancellation plain for the paying teacher; scope chat to the team by default.
- [Regulator text, US] The amended COPPA Rule was published 22 Apr 2025, took effect 23 Jun 2025, and required compliance by 22 Apr 2026. It adds separate verifiable parental consent for disclosing children's data to third parties (e.g., targeted ads) and requires written data-retention and security programmes — [FTC, COPPA final rule announcement](https://www.ftc.gov/news-events/news/press-releases/2025/01/ftc-finalizes-changes-childrens-privacy-rule-limiting-companies-ability-monetize-kids-data) [C: dates corroborated in [secure-agentic-framework use case](https://github.com/secure-agentic-framework/saf-agentic-use-cases)].
- [State law, US, direction of travel] California SB 976 (2024) bars "addictive feed" platforms from sending minors notifications between 12am-6am, and between 8am-3pm on school weekdays (Sep-May), without parental permission, and sets minors' accounts to private by default — [SB 976](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202320240SB976) [C: via a news-article copy in [Swepro2025/AMERICAN-TIMES-github.io](https://github.com/Swepro2025/AMERICAN-TIMES-github.io)]. It targets feed-based social platforms, so SubOne is very likely out of scope, but its hours are a useful default.
  - Implication for SubOne: default student quiet hours of overnight plus school hours, adjustable by the teacher (e.g., allow pings during the club's after-school slot).

### Inferences
- Probably out of scope legally but still the benchmark: an invite-only team workspace does not "disseminate to the public", so it is likely not a DSA "online platform". SubOne's chat also isn't an "addictive feed" under SB 976. Schools, teachers and parents will still judge SubOne against these rules, and the UK Children's Code applies to any UK service likely to be accessed by under-18s (legal review needed).
- Healthy mechanisms ranked by evidence for SubOne:
  - (1) progress visibility at team level (progress principle, goal-gradient/endowed progress);
  - (2) concrete next actions with owner and "when" (implementation intentions);
  - (3) batched recaps: weekly digest, "since you were last here" (see §3 batching evidence);
  - (4) reminders only for real commitments (assigned task due, meeting, competition deadline), never for "you haven't opened the app";
  - (5) social accountability within the team (visible ownership of tasks). Evidence here is weaker and indirect, so keep it gentle, with no public shaming or "X is behind" broadcasts.
- A "retained active team" metric (Duolingo's CURR idea at team level) is a good north star because it rewards serving teams already using SubOne rather than maximising time spent.

### Gaps
- Could not verify Duolingo's own blog figures on streaks (e.g., the widely repeated "7-day streak users are 3.6x more likely to stay engaged", "streak freeze reduced churn", "iOS widget +60% commitment"). Secondary repos repeat them, but they appear in AI-generated teardown documents and were not used.
- Could not confirm whether the 2025 COPPA final rule adopted or dropped the 2023 proposal to limit engagement-prompting push notifications to children. Recollection is that it was not adopted; verify on ftc.gov.
- The exact wording of the EU Art. 28 guidelines on read receipts and on AI chatbots was not retrieved; only summaries were.
- No rigorous public evidence was found that team "accountability" features improve completion among teenagers specifically.

## 3. Notifications: opt-in, over-notification, digests vs real-time, relevance and frequency caps, quiet hours, channel choice

### Takeaway
Teens already receive a median of 237 phone notifications a day, and knowledge workers are interrupted about every two minutes. Controlled studies show that batching notifications (about 3 times a day) improves wellbeing, and that interruptions cost attention and time. Well-loved tools separate "things that need me" (real-time) from "things I might want to know" (digest), let users set working/quiet hours, and cap volume at the leadership level. For a PWA, the platform rules (user-gesture permission prompts; on iPhone, push only after Home Screen install) make in-app and email the default channels and push an opt-in extra.

### Cited Findings
- [Field study with phone tracking; n=203, ages 11-17; Common Sense Media, Sep 2023] About half of participants got **at least 237 notifications a day** (median); some got nearly 5,000 in 24 hours. About **25%** arrived during the school day and about **5%** at night — [Common Sense Media, "Constant Companion"](https://www.commonsensemedia.org/research/constant-companion-a-week-in-the-life-of-a-young-persons-smartphone-use); [NBC News coverage](https://www.nbcnews.com/health/health-news/teens-inundated-phone-prompts-day-night-research-finds-rcna108044) [C: quoted in [indieweb/wiki](https://github.com/indieweb/wiki), sample size noted in [Savjee newsletter](https://github.com/Savjee/savjee.be)].
  - Implication for SubOne: every student notification competes with ~237 others. Send none at night or during class by default, and make each one specific ("Maya assigned you: sand the nose cone, due Thu").
- [Field experiment] Batching smartphone notifications into three deliveries a day improved wellbeing (attention, productivity, mood, sense of control) compared with delivery as usual; silencing notifications entirely raised anxiety/FOMO — [Fitz, Kushlev et al. 2019, Computers in Human Behavior 101:84-94](https://doi.org/10.1016/j.chb.2019.07.016) [C: citation and "winning arm three times a day" corroborated in [homer-doctrine audit](https://github.com/batterbob/homer-doctrine) and [awesome-adhd paper notes](https://github.com/yutakobayashidev/awesome-adhd); detailed effect sizes not retrieved].
  - Implication for SubOne: make digest delivery the default (daily or weekly, by role), but don't go silent. Direct asks still arrive promptly within allowed hours.
- [Within-subject field experiment] Turning phone alerts on vs off for a week each increased inattention and hyperactivity symptoms when alerts were on — [Kushlev, Proulx & Dunn 2016, CHI](https://doi.org/10.1145/2858036.2858359) [C citation; R effect details].
- [Field study] Information workers had 57% of their "working spheres" interrupted and took about 25 minutes on average to return to an interrupted task. The popular "23 minutes 15 seconds" figure comes from an interview, not the paper — [Mark, Gonzalez & Harris 2005, CHI](https://doi.org/10.1145/1054972.1055017) [C via [NathanL15 notes](https://github.com/NathanL15/mse302-individual-project) and [homer-doctrine audit](https://github.com/batterbob/homer-doctrine)].
- [Telemetry plus survey; Microsoft 365 signals and 31,000 workers in 31 markets; June 2025] Employees are interrupted by a meeting, email or chat about **every 2 minutes** during core hours; ~**275 interruptions/day**. One critical review notes that 275 applies to the most-pinged 20% of users, not the average — [Microsoft Work Trend Index, "Breaking down the infinite workday"](https://www.microsoft.com/en-us/worklab/work-trend-index/breaking-down-infinite-workday) [C: [BHAVIT-EVO evidence digest](https://github.com/BHAVIT-EVO/architecture-v1), [NathanL15 notes](https://github.com/NathanL15/mse302-individual-project)].
  - Implication for SubOne: teachers and mentors are already overloaded. Default them to a weekly (or twice-weekly) team digest plus real-time only for items that need them (approvals, safeguarding flags, direct questions).
- [Product practice, GitHub] GitHub separates notifications for things you are **participating in** (you commented, were @mentioned or assigned) from things you are **watching**. It delivers to a web inbox, email and mobile; mobile push can be limited to direct mentions, assignments and review requests; users can "schedule when GitHub Mobile will send push notifications" (working hours), create custom filters and ignore repositories — [GitHub Docs, Configuring notifications](https://github.com/github/docs/blob/main/content/subscriptions-and-notifications/get-started/configuring-notifications.md) [V].
  - Implication for SubOne: copy this model. "Needs me" (assigned, @mentioned, replies to my thread, due soon) is eligible for real-time. "Team activity" goes to the "since you were last here" summary and the digest. Per-user quiet hours come preset for students.
- [Platform rule] You "should only request consent to display notifications in response to a user gesture". Firefox (from v72) and Safari enforce this, and notifications require a secure context — [MDN, Using the Notifications API](https://developer.mozilla.org/en-US/docs/Web/API/Notifications_API/Using_the_Notifications_API) [V: read from [mdn/content](https://github.com/mdn/content)].
- [Platform rule] On iPhone/iPad, web push works only for web apps added to the Home Screen (iOS/iPadOS 16.4+), with permission requested from a user gesture — [WebKit, Web Push for Web Apps on iOS and iPadOS](https://webkit.org/blog/13878/web-push-for-web-apps-on-ios-and-ipados/) [C: consistent across [askahuman release notes](https://github.com/askahuman/askahuman) and [meshmonitor docs](https://github.com/Yeraze/meshmonitor)].
  - Implication for SubOne: many students on iPhones will never have push. In-app inbox plus email digest must carry the essentials. Ask for push in context ("Want a ping when someone assigns you a job?") after installation, never on first load.
- [Browser behaviour] Google announced Chrome would "automatically remove notification permission for sites you haven't interacted with recently", to "cut through the noise and reduce notification overload" — [press coverage copy](https://github.com/aibirthingcenter/Jupiter-Orbit-Of-Doom) [C, secondary only]. In 2020 Chrome had already introduced a "quieter" permission UI for notification prompts — [Chromium blog](https://blog.chromium.org/2020/01/introducing-quieter-permission-ui-for.html) [R].
  - Implication for SubOne: low-value pings don't only annoy; browsers now take the channel away.
- [Company practice] Duolingo's cap on notification quantity (CEO approval needed to increase it) and its auto-pause after ignored reminders — see §2 [V]/[C].
- [Sleep guidance] Teens aged 13-18 need 8-10 hours of sleep per night — [AASM consensus, Paruthi et al. 2016](https://doi.org/10.5664/jcsm.5866) [R]. California SB 976 uses 12am-6am and school hours as protected windows (§2) [C].

### Inferences
- Recommended SubOne defaults:
  - Students: in-app always. Email digest weekly, or none for under-13s unless the school or parent consents (COPPA "multiple contact" rules; legal check needed). Push off until opted in, with quiet hours 21:00-07:00 and during school hours, and ≤1 push/day except for direct assignments due within 24h.
  - Teachers/mentors: weekly digest by default, optional daily. Real-time only for approvals, flagged content and direct mentions.
- Relevance rules beat frequency caps alone. Send when the event involves *me* (assignment, mention, reply, deadline within 48h, change to something I own), and bundle everything else. "Since you were last here" is the pull-based complement and lowers the need for push.
- Measure each notification type by action rate within 24h and by opt-out/mute rate. Retire types with low action or high mute rates (Duolingo-style novelty decay implies content must change week to week).

### Gaps
- Could not verify any vendor push opt-in benchmarks (Airship, OneSignal, Braze). The only copies found were in AI-generated experiment files and were not used. Qualitatively: iOS requires explicit opt-in, and Android 13+ added a runtime notification permission — [Android developers](https://developer.android.com/develop/ui/views/notifications/notification-permission) [R].
- Could not verify the widely repeated "X pushes per week → Y% disable / uninstall" survey statistics. Treat such figures as unverified.
- No verified benchmarks for weekly-digest email open or action rates in team tools.
- Pielot et al.'s in-situ notification studies (e.g., ~63 notifications/day among adults, 2014) are recalled only.

## 4. Speed and perceived performance: response-time thresholds, optimistic UI, local-first/sync engines, skeletons vs spinners, Core Web Vitals and business impact

### Takeaway
The long-standing thresholds still govern: about 0.1 s feels instantaneous, 1 s keeps flow, and 10 s loses attention. The fastest-feeling modern tools (Linear, Figma, Superhuman) keep data locally or in memory, apply edits optimistically and sync in the background, targeting under 100 ms per interaction. On the web, Google's Core Web Vitals give concrete targets (LCP ≤2.5 s, INP ≤200 ms, CLS ≤0.1, at the 75th percentile). Speed improvements correlate with conversion in e-commerce studies. Evidence that skeleton screens "feel faster" is weak and mixed; showing real progress or work is better supported.

### Cited Findings
- [Foundational HCI guidance] Response-time limits: **0.1 s** feels instantaneous; **1 s** keeps the user's flow of thought uninterrupted; **10 s** is about the limit for keeping attention — [NN/g, Response Times: The 3 Important Limits](https://www.nngroup.com/articles/response-times-3-important-limits/) [R]. Google's RAIL model asks for a visible response to input within 100 ms — [web.dev, RAIL](https://web.dev/articles/rail) [R].
- [Company engineering standard] Superhuman's "100ms rule": every interaction should complete in under 100 ms to feel instantaneous — [Superhuman, "Superhuman is built for speed"](https://blog.superhuman.com/superhuman-is-built-for-speed/); [Performance metrics for blazingly fast web apps](https://blog.superhuman.com/performance-metrics-for-blazingly-fast-web-apps/) [C: links and rule cited in [hero-org/herocast UX research](https://github.com/hero-org/herocast)].
- [Architecture documentation endorsed by the company] Linear's sync engine:
  - Models are persisted in IndexedDB and hydrated into an in-memory object pool (MobX-observable).
  - Edits update in-memory models immediately and are queued as transactions to the server, with no waiting for confirmation.
  - The server broadcasts "delta packets" over WebSocket to all clients; hydration is lazy.
  - Linear's CTO Tuomas Artman called this reverse-engineered write-up "probably the best documentation that exists — internally or externally".
  - Source: [wzhudev/reverse-linear-sync-engine](https://github.com/wzhudev/reverse-linear-sync-engine) [V].
  - Implication for SubOne: logging a run, ticking a checklist item or moving a task should update the UI instantly and sync in the background, with a visible "saved / syncing / offline" state.
- [Company engineering blog] Figma's multiplayer uses a server-authoritative model inspired by CRDTs (per-property last-writer-wins) so edits appear instantly and converge — [Figma, How Figma's multiplayer technology works (2019)](https://www.figma.com/blog/how-figmas-multiplayer-technology-works/) [R]. The local-first ideals are: no spinners, multi-device, network optional, seamless collaboration, the long now, security/privacy by default, and user ownership — [Kleppmann et al., Ink & Switch, "Local-first software" (2019)](https://www.inkandswitch.com/local-first/) [R].
  - Implication for SubOne: race days happen at venues with poor connectivity. An offline-capable PWA (service worker plus local queue) for run logging and checklists is a differentiator, not gold-plating.
- [Google library, primary] Core Web Vitals thresholds (good / poor): **LCP ≤2,500 ms / >4,000 ms; INP ≤200 ms / >500 ms; CLS ≤0.1 / >0.25** — [GoogleChrome/web-vitals README](https://github.com/GoogleChrome/web-vitals) [V]. Pages are assessed at the **75th percentile** of loads — [web.dev, LCP](https://web.dev/articles/lcp) [C]. INP replaced FID as a Core Web Vital in March 2024 — [web.dev, INP](https://web.dev/articles/inp) [R].
  - Implication for SubOne: set budgets on low-end school Chromebooks and older Android phones (p75 INP ≤200 ms, LCP ≤2.5 s), and collect them first-party with the web-vitals library (no third-party analytics needed).
- [Correlational industry study; 37 brands, 30M+ sessions; Google/Deloitte 2020] A **0.1 s** faster mobile site was associated with **+8.4%** retail conversions, **+10.1%** travel conversions and **+40.1%** luxury product-to-cart progression — [web.dev, Milliseconds make millions](https://web.dev/case-studies/milliseconds-make-millions) [C]. **Vodafone**'s A/B test found a 31% better LCP gave **8% more sales** — [web.dev, Vodafone case study](https://web.dev/case-studies/vodafone) [C]. Both are e-commerce contexts, and the Deloitte elasticities come from already-fast sites, so they should not be extrapolated linearly.
- [Design-system guidance, GitHub Primer] For loading states:
  - Under **1 s**, show no loader ("Seeing a loading indicator flash on the screen could be distracting").
  - For **1-3 s**, use an indeterminate spinner.
  - For **3-10 s**, use determinate progress where possible.
  - For **10 s+**, use determinate progress and consider a background task.
  - Use skeletons for large content areas, give one screen-reader announcement per group of skeletons, and use `aria-busy`.
  - Source: [Primer, Loading](https://github.com/primer/design/blob/main/content/ui-patterns/loading.mdx) [V].
- [Small experiments, mixed] In Viget's 2017 test (n=136), skeleton screens did *worst*: participants shown a spinner rated the wait more positively and estimated it as shorter. Other small studies found non-significant or mild benefits — [Viget, "A Bone to Pick with Skeleton Screens"](https://www.viget.com/articles/a-bone-to-pick-with-skeleton-screens/) [C: via [orvi2014 essay](https://github.com/orvi2014/my-website) and [InTown research synthesis](https://github.com/pranitnale/InTown)].
  - Implication for SubOne: use skeletons for layout stability (which also protects CLS), not because they "feel faster". The real fix is making data local or cached so most views need no loader at all.
- [Experiments, 5 studies] The "labour illusion": when a service visibly shows the work it is doing, people can value the result more, even with a longer wait — [Buell & Norton 2011, Management Science 57(9)](https://doi.org/10.1287/mnsc.1110.1376) [C: summary in [InTown research](https://github.com/pranitnale/InTown)].
  - Implication for SubOne: for the AI race engineer's slower answers, show concrete steps ("Reading 12 runs from v4 and v5 · Comparing wheel setups…") rather than a bare spinner.

### Inferences
- Priority order for SubOne performance work: (1) optimistic writes and a local cache for the Today screen, tasks, runs and chat; (2) an app-shell PWA so repeat visits open instantly; (3) route-level code splitting to keep INP low on Chromebooks; (4) clear sync/offline status.
- An honest "Saved · Offline, will sync" indicator is part of forgiveness (§5), especially at the track.

### Gaps
- Could not re-verify the exact wording of NN/g's skeleton-screen guidance (commonly summarised as skeletons for full-page loads under ~10 s).
- No public data on how perceived speed affects retention in team workspaces (as opposed to e-commerce conversion).

## 5. Feedback and forgiveness: microinteractions, undo vs confirmation, autosave and drafts, error messages, empty states that teach

### Takeaway
Mature design systems converge on the same practices:
- make success visible through the interface itself and keep toasts sparing;
- autosave where people expect instant effect, but never lose input;
- prefer undo to "Are you sure?", keeping confirmation for truly irreversible actions;
- write errors that say what happened and how to fix it, in plain words without blame;
- turn empty states into teaching moments.
These practices cost little and matter even more for younger users, who are more likely to make mistakes and to be discouraged by them.

### Cited Findings
- [Design-system guidance, GitHub Primer, Saving] Use **explicit save** for declarative controls (text inputs, checkboxes, radios, multi-selects) because "users expect to set a value and then submit". Use **automatic saving** for imperative controls (toggles, segmented controls). "Avoid mixing explicit and automatic save patterns on a single page". On save errors, "the user's data should be preserved in the form and they should be given feedback about the failure". For destructive actions, confirm intent and "provide undo options when possible" — [Primer, Saving](https://github.com/primer/design/blob/main/content/ui-patterns/saving.mdx) [V].
  - Implication for SubOne: autosave long-form work (portfolio sections, judged-talk script, run notes) as drafts with visible "Saved" state and version history; explicit Save for settings-like forms.
- [Design-system guidance, GitHub Primer, Messaging] "Use success messaging sparingly and rely more on interaction context"; "place messages near the action they are related to" — [Primer, Notification messaging](https://github.com/primer/design/blob/main/content/ui-patterns/notification-messaging.mdx) [V].
- [Government design system guidance] GOV.UK error messages:
  - "Describe what has happened and tell them how to fix it."
  - Avoid technical jargon, "please", "sorry", "valid/invalid" and humour such as "oops".
  - Be specific: say whether the input is empty, too long or in the wrong format.
  - Use instructions ("Enter your first name") for empty fields.
  - "Do not clear any form fields when showing the Error message component."
  - Use the same message beside the field and in the error summary.
  - Source: [GOV.UK Design System, Error message](https://design-system.service.gov.uk/components/error-message/), read from [alphagov/govuk-design-system](https://github.com/alphagov/govuk-design-system/blob/main/src/components/error-message/index.md) [V].
  - NN/g's error-message guidelines similarly ask for visible, precise, human-readable, constructive and polite messages — [NN/g, Error-Message Guidelines](https://www.nngroup.com/articles/error-message-guidelines/) [R].
  - Implication for SubOne: adopt GOV.UK-style rules, written for a ~11-year-old reader ("Add a date for your first race" rather than "Invalid date").
- [Design-system guidance, GitHub Primer, Empty states] Error-state empty screens should be "as specific as possible", avoid messages like "There was a problem" and, if recovery is possible, "explain what went wrong and nudge them towards a path to recover" — [Primer, Empty states](https://github.com/primer/design/blob/main/content/ui-patterns/empty-states.mdx) [V].
- [Practitioner essay, foundational] "Never use a warning when you mean undo": people habituate to confirmation dialogs and click through them, so undo protects better — [Aza Raskin, A List Apart (2007)](https://alistapart.com/article/neveruseawarning/) [R]. NN/g: confirmation dialogs prevent errors only if used sparingly, because frequent use breeds automatic dismissal — [NN/g, Confirmation Dialogs](https://www.nngroup.com/articles/confirmation-dialog/) [R]. Gmail's "Undo send" offers a configurable 5-30 s cancellation window — [Gmail Help](https://support.google.com/mail/answer/2819488) [R].
  - Implication for SubOne: use soft-delete with an "Undo" toast for tasks, runs, files and comments; a trash kept 30 days; and typed confirmation only for irreversible, high-blast-radius actions (deleting a season, removing a member, transferring ownership).
- [Heuristics] Nielsen's heuristics include user control and freedom (undo/redo, "emergency exits"), error prevention, and helping users recognise, diagnose and recover from errors — [NN/g, 10 Usability Heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/) [R].

### Inferences
- Microinteractions worth doing for SubOne: instant check-off with a subtle state change (not confetti or points); "Saved" and "Synced" states; inline validation on blur, not on every keystroke; drag-and-drop with a keyboard alternative (WCAG 2.2 Dragging Movements, §8).
- Car versions already give SubOne a natural mental model for forgiveness: "restore this version" for documents and car specs, and a visible change history ("who changed what").
- For teens, blame-free tone and easy recovery matter doubly because peers can see mistakes in a shared space. Undo and "edit after posting" windows in chat reduce embarrassment.

### Gaps
- Could not retrieve NN/g's 2023 update of its error-message guidelines or its microinteraction articles. No quantitative studies of undo vs confirmation in team tools were found.

## 6. Collaboration UX: presence, comments and mentions, activity feeds, assignment, handoffs; feeling alive without noise

### Takeaway
Team tools feel alive through *awareness*: seeing who is here, what changed, and what is mine. They stay calm by routing only "needs me" events in real time and summarising the rest. Research on workspace awareness backs this; modern tools (Figma presence, GitHub participating vs watching, Linear's real-time sync) put it into practice. The main risk is noise: knowledge workers already face an interruption about every two minutes, and "work about work" consumes a large share of time.

### Cited Findings
- [HCI research, foundational] Workspace awareness (knowing who is present, where they are working and what they are doing) is central to coordinating shared work — [Gutwin & Greenberg 2002, CSCW Journal](https://doi.org/10.1023/A:1021271517844) [R]; [Dourish & Bellotti 1992, CSCW '92](https://doi.org/10.1145/143457.143468) [R].
- [Product practice] GitHub separates participating/@mentioned/assigned notifications from watching, offers per-repository granularity, custom inbox filters and mobile working hours (see §3) — [GitHub Docs](https://github.com/github/docs/blob/main/content/subscriptions-and-notifications/get-started/configuring-notifications.md) [V].
- [Company retrospective] Slack found teams need about **3 people** to "really work", and treated 2,000 messages as the signal a team had truly tried the product — [First Round Review](https://review.firstround.com/from-0-to-1b-slacks-founder-shares-their-epic-launch-strategy/) [C].
- [Architecture] Linear pushes real-time "delta packets" to all connected clients, so teammates see changes without refreshing — [reverse-linear-sync-engine](https://github.com/wzhudev/reverse-linear-sync-engine) [V]. Figma shows live multiplayer cursors and presence on the same file — [Figma multiplayer blog](https://www.figma.com/blog/how-figmas-multiplayer-technology-works/) [R].
- [Telemetry and survey, vendor] Interruptions about every 2 minutes during core hours (Microsoft, 2025; §3) [C]. Asana's self-reported "Anatomy of Work" surveys (≈9,600 knowledge workers, 2022-2023) put roughly 58-60% of time on "work about work". This is vendor-funded self-report, not telemetry — [Asana, Anatomy of Work](https://asana.com/resources/anatomy-of-work) [C: characterised in [BHAVIT-EVO evidence digest](https://github.com/BHAVIT-EVO/architecture-v1)].
- [Method/practice] Basecamp's "hill charts" show progress as "figuring it out" versus "making it happen", which communicates uncertainty honestly rather than with percentage bars — [Basecamp, Shape Up, "Show Progress"](https://basecamp.com/shapeup/3.4-chapter-13) [R].
  - Implication for SubOne: a simple "status" per workstream (car build, portfolio, sponsors, talk) of "figuring out / doing / done / blocked" is more honest and teen-friendly than % complete.

### Inferences
- Recommended collaboration pattern set for SubOne:
  - (1) Light presence: avatars on the part, document or run currently being edited, with no "last seen" timestamps for students by default.
  - (2) Comments with @mentions and "assign from comment" to turn discussion into a task with one owner and a due date.
  - (3) A personal inbox limited to "needs me".
  - (4) A team activity feed that is filterable and summarised in "since you were last here" and the weekly digest.
  - (5) Handoffs as a first-class action: reassign with a note ("what's done, what's next, where files are").
  - (6) Status updates per workstream in plain language.
- Teen-specific adaptation: avoid read receipts and typing indicators by default in student chat. The DSA guidelines reportedly flag read receipts as pressure features, though this was not verified. Give teachers a read-only "watch" mode, and tell students clearly what teachers can see.
- "Alive without noise" test: a new event should appear in exactly one real-time place (inbox, if it needs me) and in summaries otherwise, never as multiple pings across channels.

### Gaps
- Could not verify details of Linear "Pulse" (project-update feed and summaries), Slack's AI recaps, Notion's Updates inbox or Figma's Spotlight/observation modes, because the product sites were blocked.
- No quantitative data found on how presence or activity feeds affect retention in team tools.

## 7. AI assistant UX: PAIR, Microsoft HAX, Apple HIG; showing sources, uncertainty, easy correction, in-context help, cost/usage transparency; special care for minors

### Takeaway
The major guideline sets agree:
- say clearly what the AI can and cannot do, and how well;
- show why it said something (sources and attributions);
- make correction and dismissal effortless;
- invite granular feedback;
- give users and administrators global controls;
- label AI-generated content.
For minors, add a layer. Surveys show teens use AI companions heavily, and regulation is moving fast (California SB 243, EU AI Act Art. 50 transparency from 2 Aug 2026, UK DfE product-safety expectations referenced by KCSIE 2026). A school "race engineer" should therefore be a grounded, clearly labelled tool, not a companion persona, with teacher oversight and designs that encourage students to think rather than just copy.

### Cited Findings
- [Research-validated guidelines; user study with 49 design practitioners testing 20 AI-infused products] Microsoft's 18 Guidelines for Human-AI Interaction — [Amershi et al., CHI 2019](https://doi.org/10.1145/3290605.3300233) [V: abstract]; guideline list per [Microsoft HAX Toolkit](https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/) [R]:
  - Initially: G1 Make clear what the system can do; G2 Make clear how well it can do it.
  - During interaction: G3 Time services based on context; G4 Show contextually relevant information; G5 Match social norms; G6 Mitigate social biases.
  - When wrong: G7 Support efficient invocation; G8 Support efficient dismissal; G9 Support efficient correction; G10 Scope services when in doubt; G11 Make clear why the system did what it did.
  - Over time: G12 Remember recent interactions; G13 Learn from user behaviour; G14 Update and adapt cautiously; G15 Encourage granular feedback; G16 Convey the consequences of user actions; G17 Provide global controls; G18 Notify users about changes.
  - Implication for SubOne: open the race engineer with capability cards ("I can compare your runs, explain aero basics, check your portfolio against the rubric; I can't see your CAD files"), and label weak answers ("Only 2 runs logged: low confidence").
- [Guidebook] Google PAIR People + AI Guidebook chapters: User Needs + Defining Success; Data Collection + Evaluation; Mental Models; Explainability + Trust; Feedback + Control; Errors + Graceful Failure — [PAIR Guidebook](https://pair.withgoogle.com/guidebook/) [R].
- [Platform guidance] Apple HIG for machine learning covers explicit and implicit feedback, calibration, corrections, mistakes, multiple options, confidence, attribution and limitations — [Apple HIG, Machine learning](https://developer.apple.com/design/human-interface-guidelines/machine-learning) [R].
- [Design-system rule, IBM Carbon] "Each AI component is required to have an embedded AI label and explainability popover that alerts users to AI-generated content", and the AI label gives "a pathway to explainability" so users can learn how the AI works — [Carbon for AI guidelines](https://github.com/carbon-design-system/carbon-website/blob/main/src/pages/guidelines/carbon-for-ai/index.mdx); [AI label usage](https://github.com/carbon-design-system/carbon-website/blob/main/src/pages/components/ai-label/usage.mdx) [V].
  - Implication for SubOne: mark every AI-written or AI-suggested block (in chat, portfolio drafts, sponsor emails) with an "AI" label and a "why / sources" popover. This also helps teams follow any competition rules on AI assistance.
- [Literature review; experiment] Overreliance on AI is a documented risk — [Microsoft Research, Overreliance on AI: literature review (2022)](https://www.microsoft.com/en-us/research/publication/overreliance-on-ai-literature-review/) [R]. In an experiment (n≈199), "cognitive forcing" designs, such as asking people to decide before showing the AI's answer, reduced overreliance more than simple explanations, though participants liked them less — [Buçinca, Malaya & Gajos 2021, CSCW](https://doi.org/10.1145/3449287) [R].
  - Implication for SubOne: in learning moments ("Why is our car slower on lane 2?"), the race engineer can ask the team for its hypothesis first, then compare. This is a "coach mode" that fits a school competition's learning goals.
- [Experiments] Showing the work being done increases perceived value (labour illusion; §4) [C].
- [Survey; n=1,060 US teens aged 13-17; Common Sense Media, 2025] **72%** have used AI companions, **52%** are regular users, **33%** use them for social interaction or relationships, **31%** find those conversations as satisfying as, or more satisfying than, conversations with real friends, and **23%** trust AI companions "quite a bit" or "completely" — [Common Sense Media, "Talk, Trust, and Trade-offs"](https://www.commonsensemedia.org/research/talk-trust-and-trade-offs-how-and-why-teens-use-ai-companions) [C: consistent across [baobab-tech research](https://github.com/baobab-tech/research-ai-harms) and [Souraka229 notes](https://github.com/Souraka229/unesco)]. In the UK, **64%** of 9-17-year-olds use AI chatbots and **35%** say it feels like talking to a friend — [Internet Matters, "Me, Myself & AI" (2025)](https://www.internetmatters.org/hub/research/me-myself-and-ai-chatbot-research/) [C].
  - Implication for SubOne: don't give the race engineer a befriending persona, emotional memory or "I missed you" re-engagement. Keep it a technical tool with a clear scope.
- [State law, US] California **SB 243** (signed 13 Oct 2025, effective 1 Jan 2026) requires companion-chatbot operators to disclose clearly that the bot is AI, state that it may be unsuitable for some minors, remind known minors at least **every three hours** to take a break and that the bot is not human, and keep suicide/self-harm response protocols. It includes a private right of action ($1,000 minimum per violation) — [SB 243 text](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB243) [C: bill text in [regnavigator](https://github.com/Shauryagulati/regnavigator); summaries in [hersona SECURITY.md](https://github.com/shiro-0x/hersona) and [unslop research](https://github.com/MohamedAbdallah-14/unslop)]. Task-focused assistants are likely outside the "companion" definition, but its practices are good defaults.
- [EU regulation] EU AI Act Art. 50 requires that people be informed when they interact with an AI system, applying from **2 Aug 2026** — [Regulation (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) [C: date in [PeakPerformance research](https://github.com/daniellpsilva1/PeakPerformanceDataMonorepo) and [unslop research](https://github.com/MohamedAbdallah-14/unslop)].
- [UK education guidance] The DfE's "Generative AI: product safety expectations" (Jan 2025) sets expectations for edtech genAI, including filtering, monitoring and reporting — [GOV.UK](https://www.gov.uk/government/publications/generative-ai-product-safety-expectations) [R for the full list: filtering; monitoring and reporting; security; privacy and data protection; intellectual property; design and testing; governance]. KCSIE 2026 (statutory safeguarding guidance for English schools) references these expectations and applies filtering and monitoring requirements to generative AI — [C: [nudge-policy-vault change log](https://github.com/nudgeeducation/nudge-policy-vault)].
  - Implication for SubOne: UK schools will ask whether the AI is filtered, whether a designated adult can see flagged conversations, and whether there are reports. Build teacher-visible safety flags and conversation logs, disclosed to students, into Pro/school settings.
- [Regulator guidance] The EU Commission's Art. 28 guidelines (July 2025) also address AI chatbots integrated into platforms that minors use — [European Commission](https://digital-strategy.ec.europa.eu/en/library/commission-publishes-guidelines-protection-minors) [C: heading-level only].

### Inferences
- A concrete pattern set for the SubOne "race engineer":
  - (1) Ground answers in the team's own data and cite them inline ("from Run 14, 12 Mar; Car v5 spec").
  - (2) State confidence and assumptions.
  - (3) One-tap correction ("That's wrong: v5 uses 8g cartridges") that updates the team record, not just the chat.
  - (4) Thumbs up/down with a reason (HAX G15).
  - (5) An AI label and "why" popover on every output (Carbon).
  - (6) Scope limits and safe refusals, with signposting to a teacher for wellbeing topics.
  - (7) No companion persona and no engagement-driven follow-ups.
  - (8) Teacher controls: AI on/off per team, a coach mode (hypothesis first), and visibility of safety flags.
  - (9) Usage and cost transparency for the paying teacher: a meter showing Pro AI usage this month, what counts, and what happens at the limit, with no surprise charges (FTC dark-pattern category 3).
- Label outputs as "Draft by AI, edited by Sam". Provenance matters for judged portfolios and talks, where competition rules may restrict AI use (check each competition's rules).

### Gaps
- Could not verify whether Apple's HIG has added a dedicated generative-AI page (2025) or what the PAIR Guidebook's latest update contains.
- Could not verify the detailed text of the DfE expectations (including any 2026 additions on cognitive and emotional development and manipulation) or the EU guidelines' AI-chatbot provisions.
- No public benchmarks found on AI usage-meter UX or its effect on trust. Cost-transparency guidance above is inference plus the FTC categories.
- The Digital Omnibus proposals (Nov 2025) to amend AI Act timelines were not checked for any effect on Art. 50.

## 8. Accessibility and inclusion at scale; consistency via design systems; UX writing and voice guides

### Takeaway
Accessibility is getting worse on the open web (WebAIM Million 2026: 95.9% of home pages fail detectable WCAG checks, with errors up about 10% year on year), while legal pressure on school-facing software is rising (ADA Title II deadlines now 2027/2028 after an April 2026 extension; the European Accessibility Act since June 2025). Design systems demonstrably speed teams up (Figma study: 34% faster) and bake in accessible, consistent components. Voice and plain-language guides (Mailchimp, GOV.UK) codify how to write for stressed or young readers, but there is little rigorous public data on their effect.

### Cited Findings
- [Automated audit of top 1M home pages; Feb/Mar 2026] **95.9%** had detected WCAG 2 failures, averaging **56.1 errors per page** (up from 51 in 2025, about +10%). Low-contrast text appeared on **83.9%** of pages and missing alt text on **53.1%** — [WebAIM Million 2026](https://webaim.org/projects/million/) [C: [peterbamuhigire design-system-skills benchmark](https://github.com/peterbamuhigire/design-system-skills); [amitse a11y daily notes](https://github.com/amitse/amitse.github.io)]. The 2025 edition had 94.8% failing and 51 errors per page — [WebAIM Million 2025](https://webaim.org/projects/million/2025) [C].
  - Implication for SubOne: automated checks (axe/Lighthouse in CI) catch the most common failures cheaply. Contrast and labels come first.
- [Standard] WCAG 2.2 (W3C Recommendation, Oct 2023) added:
  - Focus Not Obscured (Minimum) (AA);
  - Dragging Movements (AA): provide a non-drag alternative;
  - Target Size (Minimum) (AA): at least 24×24 CSS px;
  - Consistent Help (A);
  - Redundant Entry (A);
  - Accessible Authentication (Minimum) (AA): no cognitive-function tests such as memorising passwords without alternatives.
  - 4.1.1 Parsing became obsolete.
  - Source: [W3C, WCAG 2.2](https://www.w3.org/TR/WCAG22/) [R].
  - Implication for SubOne: kanban drag needs a "Move to…" menu, the Help entry should sit in the same place on every screen, and student login should allow passwordless options (class code, magic link, SSO).
- [US regulation] The DOJ ADA Title II rule (April 2024) requires state and local government web content and mobile apps, including public schools and content they provide through vendors, to meet **WCAG 2.1 AA** — [ADA.gov fact sheet](https://www.ada.gov/resources/2024-03-08-web-rule/) [R]. An **Interim Final Rule of 20 Apr 2026** moved compliance dates to **26 Apr 2027** (entities serving ≥50,000 people; was 24 Apr 2026) and **26 Apr 2028** (smaller entities and special districts). Comments closed 22 Jun 2026, and the extension is reportedly being challenged by the NFB — [C: [Accessibility.Build data files (as of 16 Sep 2026)](https://github.com/Accessibility-build/Accessibility.Build-Main-Website); [jamditis accessibility skill](https://github.com/jamditis/claude-skills-journalism)].
  - Implication for SubOne: US public-school buyers will ask for a WCAG 2.1/2.2 AA conformance report (VPAT/ACR) within this window.
- [EU regulation] The European Accessibility Act applies from 28 Jun 2025 to specified consumer products and services (e.g., e-commerce). Microenterprises providing services are exempt — [Directive (EU) 2019/882](https://eur-lex.europa.eu/eli/dir/2019/882/oj) [R]. Whether SubOne's Pro checkout is in scope needs legal review.
- [Prevalence] Colour vision deficiency affects about 1 in 12 men and 1 in 200 women — [Colour Blind Awareness](https://www.colourblindawareness.org/colour-blindness/) [R].
  - Implication for SubOne: run charts and status colours (red/green "on track") must also use shape, labels or patterns. In a mostly male student cohort, expect about one colour-blind member per team of 12.
- [Counterbalanced experiment reported by Figma; sample size not retrieved] Designers with access to a current design system completed a design objective **34% faster** than those without — [Figma, Measuring the value of design systems](https://www.figma.com/blog/measuring-the-value-of-design-systems/) [C: quoted from Figma's resource-library text in [Cheggin/request-for-startups](https://github.com/Cheggin/request-for-startups) and [neozhehan/figma-edit-mcp](https://github.com/neozhehan/figma-edit-mcp)].
- [Voice guide, primary] Mailchimp: "Our voice doesn't change much from day to day, but our tone changes all the time"; voice principles include being "plainspoken" and "genuine" — [Mailchimp Content Style Guide, Voice and tone](https://styleguide.mailchimp.com/voice-and-tone/), read from [mailchimp/content-style-guide](https://github.com/mailchimp/content-style-guide) [V]. GOV.UK's error-message rules (§5) [V] show a plain-language standard applied consistently across a very large service.
- [Survey research cited by GOV.UK] GOV.UK makes plain English mandatory and cites Trudeau (2012): about 80% of people preferred plain-English sentences, and the preference rose with complexity (e.g., 97% preferred "among other things" to "inter alia") — [GOV.UK, Writing for GOV.UK](https://www.gov.uk/guidance/content-design/writing-for-gov-uk) [R].
  - Implication for SubOne: write one voice guide ("a calm, expert pit-crew mate: plain, specific, encouraging, never sarcastic") with tone rules per situation (error, success, deadline, AI uncertainty). Test copy on 11-12-year-olds, since readability for the youngest users sets the floor.

### Inferences
- Minimum bar: WCAG 2.2 AA; keyboard-complete flows; screen-reader-labelled charts with a data-table fallback; reduced-motion support; and a dyslexia-friendly type scale and line length. A tokenised design system (colour, spacing, type) makes this cheap to maintain and keeps the phone and laptop experiences consistent.
- Consistency with well-known tools (Jakob's law, i.e. users' expectations come from other apps they use) lowers learning costs for teens who already know Google Docs, Canva and Discord. Use familiar patterns (@mentions, comment threads, kanban) rather than novel ones.

### Gaps
- Could not verify NN/g's teen usability findings; recollection is that teens have lower task-success rates than adults and dislike "childish" design. Shopify Polaris content guidelines were not retrieved. No rigorous public study found that quantifies the business effect of a voice/UX-writing guide.
- The sample size of Figma's design-system study was not retrieved.

## 9. Measuring UX privately: first-party/aggregated analytics, micro-surveys, small-sample usability testing, teacher interviews, and which metrics matter

### Takeaway
SubOne can learn what works without third-party analytics by combining:
- server-side or first-party aggregated counts (Plausible-style cookieless page metrics plus product events counted at *team* level);
- a HEART-style metric set (activation, weekly active teams, retention by season cohort, task success);
- small, frequent usability tests (5 per round, repeated, spread across age bands);
- 6-12 teacher interviews per segment (saturation research).
The "5 users find 85%" rule is an average with wide variance, so run several small rounds rather than one.

### Cited Findings
- [Framework, Google] HEART (Happiness, Engagement, Adoption, Retention, Task success) with the Goals-Signals-Metrics process — [Rodden, Hutchinson & Fu, CHI 2010](https://research.google/pubs/measuring-the-user-experience-on-a-large-scale-user-centered-metrics-for-web-applications/) [R].
- [Model plus guidance] Five users find about **85%** of usability problems, assuming a 31% average per-user detection rate; the advice is to run many small, iterative tests — [NN/g, Why You Only Need to Test with 5 Users](https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/) [R].
- [Empirical test of the model; 60 participants (sample size recalled)] Random 5-user samples found between **55% and 99%** of problems. Samples of 10 found at least ~80%, and samples of 20 at least ~95% — [Faulkner 2003, Behavior Research Methods](https://doi.org/10.3758/BF03195514) [C: [kranthi7899/water usability skill](https://github.com/kranthi7899/water)]. On complex e-commerce sites, the first 5 of 49 users found only ~35% of problems — [Spool & Schroeder 2001, CHI EA](https://doi.org/10.1145/634067.634236) [C].
  - Implication for SubOne: test with 5 students per round, and run separate rounds for 11-13, 14-16 and 17-19 year-olds and for teachers. Repeat every few weeks rather than running one big study.
- [Methods research] In interview studies, thematic saturation typically arrived by ~12 interviews in a homogeneous group, with basic themes present by ~6 — [Guest, Bunce & Johnson 2006, Field Methods](https://doi.org/10.1177/1525822X05279903) [C: [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills)].
  - Implication for SubOne: 6-12 teacher/mentor interviews per segment (e.g., UK STEM Racing teachers vs other competitions) before locking decisions on digests, Pro value and safeguarding controls.
- [Benchmark] The average System Usability Scale score is about **68** across 500+ studies — [MeasuringU, SUS](https://measuringu.com/sus/) [C: [kranthi7899/water](https://github.com/kranthi7899/water)]. SUS item wording can trip up less experienced readers. Finstad (2006) found non-native English speakers often misread "cumbersome", and Bangor, Kortum & Miller (2008) used "awkward" instead — [Bangor, Kortum & Miller 2008, IJHCI](https://doi.org/10.1080/10447310802205776) [R].
  - Implication for SubOne: use SUS with teachers and simplified wording, or the single-question SEQ, with students after key tasks.
- [Privacy-preserving analytics, primary docs] Plausible counts unique visitors without cookies. It hashes a daily-rotating salt with the site domain, IP and user agent, deletes salts every 24 hours, does not store raw IP addresses, and reports aggregates only — [Plausible data policy](https://plausible.io/data-policy) [R]. Apple uses local differential privacy to learn aggregate usage patterns without identifying individuals — [Apple ML Research, Learning with Privacy at Scale (2017)](https://machinelearning.apple.com/research/learning-with-privacy-at-scale) [R].
- [Regulator text, UK] The Children's Code expects profiling "off" by default (Std 12), high-privacy defaults (Std 7) and data minimisation (Std 8) — [ICO Children's Code](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/age-appropriate-design-a-code-of-practice-for-online-services/) [R].
- [Primary library] Core Web Vitals can be collected first-party with Google's open-source web-vitals library and sent to your own endpoint — [GoogleChrome/web-vitals](https://github.com/GoogleChrome/web-vitals) [V].

### Inferences
- A metric set that fits SubOne and privacy:
  - Adoption and activation: % of new teams reaching the team-activation threshold within 14 days (§1).
  - Engagement: **weekly active teams** (≥3 members doing a meaningful action, such as completing a task, logging a run or editing a document, per week), and % of members active per team.
  - Retention: by season-start cohort, measured against the competition calendar rather than calendar months (teams naturally go quiet after finals).
  - Task success: completion and time in moderated tests, plus a first-party funnel for 3-5 core tasks.
  - Happiness: a teacher SUS twice a season, plus an optional one-question in-product pulse after key tasks for students.
  - Notification health: action rate within 24h and mute/opt-out rate per notification type.
  - AI quality: helpful vs unhelpful rate, correction rate, and safety-flag rate.
- Privacy engineering: count events server-side keyed to team, not person, where possible. Drop IPs, rotate or pseudonymise IDs, and aggregate with minimum cohort sizes (e.g., hide cohorts under 5 teams). Run A/B tests with server-side flags and aggregate-only reporting. Publish a plain-language "what we measure" page for students, parents and teachers.
- Research with minors: recruit through teachers or schools, get parental consent and the child's assent (especially for under-16s and under-13s), have a teacher present or in the loop, collect no recordings of faces unless essential, and test in school settings with school devices.

### Gaps
- Could not verify whether the UK Data (Use and Access) Act 2025 relaxations of PECR consent for analytics cookies have commenced, or their exact conditions.
- No verified benchmarks for in-product micro-survey response rates.
- UK MRS guidance on research with children (consent ages) was not retrieved.
- No published "weekly active teams" benchmarks were found for education or team tools.

## 10. Cross-cutting: which practices fit a team product used by teenagers and teachers (adopt / adapt / avoid)

### Takeaway
Most practices behind excellent UX transfer directly: fast optimistic UI, forgiving design, plain language, templates, contextual onboarding and grounded AI. The practices to drop are engagement mechanics built on competition, loss aversion and variable rewards (streaks, leaderboards, like counts, guilt-framed reminders). Regulators and child-development evidence now treat these as inappropriate by default for minors, and Duolingo's own data shows how strongly they pull. Teachers need calm digests, control and safeguarding visibility. Students need privacy from each other's metrics, clear ownership, and quiet hours.

### Cited Findings
- [Survey; Pew Research, Dec 2024] **46%** of US teens say they are online "almost constantly" — [Pew Research Center, Teens, Social Media and Technology 2024](https://www.pewresearch.org/internet/2024/12/12/teens-social-media-and-technology-2024/) [R].
- [Field study] Median of 237 notifications a day for 11-17-year-olds, a quarter of them during school (§3) — [Common Sense Media](https://www.commonsensemedia.org/research/constant-companion-a-week-in-the-life-of-a-young-persons-smartphone-use) [C].
- [Regulator guidance] EU Art. 28 guidelines: streaks, autoplay and push notifications off by default for minors (§2) [C]. ICO Standard 5: don't use data to incentivise continued engagement; present "continue" options neutrally; provide pause mechanisms (§2) [C].
- [Company data] Leaderboards and streaks strongly lift engagement (Duolingo: +17% learning time, highly engaged learners tripled) (§2) [V].
- [Adolescent neuroscience] Teens show heightened reward-circuit responses to peer "likes" (n=32) (§2) [R].
- [Enforcement] The FTC's Epic Games settlement included default-on voice/text chat for children and dark-pattern purchases (§2) [C/R].
- [Teen AI use] 72% of US teens have used AI companions, and 23% trust them "quite a bit" or "completely" (§7) [C].

### Inferences
- **Adopt as is:**
  - sample workspace before signup;
  - template-first season setup;
  - short, user-triggered tours and contextual hints;
  - the team setup checklist (endowed progress);
  - Today "one next move" with an owner and optional "when";
  - "since you were last here" summaries;
  - optimistic, offline-tolerant UI;
  - autosave, version history and undo;
  - GOV.UK-style error copy;
  - WCAG 2.2 AA;
  - an AI label with sources, confidence and one-tap correction;
  - HEART-style private metrics.
- **Adapt for teens and teachers:**
  - Notifications: digest-first; students' push opt-in only with default quiet hours (night plus school hours) and ≤1/day; teachers weekly by default.
  - Presence: avatars on items, but no "last seen", read receipts or typing indicators for students by default.
  - Kudos: allowed within the team, but with no counts and no leaderboards.
  - Progress: shown at team or workstream level, never ranking individual students.
  - Reminders: tied only to real commitments, neutral tone, auto-pausing when ignored.
  - AI: a tool persona, not a companion; coach mode for learning moments; teacher controls; visible safety flags; clear notice to students of what teachers can see.
- **Avoid:**
  - streaks;
  - points/XP, badges for time-on-app, and leaderboards between students or teams;
  - like/view counts;
  - loss-framed or guilt copy ("Your team is falling behind!");
  - variable-reward surprises;
  - infinite feeds and autoplay;
  - default-on public profiles or cross-team DMs;
  - Pro upsells shown to students;
  - confirm-shaming;
  - hard-to-cancel billing;
  - third-party trackers and ads (already SubOne policy).
- **Where engagement evidence and teen protection conflict** (e.g., Duolingo-style leaderboards), SubOne should accept a possible engagement cost. Its buyer is a teacher, whose trust depends on SubOne visibly not manipulating students, and its "retained active team" metric does not require individual time-on-app.

### Gaps
- No controlled studies were found comparing competitive vs cooperative-only mechanics in teen *team* project tools specifically.
- Whether SubOne's chat makes it a "user-to-user service" under the UK Online Safety Act (and which Ofcom children's codes might apply) was not researched. Flag for legal review.
