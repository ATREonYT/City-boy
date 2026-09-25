# Comparable team workspaces: lessons from Linear, Notion, Asana, Basecamp and Trello (plus ClickUp, Monday.com, Slack, Discord and Figma) for SubOne, a school racing team workspace

_Method note (25 Sep 2026): Every direct page fetch was blocked by the network proxy (linear.app, basecamp.com, figma.com, atlassian.com, firstinspires.org, chiefdelphi.com and others). The session's web-search budget also ran out before the Reddit and Chief Delphi threads could be read directly. So every finding below comes from search-engine summaries of the cited pages. Quotes are given as those summaries rendered them, so spot-check them against the live page before publishing. Evidence tags: **(Primary)** = the company's own docs, changelog or founders; **(Secondary)** = press or third-party analysis; **(Reviews)** = G2/Capterra/forum user reports, which are anecdotal and have no sample size unless one is stated; **(Opinion)** = commentary. Lines starting "→ Implication for SubOne" are my inferences, not sourced facts._

---

## 1. Linear: its signature decisions, the Linear Method, and what the 2024 and 2026 redesigns changed and why

### Takeaway
Linear's edge comes from discipline:
- **An opinionated workflow.** Everything is built from issues, projects and cycles, and a Triage inbox sits in front of the backlog.
- **Speed.** A local-first sync engine removes loading spinners, so the keyboard and ⌘K feel instant.
- **Repeated rounds of subtraction.** Linear has cut back its interface several times: a redesign in March 2024, a personalised sidebar in December 2024, a mobile redesign in October 2025 and a "calmer interface" refresh in March 2026. The user's "2024–2025 redesign" is really this sequence.

Each round pushed navigation back and brought content forward. Its theme generator is especially relevant: it builds a whole theme from three inputs (base colour, accent colour, contrast) in the perceptually uniform LCH colour space, which maps almost exactly onto SubOne's "one team colour" design.

### Cited Findings
**Core idea and method**
- **(Primary)** Linear presents the Linear Method as a set of principles for building high-quality software. It includes saying no to busy work and starting simple before growing — [Linear Method: Principles & Practices](https://linear.app/method/introduction). Third-party guides summarise the method as "speed, clarity, and execution" — [TMetric guide](https://blog.tmetric.com/linear-project-management-guide-features-workflow-and-benefits/); [Morgen guide](https://www.morgen.so/blog-posts/linear-project-management).
- **(Primary/interview)** Linear believes productivity software should be opinionated. In its view, flexible software "lets everyone invent their workflows, which creates chaos as teams scale" — [Figma blog: The Linear Method: Opinionated Software](https://www.figma.com/blog/the-linear-method-opinionated-software/); [Linear Method](https://linear.app/method/introduction).
  - → Implication for SubOne: ship fixed, sensible defaults, such as one status flow for car parts and one for tasks, instead of a blank board teams must configure. Allow renaming, not redesign.
- **(Secondary)** By default, issues move Triage → Backlog → In Progress. Reviewers say this reduces decision fatigue and keeps team practice consistent — [Siit review 2026](https://www.siit.io/tools/trending/linear-app-review).
- **(Primary)** Cycles are described as a cadence and routine in which teams "decide priorities and assign responsibilities". The goal is "healthy momentum, not rushing toward the end". Two-week cycles are described as the most common — [Linear Method](https://linear.app/method/introduction).
  - → Implication for SubOne: short, repeating two-week blocks between the fixed competition dates give students a rhythm without sprint-style pressure.
- **(Secondary)** Issues, projects and cycles are the three core planning building blocks — [OpenHands blog, 27 Aug 2026](https://www.openhands.dev/blog/linear-for-project-management); [Contrary Research on Linear](https://research.contrary.com/company/linear).

**Triage and inbox**
- **(Primary)** Triage is "your team's shared inbox for new issues". Issues created by integrations, or by workspace members outside the team, land there first. From Triage you can accept an issue into the backlog, escalate it to the current cycle, merge it, decline it (which prompts a comment explaining why) or snooze it. An issue can also wait in Triage while you gather more information — [Linear Docs: Triage](https://linear.app/docs/triage).
- **(Primary)** Since 12 Oct 2023, "Triage responsibility" lets a team put named people on triage duty. They can either be notified or be assigned issues directly, rotating round-robin when there are several people — [Linear changelog 2023-10-12](https://linear.app/changelog/2023-10-12-triage-responsibility).
  - → Implication for SubOne: send input from outside the core team into a triage queue owned by a rotating student. That covers mentor suggestions, judges' feedback, the AI race engineer's recommendations and failed rules checks. Nothing enters the plan until someone accepts it.

**Speed, keyboard and command menu**
- **(Secondary, technical analyses)** Linear keeps workspace data on the client in browser storage, loads from that local copy on a warm start, and syncs changes in the background. Keyboard navigation works because "all the data required to show the UI is available locally—no spinners, no loading states". The ⌘K palette searches the local store, not the server — [performance.dev: How's Linear so fast?](https://performance.dev/how-is-linear-so-fast-a-technical-breakdown); [DEV: Why Linear Feels Fast](https://dev.to/0xgosu/why-linear-feels-fast-local-data-small-updates-and-product-discipline-1m53).
- **(Secondary)** ⌘K/Ctrl+K opens a global command menu. One guide's advice: "if you forget any other shortcut, open the command menu and type what you want to do". Nearly every action can be done without a mouse — [Morgen guide](https://www.morgen.so/blog-posts/linear-project-management).
  - → Implication for SubOne: ⌘K is what makes 14 sections bearable. It should search locally cached parts, runs, sponsors and tasks, and it should run actions ("log run", "add sponsor") as well as navigate.

**March 2024 redesign: "Welcome to the new Linear"**
- **(Primary)** The changelog entry is dated 20 Mar 2024; one search summary gives 27 Mar 2024. The redesign "redefined the foundational layers" of the interface to improve hierarchy, balance and density:
  - a new sidebar;
  - tabs, headers, filters and panels adjusted "to reduce the visual noise and clutter";
  - the current view, available actions and meta properties presented more clearly.

  Sources: [Linear changelog](https://linear.app/changelog/2024-03-20-new-linear-ui); [Linear on X](https://x.com/linear/status/1773435685275328542).
- **(Primary)** Linear rebuilt its theme system on the LCH colour space instead of HSL. LCH is perceptually uniform: a red and a yellow at lightness 50 look equally light, so custom themes look consistently good whatever base colours are chosen. The same generator now also produces the default light and dark themes. Instead of 98 hand-set variables per theme, Linear defines three inputs: base colour, accent colour and contrast. Contrast in the default themes was increased — [How we redesigned the Linear UI (part II)](https://linear.app/now/how-we-redesigned-the-linear-ui).
  - → Implication for SubOne: generate the whole palette from the team colour, a neutral base and a contrast value in a perceptually uniform space (LCH or OKLCH). Then a team that picks neon yellow or navy still gets legible, accessible screens.
- **(Primary, as summarised)** According to search summaries, the redesign took about six weeks. It was led by two designers (Romain and Yann) with the wider design team, and "no infinite-loop processes, workshops, or sticky notes" were involved. A two-part series explains why redesigns matter (Part I, "A design reset") and how this one was done (Part II) — [Part II](https://linear.app/now/how-we-redesigned-the-linear-ui); [Part I: A design reset](https://linear.app/now/a-design-reset); [LinkedIn share of Part II](https://www.linkedin.com/posts/alex-hinds-12449660_how-we-redesigned-the-linear-ui-part-%E2%85%B1-activity-7271662369150242816-Rssm).

**December 2024: personalised sidebar**
- **(Primary)** Since 18 Dec 2024, users can hide sidebar items or tuck them behind a "More" menu, drag items to reorder them, and choose whether unread notifications appear as a count or a dot. Right-click or "Customize sidebar" opens these options — [Linear changelog 2024-12-18](https://linear.app/changelog/2024-12-18-personalized-sidebar).
  - → Implication for SubOne: let each student hide sections they never use (a CAD lead may never open Money), and offer a dot instead of a number on badges, which is calmer. Teachers could set defaults per role.

**October 2025 and March 2026**
- **(Primary)** 16 Oct 2025: mobile app redesign — [changelog](https://linear.app/changelog/2025-10-16-mobile-app-redesign). Details were not retrieved.
- **(Primary)** 12 Mar 2026: a "UI refresh" plus an essay, "A calmer interface for a product in motion", by Charlie Aufmann and Maxime Heckel. Its central idea: in an information-dense product "not every element of the interface should carry equal visual weight". Elements central to the user's task stay in focus, while elements for orientation and navigation recede. Concretely:
  - the navigation sidebar was made dimmer so the content area takes precedence;
  - desktop tabs became compact instead of spanning the full width, with rounded corners and smaller icons and text;
  - reliance on icons "had become excessive in some views", so icons were redrawn and resized;
  - headers, navigation and view controls were made consistent across projects, issues, reviews and documents;
  - the palette moved from a cool, blue-ish grey to a warmer, less saturated grey that still feels crisp.

  Sources: [Linear: A calmer interface for a product in motion](https://linear.app/now/behind-the-latest-design-refresh); [Changelog 2026-03-12: UI refresh](https://linear.app/changelog/2026-03-12-ui-refresh). Linear's own framing was "a visual update designed to reduce noise and bring structure back into focus as the Linear product continues to evolve" — [Linear on LinkedIn](https://www.linkedin.com/posts/linearapp_linear-interface-refresh-a-visual-update-activity-7437912086438932483-9A5Z).
  - → Implication for SubOne: the "calm" recipe is concrete. Dim the sidebar and bottom bar relative to the content. Use the same header and view-control layout in every section. Use icons only where they help recognition. Surround the single team colour with warm neutral greys.
- **(Primary)** 24 Mar 2026: "Introducing Linear Agent" — [changelog](https://linear.app/changelog/2026-03-24-introducing-linear-agent). Details were not retrieved; this is relevant background for the AI race engineer.
- **(Opinion)** Linear's look has become a named SaaS design trend, "Linear design" — [LogRocket](https://blog.logrocket.com/ux-design/linear-design/).

**Pricing** (education offers are in Q10)
- **(Secondary)** The free plan allows unlimited members, 250 issues (archived issues don't count), 2 teams and 10 MB uploads — [t0ggles](https://t0ggles.com/blog/linear-free-plan-limits); [Omid Saffari](https://omidsaffari.com/blog/linear-pricing).
  - → Implication for SubOne: a cap on active items, with archiving as the release valve, is a known free-tier pattern. Avoid any cap that deletes history (see Slack in Q6).

### Inferences
- Linear shows that calm is kept by repeated subtraction, not a single design pass. The 2024 reset, the 2024 sidebar and the 2026 refresh were each framed as removing noise that built up as features grew. SubOne already has about 14 sections plus the AI, so it should plan for regular "noise audits".
- An opinionated workflow suits student teams even better than software teams. Members aged 11–19 change every year and have no appetite for configuring tools, so the defaults are the product.
- Local-first speed matters in workshops and at race venues with poor Wi‑Fi (see the Notion offline gap in Q2).

### Gaps
- I could not read Parts I or II in full. The "six weeks" figure and the team details come from search summaries. Part II's exact publication date is unverified: Roger Wong's commentary URL is dated Nov 2024 ([rogerwong.me](https://rogerwong.me/2024/11/how-we-redesigned-the-linear-ui-part-ii)), while Linear's X post "How we redesigned the Linear UI" dates to about late March 2024 by its post ID (my own calculation).
- I found no sourced user criticism of Linear (for example, that it is too rigid for non-engineering teams).
- Details of Linear Agent, the 2025 mobile redesign and Linear's onboarding and templates were not retrieved. The full list of Linear Method principle headings was not retrieved either.

---

## 2. Notion: blocks, templates, databases with several views, sidebar and teamspaces; what users love and what overwhelms them

### Takeaway
Notion's strength is a single flexible model: pages made of blocks, plus databases that can be shown in many views. It can become anything. Its main failure comes from the same place: a blank page and a "/" menu of dozens of block types leave newcomers unsure where to start. Notion's own fixes carry direct lessons for SubOne:
- asking what the user will use it for and preloading matching templates;
- teamspaces that let people hide irrelevant areas;
- a late and still-limited offline mode (August 2025).

### Cited Findings
- **(Opinion/analysis)** The "blank page" challenge: new users face an empty workspace full of unfamiliar tools, and "the overwhelming list of blocks you see when you hit /" makes it worse. As Notion has grown more powerful, newcomers "feel like they've jumped into the deep end" — [notion.ist](https://notion.ist/notions-blank-page-challenge/); [Nora: Why is Notion so hard to use?](https://www.noratemplate.com/post/why-is-notion-so-hard-to-use); [Medium: "Notion is not the problem…"](https://medium.com/@notionwithro/notion-is-not-the-problem-but-it-is-the-way-you-approach-it-7a0d8bf99420).
- **(Analysis)** Notion's onboarding asks up to three questions, the key one being "What will you use Notion for?", and preloads relevant templates. This removes "the anxiety of not knowing where to start" — [OnboardMe teardown](https://onboardme.substack.com/p/how-notion-solved-the-blank-page-product-strategy-deepdive); [Medium version](https://wyndomb.medium.com/how-notion-solved-the-blank-page-problem-686b2e73ae57).
  - → Implication for SubOne: onboarding should ask each person's role (designer, manufacturing, enterprise/marketing, team principal, teacher/mentor) and the team's competition class and region. It should then preload the season playbook, key deadlines, sample car parts and a sample sponsor pipeline. No section should ever open empty.
- **(Primary)** A Notion database can show the same items as a table, board, calendar, timeline, gallery, list, form, chart, map or dashboard. Views sit as tabs across the top of the database. Editing a date in the calendar view updates every other view. Filters, sorts and groups are saved separately for each view — [Notion Help: views, filters & sorts](https://www.notion.com/help/views-filters-and-sorts); [Notion guide: Using database views](https://www.notion.com/help/guides/using-database-views).
- **(Primary)** Teamspaces arrived with a new sidebar design "to help Notion scale". Organisations can create a teamspace per department, or temporary ones for cross-team projects. Members join only the teamspaces relevant to them and hide the rest — [Notion blog: New sidebar design](https://www.notion.com/blog/new-sidebar-design); [Intro to teamspaces](https://www.notion.com/help/intro-to-teamspaces); [Notion on X announcing the Teamspaces sidebar section, Dec 2022 by post ID](https://twitter.com/NotionHQ/status/1602762413463347200). Help pages disagree on which plans include teamspaces: one says Plus, Business and Enterprise; another summary says all plans — [sidebar set-up guide](https://www.notion.com/help/guides/the-best-way-to-set-up-your-teams-sidebar-for-clear-organization).
  - → Implication for SubOne: sub-team areas (Engineering, Enterprise and so on) inside one team, which students can join or hide, mirror how STEM Racing teams split roles.
- **(Primary)** Offline mode launched on 19 Aug 2025 (Notion 2.53) for the desktop and mobile apps — [Notion release notes](https://www.notion.com/releases/2025-08-19); [AlternativeTo](https://alternativeto.net/news/2025/8/notion-rolls-out-offline-mode-edit-pages-without-an-internet-connection). Its limits:
  - AI, embeds, forms, buttons, file uploads, real-time collaboration and advanced automations don't work offline;
  - offline databases started at 50 rows each;
  - some users report slow loading of saved offline pages.

  Sources: [21notion review](https://21notion.com/en/blog/notion-offline-mode-review-2025); [Fayedtion](https://fayedtion.com/notion-offline-mode/).
  - → Implication for SubOne: workshops and race venues have bad connectivity. The run log, reaction-time starts and build checklists must work offline and sync later.
- **(Opinion)** Slowness is a recurring complaint. An XDA columnist wrote "Notion is really starting to fall behind alternatives, and I can't see myself sticking around", and the rival Nuclino publishes "Notion slow? 7 ways to make Notion faster" — [XDA](https://www.xda-developers.com/notion-starting-to-fall-behind-alternatives-cant-see-myself-sticking-around/); [Nuclino](https://www.nuclino.com/articles/notion-slow); [Capterra listing](https://www.capterra.com/p/186596/notion/).
- **(Primary)** Notion publishes marketplace templates for team hubs, project management and wikis — [Notion templates: team hub](https://www.notion.com/templates/category/team-hub); [Team project management template](https://www.notion.com/templates/team-project-management).
- Age limits and education offers are covered in Q10: under-13s are barred and K–12 is excluded from the Education Plus plan.

### Inferences
- Notion's flexibility suits enthusiasts but burdens groups, because every team has to design its own system. Student teams change every year, so a hand-built Notion workspace is likely to decay when its builder graduates. I found no direct source for this.
- View tabs over the same data, each with its own filters, are the most-copied answer to "many views", and SubOne's Plan should follow the pattern (see Q8).

### Gaps
- No quantified G2 or Capterra sentiment for Notion was retrieved. I found nothing on Notion 3.0 or its AI agents (2025), or on Notion's personal "Home" and "My tasks" features.
- I found no sourced evidence of FRC or STEM Racing teams using Notion (see Q9).

---

## 3. Asana: My Tasks, Home, Inbox, goals, portfolios and workload; personal versus team work; notification complaints

### Takeaway
Asana separates "my work" (My Tasks, Home) from "team work" (projects, portfolios, goals) and adds an Inbox for updates. Managers also get Workload and Portfolios. The cautionary tale is notifications: complaints about email and inbox floods from repeated edits and automation rules are persistent and widely reported.

### Cited Findings
- **(Primary)** My Tasks lists every task assigned to you. You can organise it with custom sections and rules that move tasks automatically, so it works as a personal task tracker. Every plan includes it — [Asana: My Tasks](https://asana.com/features/project-management/my-tasks); [Asana Help: My Tasks](https://help.asana.com/s/article/my-tasks); [Asana Forum: private project vs My Tasks](https://forum.asana.com/t/private-team-project-for-personal-tasks-vs-my-tasks/160391).
- **(Primary)** The Inbox shows the latest updates on tasks you are involved in and lets you reply in place. You can filter it by person, tasks assigned to you, @mentions, or tasks you assigned to others — [Asana: Inbox](https://asana.com/features/project-management/inbox).
- **(Secondary)** Home gives an overview of your tasks, goals and projects — [Lux & Vita explainer](https://luxandvita.com/what-is-asana-and-how-does-it-work/).
- **(Primary)** The manager-level features:
  - **Portfolios** group projects so their health can be tracked with dashboards, status updates and workload.
  - **Workload** gives "a visual snapshot of team capacity" across projects. It shows who is overloaded, and managers can drag tasks between people.
  - **Goals** connect work to objectives and appear as a "Connected goals" column in portfolios.

  Sources: [Asana: Portfolios](https://asana.com/features/goals-reporting/portfolios); [Help: workload](https://help.asana.com/s/article/portfolio-workload-and-universal-workload?language=en_US); [Asana: Goals & reporting](https://asana.com/features/goals-reporting); [Help: portfolio views](https://help.asana.com/s/article/portfolio-views?language=en_US).
  - → Implication for SubOne: treat the judging criteria (portfolio, verbal presentation, stand, marketing and so on) as "goals" and link tasks and evidence to them. A teacher then sees which areas are covered, not just how busy people are.
- **(Reviews; anecdotal forum threads, no sample size)** Complaints recur:
  - 10 notifications for 10 edits in a row;
  - four emails for a single action (file upload, comment, status change, column move);
  - automation rules cluttering other people's inboxes when several fields are added at once;
  - teams threatening to switch tools over the email volume.

  Sources: [Asana Forum: way too many email notifications despite adjusting settings](https://forum.asana.com/t/way-too-many-email-notifications-going-to-my-team-despite-adjustments-in-the-notification-tab/579459); [too many notifications based on rules](https://forum.asana.com/t/too-many-notifications-based-on-rules/72934); [too many email notifications](https://forum.asana.com/t/too-many-email-notifications/50465); [notification overload best practices](https://forum.asana.com/t/notification-overload-best-practices-to-decrease-notifications/854073); [too many notifications on Android](https://forum.asana.com/t/too-many-notifications-on-android/723). A competitor's blog calls a noisy Asana inbox "one of the most common criticisms" — [ONES blog](https://ones.com/blog/what-reddit-users-get-wrong-about-asana-for-project-management/) (vendor opinion).
  - → Implication for SubOne: bundle all edits to one item in one burst into a single notification. Make digests the default, send students no email by default, and offer "dot, not count" badges.
- **(Reviews; anecdotal and dated, c. 2017)** An FRC team used Asana from mid-2017 to manage tasks between team leaders. It cited two limits: only one assignee per task, and a free-plan cap of 15 members (the limit at the time; the current cap was not verified) — [Chief Delphi: Project Management Platforms](https://www.chiefdelphi.com/t/project-management-platforms/153044); [Chief Delphi: Project Management in FRC](https://www.chiefdelphi.com/t/project-management-in-frc/161613).
  - → Implication for SubOne: student work is often done in pairs, so allow one owner plus helpers on a task.

### Inferences
- SubOne's Today ("one next move per person") is a sharper version of My Tasks. Asana lists everything assigned to you; SubOne picks one thing. Keep the full list one tap away for students who want it.
- A Workload view for teachers should be framed as "balancing the team" rather than monitoring individuals, given the users are minors.

### Gaps
- Asana's 2025–2026 interface changes, AI features, onboarding and templates, and current free-plan seat limit were not retrieved.

---

## 4. Basecamp: the "calm" philosophy, Hill Charts, automatic check-ins, message boards versus chat, Shape Up, and the stance on notifications and real-time chat

### Takeaway
Basecamp (made by 37signals) sells calm as a feature:
- asynchronous communication first: message boards for things that matter, Campfire chat for quick things;
- Automatic Check-ins that replace status meetings;
- Hill Charts that show honest progress on uncertain work;
- a single "Hey!" notification menu;
- "Work Can Wait" quiet hours, switched on by default.

Its Shape Up method, with fixed six-week cycles, flexible scope and a two-week cool-down, fits competitions with fixed dates. I found no independent evidence that the approach improves team outcomes.

### Cited Findings
- **(Primary)** Automatic Check-ins ask the team a question on a schedule, such as "What are you working on this week?" every Monday at 9am, and collect the answers in one place. They can run daily, weekly or monthly — [Basecamp features](https://basecamp.com/features); [ProofHub](https://www.proofhub.com/articles/basecamp-project-management).
  - → Implication for SubOne: a weekly check-in ("What did you do? What's blocking you?") also produces dated portfolio evidence and removes the need for teachers to chase students.
- **(Primary)** Hill Charts track work that involves uncertainty. The uphill half means still figuring it out; the downhill half means executing a clear plan. They don't update automatically: people move the dots by hand, based on their understanding of the work. 37signals later shipped "Better Hill Charts" — [Basecamp: Hill Charts](https://basecamp.com/hill-charts); [Basecamp 5 Help: Hill Charts](https://5.basecamp-help.com/article/1078-hill-charts); [37signals: New in Basecamp: Better Hill Charts](https://updates.37signals.com/post/new-in-basecamp-better-hill-charts-and-more).
  - → Implication for SubOne: for car work (aero research versus machining a wheel pod), a percent-complete figure misleads. A hill for each part or sub-project is honest and teaches students to name their uncertainty.
- **(Primary, 2015)** "Work Can Wait" in Basecamp 3 lets users set their working hours and days. Outside those hours Basecamp sends no email, push or in-app notifications. The default is 8am–6pm in each user's time zone, "to encourage Work Can Wait rather than default everyone's notifications on 24/7/365" — [Signal v. Noise: Basecamp 3: Work Can Wait](https://signalvnoise.com/svn3/basecamp-3-work-can-wait/); [Medium copy](https://medium.com/woah-basecamp-3/basecamp-3-work-can-wait-4adfb285c84b).
  - → Implication for SubOne: set quiet hours by default for minors (for example, no pushes after a school-night cut-off). A teacher could set them, with an override only on race days.
- **(Primary)** The "Hey!" menu is "a single inbox for nearly every kind of Basecamp notification": @mentions, assigned to-dos, completed to-dos, messages and comments — [Signal v. Noise: preview of Basecamp 3](https://signalvnoise.com/posts/3955-a-preview-of-whats-new-in-basecamp-3); [Basecamp Help: How notifications work](https://3.basecamp-help.com/article/86-how-notifications-work); [Basecamp 5 Help: notification settings](https://5.basecamp-help.com/article/1177-notifications).
- **(Primary/founder opinion)** Jason Fried, co-founder of 37signals, on group chat:
  - "Following group chat at work is like being in an all-day meeting with random participants and no agenda."
  - Group chat "has become the greatest interruption factory at work".
  - His rule of thumb: "Real-time sometimes, asynchronous most of the time."

  Context: his 2016 essay, repeated in later posts. 37signals itself pioneered business group chat with Campfire — [Boing Boing, 8 Mar 2016](https://boingboing.net/2016/03/08/group-chat-an-all-day-meeti.html); [Fried on X](https://x.com/jasonfried/status/700314634939543552); [Fried on LinkedIn: "Group Chat: The Best Way to Totally Stress Out Your Team"](https://ir.linkedin.com/posts/jason-fried_group-chat-the-best-way-to-totally-stress-activity-7003514151985696768-puap).
- **(Secondary)** How the two channels divide the work:
  - **Message Board:** long-form, permanent, asynchronous posts such as announcements, kick-offs and "important decisions, ensuring that vital context is never lost".
  - **Campfire:** quick real-time questions.
  - **The rule:** urgent clarifications go to Campfire; strategic discussion and project updates go to the board.

  Sources: [Unito: beginner's guide to Basecamp](https://unito.io/blog/ultimate-beginners-guide-to-basecamp/); [Pebb](https://pebb.io/articles/how-to-use-basecamp-for-internal-communication). Fried also writes on keeping the product simple — [HEY World: "Keeping easy from becoming hard"](https://world.hey.com/jason/keeping-easy-from-becoming-hard-e6af27d0) (title only retrieved).
  - → Implication for SubOne: Chat needs a companion "Announcements/Decisions" space, plus a one-tap "turn this message into a decision" action so outcomes don't scroll away.
- **(Primary)** Shape Up, Basecamp's product method:
  - six-week cycles followed by a two-week cool-down;
  - "appetite" (how much time do we want to spend on this?) replaces estimates, and "shaping" narrows the problem to fit that time;
  - a "betting table" meets during cool-down to choose the next cycle's work;
  - unfinished projects get no extension by default.

  Sources: [Shape Up](https://basecamp.com/shapeup); [Shape Up: The Betting Table](https://basecamp.com/shapeup/2.2-chapter-08); [Shape Up: Adjust to Your Size](https://basecamp.com/shapeup/4.1-appendix-02).
  - → Implication for SubOne: STEM Racing dates are fixed (regional, then national, then world finals). The season playbook can give each workstream a fixed time budget with flexible scope, and schedule a cool-down or review after each event.
- **(Secondary)** Pricing:
  - a free plan with 1 project and 1 GB;
  - $15 per user per month;
  - Pro Unlimited at a flat $299/month billed annually, or $349 billed monthly;
  - every paid plan has the same features, so you pay for team size, not for features.

  Sources: [Capterra: Basecamp pricing](https://www.capterra.com/p/56808/Basecamp/pricing/); [SmartSuite: Basecamp pricing](https://www.smartsuite.com/blog/basecamp-pricing).
  - → Implication for SubOne: a flat price paid by the adult (as Pro Unlimited does) is simple and never penalises team size. It is the closest analogue to SubOne's "Pro paid by a teacher or mentor".
- **(Opinion, third-party)** Reviewers describe Basecamp's calm-company approach as discouraging false urgency and burnout, with updates read in people's own time rather than as pings — [SmartSuite review](https://www.smartsuite.com/blog/basecamp-review).

### Inferences
- Basecamp's calm comes from its defaults (quiet hours on, a single inbox, asynchronous boards), not from settings people must find. For a young audience, SubOne should make calm the default rather than an option.
- Moving a Hill Chart dot by hand is itself a moment of reflection. That suits teaching, and the same "where are we really?" narrative is what engineering portfolios ask for.

### Gaps
- I found no independent studies or surveys showing Basecamp's approach improves outcomes. No G2 or Capterra "cons" were retrieved this session; commonly cited weaknesses such as limited views and reporting are unverified here.
- Help-site URLs mention "Basecamp 5", but its launch date and changes were not verified. I also found nothing on the HEY email product's "Screener".

---

## 5. Trello: why its board simplicity succeeded, where it breaks down, Power-Ups, and Atlassian's changes

### Takeaway
Trello's one-concept model (cards on lists on a board) made it instantly learnable, and it is still what student teams reach for first. It breaks down with dependencies, hundreds of cards, hierarchy across boards and reporting; at that point teams bolt on Power-Ups (add-ons), which bring clutter and extra cost. Atlassian has since made two big changes:
- in 2024 it capped free workspaces at 10 collaborators;
- in 2025 it shifted towards personal productivity, adding an Inbox and a Planner.

### Cited Findings
- **(Primary)** Free workspaces are capped at 10 collaborators, counting members, guests and pending invitations. From 8 Apr 2024, workspaces already at 10 or more could not add members. From 20 May 2024, workspaces over the limit became view-only — [Atlassian: collaborator limit update](https://www.atlassian.com/blog/trello/new-collaborator-limits); [Atlassian Support](https://support.atlassian.com/trello/docs/workspace-user-limit/); [GIGAZINE](https://gigazine.net/gsc_news/en/20240305-trello-free-plan-collaborator-limits/).
  - → Implication for SubOne: a single STEM Racing team (a handful of students plus teacher and mentors) fits under 10. A school running several teams in one workspace, or a large robotics team, does not. SubOne's "free for the whole team" with no seat cap matters most for multi-team schools.
- **(Secondary)** The free plan also caps automation at 250 runs a month and files at 10 MB — [Carly: Trello free plan limits](https://www.usecarly.com/blog/trello-free-plan-limits/).
- **(Primary)** In 2021 Trello dropped the rule of one Power-Up per board, so free users get unlimited Power-Ups. Butler automation (acquired in Dec 2018) is free with usage limits — [Atlassian: revamped pricing and Power-Ups for all](https://www.atlassian.com/blog/trello/revamped-pricing-and-power-up-news); [Trello automation](https://trello.com/butler-automation).
- **(Primary + secondary)** The "new Trello" added three things:
  - **Inbox:** capture to-dos from email, Slack, Teams or Siri;
  - **Planner:** connect a Google or Microsoft calendar and drag cards into time blocks;
  - **AI:** pulls due dates and action items out of forwarded messages.

  It rolled out to Free, Standard and Premium users from May to the end of July 2025 — [Atlassian: The wait is over—the new Trello is here](https://www.atlassian.com/blog/announcements/new-trello-is-here); [Techzine](https://www.techzine.eu/blogs/applications/129033/atlassian-revamps-trello-introduces-new-inbox-and-planner/); [devicebase](https://devicebase.net/en/atlassian-trello/updates/new-inbox-planner-and-ai-features-let-you-capture-organize-tackle-your-to-dos/5wr); [Francesco D'Alessio on X, May 2025](https://x.com/FrancescoD_Ales/status/1920166185146163655); [Trello Inbox](https://trello.com/inbox). **Date conflict:** one summary dates the announcement 19 Apr 2024, but the rollout timing and social posts point to spring 2025. Trade press described it as making Trello "a central hub for individual task management" — [Reworked](https://www.reworked.co/digital-workplace/trello-update-makes-it-a-central-hub-for-individual-task-management/).
  - → Implication for SubOne: even the classic team board decided users need a personal "capture it, then plan my day" layer on top of shared boards. That supports SubOne's Today.
- **(Reviews; aggregated, no sample sizes)** Where Trello breaks down:
  - it "very quickly shows its limits" with hundreds of tasks or complex dependencies;
  - there is no native dependency tracking, workload view or advanced reporting;
  - there is no hierarchy across boards;
  - screens become "overcrowded and unreadable";
  - Power-Ups "clutter the interface or require extra subscriptions".

  Sources: [Capterra: Trello reviews](https://www.capterra.com/p/211559/Trello/reviews/); [G2: Trello pros & cons](https://www.g2.com/products/trello/reviews?qs=pros-and-cons); [projectmanagers.net](https://projectmanagers.net/top-8-disadvantages-of-using-trello/); [Meister (a competitor)](https://www.meistertask.com/blog/trello-task-management-alternatives-2026-comparison-guide).
  - → Implication for SubOne: build the racing-specific features (parts tracking, run log, budget) into the product rather than relying on add-ons, and keep board cards visually simple.
- **(Student-team evidence)** STEM Racing / F1 in Schools team Rapidity Racing trialled Trello. The team signed off tasks on it, used card comments for feedback and suggestions, and used the calendar and scheduling features to stay accountable — [Rapidity Racing enterprise portfolio (PDF)](https://d347awuzx0kdse.cloudfront.net/nationalpipeline/content-file/T50_RAPIDITYRACING_ENTERPRISEPORTFOLIO_PDF%20%282%29.pdf?v=3c90a95a2ec3b7c6d0158c214db526b68c6cb980). FRC teams discuss their Trello use on Chief Delphi — [How does your team use Trello?](https://www.chiefdelphi.com/t/how-does-your-team-use-trello/152595) (title only). Trello publishes education templates — [Trello education templates](https://trello.com/templates/education).

### Inferences
- Trello succeeded by keeping the number of concepts tiny. SubOne's Board view should look Trello-simple while being backed by richer data (part, owner, due date, evidence).
- Teams writing up their tool use in portfolios (as Rapidity Racing did) suggests judges reward visible project management. SubOne's Plan exports are therefore portfolio material.

### Gaps
- Trello's current user numbers, Atlassian's 2025–2026 roadmap and account changes, and which views are paid-only were not retrieved. The date of the "new Trello" announcement is contested (see above).

---

## 6. ClickUp and Monday.com (the cost of the "everything app"); Slack and Discord (noise, lost decisions, and how student teams use them)

### Takeaway
- **Everything apps trade learnability and speed for breadth.** ClickUp's top complaints are its learning curve, its clutter and its slow views. Monday.com's most criticised aspect is how it charges: a three-seat minimum and seats sold in buckets.
- **Chat is where student teams actually live.** FIRST names Discord, Slack and Google Classroom as the standard tools for FRC teams.
- **But chat has real costs.** It buries decisions. Slack's free plan hides messages older than 90 days and has deleted anything over a year old since August 2024. Discord raises age and safety questions, and tightened its teen protections in 2026.

### Cited Findings
**ClickUp**
- **(Aggregator of G2 data; methodology unverified)** "Learning curve" is the second most-cited complaint (1,752 mentions on G2). "Ease of Setup" scores 8.2/10, the lowest of the measured metrics — [CheckThat.ai: ClickUp reviews](https://checkthat.ai/brands/clickup/reviews).
- **(Quoted via an aggregator; attributed to G2's editorial team; unverified)** "The UI is overwhelming. There are buttons everywhere, sidebars, menus, settings, tabs, and a dizzying array of options competing for attention." — [G2: ClickUp reviews](https://www.g2.com/products/clickup/reviews?page=8). One reviewer called the interface "cluttered with too many features that no one asked for" — [Capterra: ClickUp reviews](https://www.capterra.com/p/158833/ClickUp/reviews/).
- **(Reviews)** Some views load slowly, device syncing isn't always seamless, and large workspaces lag when switching between Board, Gantt and Calendar. Users also report the app "can get very sluggish" and automations "breaking frequently" — [Capterra p.4](https://www.capterra.com/p/158833/ClickUp/reviews?page=4); [TaskRhino 2026](https://www.taskrhino.ca/blog/clickup-review-2026-honest-analysis/).
- **(Opinion; reviewer consensus)** ClickUp offers "more features per dollar than any competitor", but you pay for it with a 2–4 week learning curve — [TaskRhino](https://www.taskrhino.ca/blog/clickup-review/); [Hack'celeration](https://hackceleration.com/labs/review/clickup).
- **(Primary press)** ClickUp 4.0 was announced in Dec 2025 and positioned against "work sprawl" — [BusinessWire, 10 Dec 2025](https://www.businesswire.com/news/home/20251210211779/es). Search results also surfaced complaints about "the redesign", but those were about Slickdeals' own app, not ClickUp, so I excluded them.
  - → Implication for SubOne: 14 sections is ClickUp-scale breadth. SubOne must counter it with role-based hiding, Today as the landing screen, ⌘K and consistent layouts, or it risks ClickUp's "buttons everywhere" reputation.

**Monday.com**
- **(Secondary; pricing analyses)** Monday's pricing mechanics:
  - every paid plan requires at least 3 seats, and seats are then sold in buckets, so "a team of six pays for ten seats";
  - automation and integration actions are capped per month (e.g., 250 on Standard);
  - analysts call this the most criticised aspect of its pricing: "invisible on the pricing page and very visible on the invoice".

  Sources: [Quackback](https://quackback.io/blog/monday-pricing); [TinyCommand](https://tinycommand.com/blogs/monday-pricing-explained); [LogicBalls: "the 3-seat trap"](https://logicballs.com/blog/monday-com-review); [Capterra: Monday.com reviews](https://capterra.com/p/147657/monday-com/reviews/?page=2).
  - → Implication for SubOne: never charge per student or for "ghost seats". A single flat Pro fee paid by the adult is easier to explain to a school.

**Slack**
- **(Primary + press)** Free workspaces show only 90 days of messages and files. From 26 Aug 2024, Slack began permanently deleting free-workspace messages and files older than one year, on a rolling basis. Upgrading later cannot restore them — [Slack Help: free-plan limits](https://slack.com/help/articles/27204752526611-Feature-limitations-on-the-free-version-of-Slack); [TidBITS, 24 Jun 2024](https://tidbits.com/2024/06/24/slack-to-stop-storing-historical-content-for-free-workspaces/); [Forbes, 19 Aug 2024](https://www.forbes.com/sites/jaymcgregor/2024/08/19/slack-delete-files-and-messages-august-26-free-account-premium/); [AlternativeTo](https://alternativeto.net/news/2024/8/slack-will-delete-content-older-than-one-year-for-free-plan-users-starting-august-26th). The free plan is also limited to 10 app integrations and one-to-one huddles (calls) — [slack.green](https://slack.green/en/blog/slack-free-plan-limits).
  - → Implication for SubOne: a racing season lasts many months, and the portfolio needs evidence from its early weeks. SubOne should keep full history free and let any message be pinned as evidence.
- **(Vendor blogs; opinion; statistics without disclosed method)** Decisions "get buried in threads where most people don't look", and teams rehash old discussions because chat history isn't built for long-term knowledge. Claims such as "~55% of workers say instant messaging hampers deep work" and "40% of internal queries are repeated" come with no methodology; treat them as unverified — [Thread Patrol](https://thread-patrol.com/blog/slack-thread-best-practices); [Question Base](https://www.questionbase.com/resources/blog/solving-information-overload-in-slack-channels); [Asa.Team](https://blog.asa.team/slack-notification-overload-project-status/).

**How student teams use chat**
- **(Primary; FIRST guidance)** FIRST says "Discord, Slack, and Google Classroom" have become the standard tools for communication within FRC teams. They are used to announce events and meetings and, in more experienced teams, to share ideas during the season. FIRST also advises:
  - check with the school administration before creating accounts;
  - make all student–mentor communication follow the FIRST Youth Protection Program (YPP) and school policy.

  Sources: [FIRST: How To: Organize a Team (PDF)](https://www.firstinspires.org/sites/default/files/uploads/resource_library/frc/team-resources/tca/tca-team-organization.pdf); [newer copy](https://www.firstinspires.org/hubfs/web/program/frc/resources/team-org.pdf?hsLang=en); [FIRST team management resources](https://www.firstinspires.org/resources/library/frc/team-management-resources).
- **(Secondary)** On Discord, teams give members sub-team roles so a tag notifies only that sub-team, not everyone. In the FRC context, server owners can lock down channel creation and keep access to every channel for monitoring — [FIRST PDF](https://www.firstinspires.org/hubfs/web/program/frc/resources/team-org.pdf?hsLang=en); [Chief Delphi: best way to use Slack for an FRC team](https://www.chiefdelphi.com/t/what-is-the-best-way-to-use-slack-for-a-frc-team/358293?page=3).
- **(Team practice)** Pearce Robotics runs a mentor-only channel on its team Slack and gives guidance on notification settings "so members don't get overwhelmed". Its mentors need background checks and YPP training — [Pearce Robotics: Team Communication: Slack](https://team.pearcerobotics.com/training/slack); [Pearce Robotics: Mentors](https://team.pearcerobotics.com/mentors).
- **(Team practice, UK)** Student Robotics gates its Discord. Invite links and passwords go to team supervisors, and newcomers see only welcome and rules channels until they read the rules and enter the password — [Student Robotics: Discord](https://studentrobotics.org/docs/tutorials/discord).
- **(Reviews; anecdotal)** FRC teams tried Google Groups and email for coordination, but it failed because emails were missed or misread. Other teams report using Trello, ClickUp, Wrike, or Slack combined with Asana — [Chief Delphi: Project Management Platforms](https://www.chiefdelphi.com/t/project-management-platforms/153044).
- **(Anecdotal; not student teams)** Organisations that moved from Slack to Discord cite Discord's better free tier, voice, screen sharing and community features — [MAMMOTH XR on Medium](https://medium.com/mammoth-xr/discord-in-the-time-of-covid-why-our-team-switched-from-slack-to-discord-de52a536fb6b); [Qovery on DEV](https://dev.to/qovery/why-we-moved-from-slack-to-discord-288j).

**Discord's age and safety rules**
- **(Primary)** Discord requires users to be at least 13, or older where local law says so — [Discord Terms](https://discord.com/terms); [BrightCanary guide](https://www.brightcanary.io/is-discord-safe/).
- **(Primary)** On 9 Feb 2026, Discord announced global "teen-by-default" settings for all new and existing users:
  - content filters and restricted access to age-gated spaces;
  - direct messages from people a user may not know go to a separate inbox, and only age-verified adults can change that setting;
  - only age-verified adults can speak on "stage" (broadcast) channels in servers.

  Age checks roll out in phases from early March 2026, using an AI age estimate, on-device facial age estimation or an ID scan — [Discord press release](https://discord.com/press-releases/discord-launches-teen-by-default-settings-globally); [WBRC, 17 Feb 2026](https://www.wbrc.com/2026/02/17/discord-rolling-out-teen-by-default-settings-enhance-safety-younger-users/); [Discord teen and child safety policy](https://discord.com/safety/child-safety-policy-explainer).
- **(Primary; community support)** Deleting a Discord channel is permanent and the data can't be recovered — [Discord support community](https://support.discord.com/hc/en-us/community/posts/360029420552-Grace-Period-for-Deleted-Channel-Recovery?page=2).
  - → Implication for SubOne: SubOne cannot beat Discord on voice or social features. Its chat should win on three things instead:
    - being school-safe: no private adult-to-minor messages, channels visible to mentors, no ads or trackers, and usable by under-13s under teacher management;
    - being linked to work items (parts, sponsors, evidence);
    - being permanent.

### Inferences
- The cost of an everything app is paid in the first two weeks (learning) and then every day (lag and clutter). For student teams, whose season starts fast and whose members change yearly, learnability in the first week is decisive.
- Chat is the de facto student workspace. SubOne should coexist with Discord and WhatsApp rather than demand a full switch (for example, links that preview nicely, or a digest). Any integration must still respect the "no third-party trackers" rule.

### Gaps
- Monday.com's UX praise (its visual boards and ease of use) and its education or nonprofit offers were not sourced this session.
- The r/FRC and r/FirstTechChallenge threads and the Chief Delphi threads were not read in full.
- I found no survey with sample sizes on how student teams use chat.

---

## 7. Figma: what its multiplayer, presence and commenting model teaches about collaboration

### Takeaway
Figma made presence ambient and feedback spatial:
- **Ambient presence:** live cursors, avatars, and modes for following another person's view.
- **Spatial feedback:** comments pinned to the exact spot on the canvas, which can then be resolved.
- **Two kinds of talk:** throwaway "cursor chat" that fades, versus comments that last.

Its engineering choice, a simple server-authoritative sync rather than the full complexity of Google Docs-style algorithms, shows real-time collaboration can be built simply.

### Cited Findings
- **(Primary)** Figma launched multiplayer editing in Sept 2016, when no other design tool had live collaboration. It shows every active participant's cursor and selection because "it provides important context". People also wave their cursor to get attention or point at an object, and everyone in the file has an avatar in the top-right corner — [Figma blog: Multiplayer Editing in Figma](https://www.figma.com/blog/multiplayer-editing-in-figma/); [Evan Wallace on Medium](https://medium.com/figma-design/multiplayer-editing-in-figma-8f8076c6c3a6).
- **(Primary)** Figma rejected operational transforms (the algorithm behind Google Docs) as unnecessarily complex for its problem. It borrowed from CRDTs (conflict-free replicated data types) but simplified them, because every edit flows through one central server — [Figma blog: How Figma's multiplayer technology works](https://www.figma.com/blog/how-figmas-multiplayer-technology-works/); [madebyevan.com](https://madebyevan.com/figma/how-figmas-multiplayer-technology-works/).
- **(Primary)** Comments are pinned to the point or region of the canvas the commenter selected, and can be resolved from the sidebar or the pin — [Figma Help: View and manage comments](https://help.figma.com/hc/en-us/articles/360041547593-View-and-manage-comments); [Figma Help: Comments in FigJam](https://help.figma.com/hc/en-us/articles/1500004290941-Comments-in-FigJam).
- **(Primary)** Observation mode lets you follow a collaborator's view in real time — [Figma blog: Observation Mode](https://www.figma.com/blog/figma-feature-highlight-observation-mode/).
- **(Secondary)** Spotlight lets others follow your movements, including zoom and page changes. Cursor chat shows a live, temporary bubble next to your cursor with no send button, and it lingers about 5 seconds after you stop typing — [DesignerUp](https://designerup.co/blog/5-ways-to-unlock-the-power-of-collaborate-and-communicate-in-figma/); [WPDean](https://wpdean.com/how-to-chat-in-figma/).
  - → Implication for SubOne: pin comments to a car part, a point on the 3D model or a page of the portfolio draft. Resolving a comment closes the loop and can feed the evidence log. Show avatars of who is present on the pitch outline and portfolio, and add a "follow me" mode for pitch rehearsals and design reviews.

### Inferences
- Figma's split between throwaway and lasting communication (cursor chat versus comments) is the same split as Basecamp's Campfire versus Message Board. Both suggest SubOne should make lasting feedback, attached to a specific item, the default, and chat the exception.

### Gaps
- No user sentiment on Figma's comment model (for example, comment overload) was gathered.

---

## 8. How these apps show several views of the same data (list, board, calendar, timeline) without confusing people

### Takeaway
The pattern that works:
- one dataset;
- a small set of views shown as tabs in the same place every time;
- each view remembers its own filters and grouping;
- an edit in one view appears in all of them.

Confusion comes from view controls that move around from section to section, from too many views, and from slow switching.

### Cited Findings
- **(Primary)** Notion shows views as tabs across the top of a database, with the same items and properties in every view. An edit in one view updates all of them, and filters, sorts and groups are saved per view — [Notion Help: views, filters & sorts](https://www.notion.com/help/views-filters-and-sorts); [Notion guide: Using database views](https://www.notion.com/help/guides/using-database-views); [Notion Developers: Working with views](https://developers.notion.com/guides/data-apis/working-with-views).
- **(Primary)** Linear's 2024 redesign presented "the current view, available actions, and meta properties" more clearly. The 2026 refresh made headers, navigation and view controls consistent across projects, issues, reviews and documents, "making it simpler to orient yourself" — [Linear changelog 2024](https://linear.app/changelog/2024-03-20-new-linear-ui); [Linear changelog 2026](https://linear.app/changelog/2026-03-12-ui-refresh).
- **(Primary)** Asana portfolios offer list, progress, dashboard and workload views over the same set of projects — [Asana Help: portfolio views](https://help.asana.com/s/article/portfolio-views?language=en_US); [Asana Help: portfolios overview](https://help.asana.com/s/article/portfolios-overview?language=en_US).
- **(Reviews)** ClickUp users report lag when switching between Board, Gantt and Calendar, and an overwhelming number of options — [Capterra](https://www.capterra.com/p/158833/ClickUp/reviews/); [CheckThat.ai](https://checkthat.ai/brands/clickup/reviews).
- **(Reviews)** Trello's single board becomes "overcrowded and unreadable" at scale — [projectmanagers.net](https://projectmanagers.net/top-8-disadvantages-of-using-trello/).
  - → Implication for SubOne: Plan should offer five fixed views (calendar, timeline, board, workload, risks) over one shared model of tasks and milestones. The tabs should sit in the same place in every section, switching should be instant because the data is local, and each person's last view should be remembered.

### Inferences
- Make the shared data visible. For example, when dragging a card on the board changes its date, briefly highlight that change in the timeline, and label views "as board" / "as timeline" rather than as separate pages.
- Choose the default view by role and device (teacher: timeline or workload; student: board or list; phone: list). That reduces how often anyone has to choose.
- Keep the number of views small and fixed. ClickUp's breadth shows the cost of letting views multiply.

### Gaps
- No Nielsen Norman Group (NN/g) or academic usability research on switching between views was retrieved.

---

## 9. What school and student teams actually use today, and the gaps they report

### Takeaway
Student teams assemble a patchwork of tools:
- group chat: Discord, Slack, Google Classroom, or texts and email;
- Google Drive for files;
- sometimes a board (Trello, Asana, ClickUp) or a method (Scrum, Gantt charts), which then gets written up in the portfolio.

The gaps they report keep recurring: missed or misread messages, notification overload, seat and history limits on free tiers, and youth-protection rules on adult–student contact. No generic tool fits the competition's own data or judging needs, which is why teams build their own tools, such as "Lookout for FRC". Project management is formally assessed in F1 in Schools / STEM Racing.

### Cited Findings
- **(Primary)** STEM Racing teams must produce an enterprise portfolio and an engineering portfolio. These cover the team, car design, manufacturing, marketing, project management, teamwork and team identity — [Wikipedia: STEM Racing](https://en.wikipedia.org/wiki/STEM_Racing).
- **(Primary)** F1 in Schools' Project Management Guide was written with the PMI Educational Foundation (PMIEF), the charitable arm of the Project Management Institute, using PMBOK methods. It states that "project management is now an assessed part of the competition". PMIEF provides funding, educational resources and volunteer project managers, and reports that nearly 3 million students have been impacted — [PMI: STEM Racing partnership](https://www.pmi.org/pmi-educational-foundation/about-us/news/the-impact-of-the-pmief-and-f1-in-schools-partnership); [PMIEF press release via Special Olympics](https://www.specialolympics.org/stories/news/pmi-educational-foundation-partners-with-leading-nonprofits-to-help-youth-learn-project-management); [copy of the F1 in Schools PM Guide on Studocu](https://www.studocu.com/in/document/dr-apj-abdul-kalam-technical-university/masters-of-business-administration/project-report/98717353); [ProjectManagement.com: Racing Toward Success](https://www.projectmanagement.com/articles/1035315/racing-toward-success--how-f1-in-schools-and-pmief-power-future-innovators-). Older PMIEF material cites 26,000 schools taking part; its date is unclear.
  - → Implication for SubOne: Plan, Risks and Workload are assessed evidence, not just productivity features. Exports should match what judges expect: a timeline or Gantt chart, a risk register, and roles and responsibilities.
- **(Team portfolios)** Examples of what teams used:
  - **Rapidity Racing:** Trello for sign-offs, comments and the calendar — [enterprise portfolio PDF](https://d347awuzx0kdse.cloudfront.net/nationalpipeline/content-file/T50_RAPIDITYRACING_ENTERPRISEPORTFOLIO_PDF%20%282%29.pdf?v=3c90a95a2ec3b7c6d0158c214db526b68c6cb980).
  - **Formula Wood:** six members coordinating over winter break through Google Hangouts, daily after-school meetings, emails and texts (an older portfolio) — [Scribd](https://www.scribd.com/doc/296496149/enterprise-portfolio).
  - **Aeolos (World Finals 2023):** described an agile, Scrum-based approach — [SlideShare](https://www.slideshare.net/slideshow/aeolos-project-managment-portfolio-world-finals-2023/266693075).

  Teams also share example portfolios publicly — [Off The Track: Portfolios](https://offthetrack.net/portfolios/); [Yas in Schools sample portfolios](https://f1-in-schools-torque.invisionzone.com/gallery/category/2-sample-portfolios/).
- **(Primary)** In FRC, Discord, Slack and Google Classroom are the standard communication tools, and youth-protection rules apply (full detail in Q6) — [FIRST: How To: Organize a Team](https://www.firstinspires.org/hubfs/web/program/frc/resources/team-org.pdf?hsLang=en).
- **(Secondary; FTC community wiki)** Slack, Google Chat and Discord are all text-based options for keeping teams in contact. Teams should weigh the pros and cons of Slack, Discord and Trello, and use Google Drive for sharing documents. Teams need team-management software to manage to-do lists and communicate when they aren't in the same room — [Project Robotica: FTC Team Management Software](https://projectrobotica.wiki/wiki/FTC:Team_Management_Software).
- **(Reviews; anecdotal)** Reports from FRC teams: email and Google Groups failed because messages were missed or misread; Asana had limits (one assignee per task, a member cap); other teams use Trello, ClickUp or Wrike — [Chief Delphi: Project Management Platforms](https://www.chiefdelphi.com/t/project-management-platforms/153044); [Chief Delphi: Project Management in FRC](https://www.chiefdelphi.com/t/project-management-in-frc/161613); [Chief Delphi: FRC 4935 project management process](https://www.chiefdelphi.com/t/frc-4935-t-rex-project-management-process/459348) (title only).
- **(Primary)** An FRC team built "Lookout", a web app that combines match and pit scouting with task management, "created by a FIRST team for FIRST teams" — [Chief Delphi: Introducing Lookout for FRC](https://www.chiefdelphi.com/t/introducing-lookout-for-frc-your-comprehensive-team-management-solution/452666). Teams have also used ProjectLibre for build schedules — [ProjectLibre FRC tutorial](https://www.academia.edu/6948304/Project_Libre_FRC_Tutorial).
  - → Implication for SubOne: teams want tools built for their competition, because generic project apps don't hold competition data (scouting in FRC; race times, aero figures and rules checks in STEM Racing).
- **(Primary)** Scale of a comparable programme: the 2026 FRC season has 3,791 teams across 56 regionals and 144 district events — [Wikipedia: FIRST Robotics Competition](https://en.wikipedia.org/wiki/FIRST_Robotics_Competition).

### Inferences
- A typical STEM Racing team's toolset, inferred from portfolios and FIRST guidance: group chat, plus Google Drive or OneDrive, plus an optional board, plus a Gantt chart or slides assembled for the portfolio after the fact. SubOne's opportunity is to make evidence build up during the season instead of being reconstructed at the end.
- Rules on adult–student contact (FIRST YPP and school safeguarding) are a design requirement: channels mentors can see, no private messages between adults and minors, and an audit trail. General-purpose chat apps leave this to each team's own configuration.

### Gaps
- I couldn't read Reddit (r/FRC, r/FirstTechChallenge, r/F1inSchools) or the Chief Delphi threads in full, because the search budget ran out and direct fetching was blocked.
- I found no STEM Racing team website confirming Notion use, and no survey data (with sample sizes) on the tools student teams use.
- Student complaints about Google Drive (file sprawl) and Microsoft Teams/Planner in schools were not researched.

---

## 10. Education programmes: what each app gives students and teachers for free (plus age rules)

### Takeaway
Most "free for education" programmes target university students or need institutional verification, and school-age (K–12) users are often excluded or restricted:
- Notion's Education Plus plan excludes K–12;
- Figma gives schools access but withholds AI tools from K–12;
- Slack gives 85% off, not a free plan;
- Linear's education programme is for colleges;
- Asana gives 50% off.

Minimum ages of 13 (Discord; and, per search summary, Notion) leave SubOne's 11–13-year-olds poorly served by mainstream tools. SubOne's "free for the whole team" is more generous for secondary schools than any programme found.

### Cited Findings
- **(Primary) Notion:**
  - Education Plus is free for individual students and educators with an eligible school email, as a one-member workspace. It includes unlimited pages and blocks, file uploads and 30-day version history.
  - "K–12 students and educators are not eligible" for this offer.
  - Student-led organisations at "select verified higher education institutions" can get the Plus plan free for all members.

  Sources: [Notion Help: Education plan](https://www.notion.com/help/notion-for-education); [Notion for Education](https://www.notion.com/product/notion-for-education); [Notion Help: can't upgrade to Plus for education](https://www.notion.com/help/cant-upgrade-to-the-plus-plan-for-education). Per the search summary, Notion's Personal Use Terms bar users aged "13 years of age or younger"; check the exact wording — [Notion Personal Use Terms](https://www.notion.so/Personal-Use-Terms-of-Service-00e4e5d0f2b9411cbee6493f15779500).
- **(Primary) Slack:** Slack for Education gives 85% off the Pro or Business+ plans for eligible K–12 schools, with discounts for higher education. Schools must provide documents proving accredited or nonprofit status, and processing takes 2–3 weeks — [Slack Help: Apply for the Slack for Education discount](https://slack.com/help/articles/206646877-Apply-for-the-Slack-for-Education-discount); [UserJot pricing summary](https://userjot.com/blog/slack-pricing-2025-plans-costs-hidden-fees).
- **(Primary) Figma:**
  - Figma for Education is free for verified students and educators.
  - K–12 students and educators get the Enterprise plan through their school or district; higher-education, bootcamp and secondary students get the Professional plan.
  - K–12 and high-school users do not get AI tools, Figma Make or Figma Sites.
  - Higher-education verification lasts a year, and new team members have 7 days to verify.
  - Figma changed its Education plan in 2025.

  Sources: [Figma Help: Figma for Education](https://help.figma.com/hc/en-us/articles/360041061214-Figma-for-Education); [Figma Forum: Updates to our Figma Education plan](https://forum.figma.com/product-updates-3/updates-to-our-figma-education-plan-44818); [Figma Education](https://www.figma.com/education/).
- **(Primary) Linear:** the Education Program gives full-time students a 100% discount (free for one year) for student-led programmes, clubs and other educational activities. It is open to colleges and higher-level institutions, and you apply by emailing support from a .edu address. Nonprofits get 75% off the Basic and Business plans — [Linear Docs: Billing and plans](https://linear.app/docs/billing-and-plans); [third-party summary](https://aistudentdiscount.com/linear-student-discount/).
- **(Primary) Asana:** 50% off for K–12 and higher-education institutions, and a 50% nonprofit discount verified through Goodstack — [Asana for Education](https://asana.com/industry/education); [Asana for Nonprofits](https://asana.com/industry/nonprofit); [Asana: nonprofits of all budget sizes](https://asana.com/inside-asana/asana-for-nonprofits-expands-all-budget-sizes).
- **(Conflicting) Trello:** some sources report a 75% discount on Standard and Premium for teachers and students, plus a Classroom licence at 75% off Premium. Others say there is no official student programme — [TCEA blog](https://blog.tcea.org/trello-for-teachers/); [Atlassian Community: special price for schools?](https://community.atlassian.com/forums/Trello-questions/special-price-for-schools/qaq-p/2815371); [Trello for Educators](https://trello.com/education).
- **(Primary) Discord:** minimum age 13, with teen-by-default settings since 2026 (see Q6) — [Discord Terms](https://discord.com/terms).
  - → Implication for SubOne: the real competitors for secondary-school teams are consumer tools that are free forever (Discord, Google Drive, WhatsApp), not discounted business software. SubOne's free team tier, with Pro paid by a teacher, beats every programme found on price. Supporting under-13s through teacher-managed accounts is a clear gap in the market.

### Inferences
- Several vendors deliberately withhold AI from school-age users (Figma's K–12 tier excludes its AI tools). SubOne's AI race engineer for 11–19-year-olds will need visible safeguards and teacher controls to be acceptable to schools. This is an inference; school AI policy was not researched here.
- Per-seat, discount-based education pricing (Slack, Asana) needs school paperwork and weeks of processing. A teacher paying one flat Pro fee by card is far lower-friction.

### Gaps
- Not retrieved: ClickUp, Monday.com and Basecamp education offers, and Google Workspace for Education or Microsoft 365 A1 (free to schools, and the default toolset many schools already have).
- Slack's minimum-age terms and under-13 legal requirements (COPPA in the US, the UK Age Appropriate Design Code) were not researched this session.
