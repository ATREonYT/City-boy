# Layout and Navigation Patterns for a Multi-Section Team Workspace (desktop + phone): research notes for SubOne

Research compiled 25 Sep 2026. It informs SubOne: a PWA team workspace for school racing-car teams (students aged about 11–19, plus teachers and mentors), with about 11 top-level sections, 3–6 tabs per section, a desktop sidebar, a phone bottom bar (4 items plus "More"), ⌘K search, editing done mostly in dialogs, an AI "race engineer", and team chat.

**How to read the tags**
- **Evidence type:** [Tested] = empirical study with users or data. [Guideline] = platform or design-system guidance (expert consensus, usually not published as a controlled test). [Standard] = normative accessibility standard. [Product] = documented product behaviour, changelog or press coverage. [Expert] = practitioner opinion or analysis.
- **How the source was read:** **(read)** = I read the page, or its official source file on GitHub, directly in this session. **(summary)** = the claim comes from a search-engine summary of the cited page. Those pages could not be fetched here (nngroup.com, linear.app, m3.material.io, figma.com, discord.com, blog.superhuman.com and others were blocked). Check exact numbers marked (summary) before quoting them verbatim.
- **Research limits:** the session's shared web-search quota ran out partway through. Some sub-topics are listed under Gaps for that reason: teen-specific UX studies, Linear Inbox, Notion Home, keyboard-shortcut adoption studies, and Raycast and VS Code documentation.

---

## Q1. Navigation breadth vs depth, visible vs hidden navigation, and what belongs in a phone bottom bar

### Takeaway
The evidence favours broad, shallow structures with the main destinations visible. In NN/g's quantitative study, hiding navigation behind a menu roughly halved how often people used it on desktop. Material and NN/g both put the bottom-bar range at 3–5 labelled destinations, and Apple advises fewer tabs and warns that an overflow "More" tab hides content. For SubOne, this supports about 11 visible, grouped sections on desktop and "4 + More" on phones. The phone version is a "combo" pattern, which tested far better than fully hidden navigation. It only works if frequent destinations stay one tap away and "More" mirrors the desktop groups.

### Cited Findings
- [Tested] NN/g ran a quantitative study (2016) with 179 participants on 6 websites, on desktop and mobile, together with WhatUsersDo. **On desktop**, people used hidden navigation (hamburger) in **27%** of cases, against **48%** for visible and **50%** for combo navigation. **On mobile**, they used hidden navigation in **57%** of cases against **86%** for combo, which is 1.5 times more. With hidden navigation, "discoverability is cut almost in half", tasks took **39% longer on desktop and 15% longer on mobile**, and people rated tasks as harder. Visible or combo navigation also meant more people completed tasks without falling back on search. — [NN/g: Hamburger Menus and Hidden Navigation Hurt UX Metrics](https://www.nngroup.com/articles/hamburger-menus/); [NN/g video](https://www.nngroup.com/videos/hamburger-menus/) (summary)
  - *Implication for SubOne:* Never collapse the laptop sidebar into a hamburger by default. On phones, the bar plus More is "combo" navigation, the pattern that scored best. Even so, whatever sits in More will be used noticeably less than the bar items.
- [Tested] NN/g's later work finds the hamburger icon itself is now widely recognised. Recognising the icon is a different thing from discovering what is behind it, which is what the 2016 study measured. — [NN/g: The Hamburger-Menu Icon Today](https://www.nngroup.com/articles/hamburger-menu-icon-recognizability/) (summary)
  - *Implication for SubOne:* People will find "More". The risk is that they won't know what is inside it, so label it with text, and have it open a list that uses the same group labels as desktop.
- [Tested, foundational] Larson & Czerwinski (1998) arranged 512 items as 8×8×8, 16×32 and 32×16. **16×32 was fastest** and left people "lost" least often; **8×8×8 (deepest) was slowest**. Breadth-vs-depth research broadly agrees that moderately broad, shallow menus beat narrow, deep ones. — [UMD HCIL technical report](https://www.cs.umd.edu/hcil/trs/99-15/99-15.html); [Human Factors International: Breadth vs. Depth](https://www.humanfactors.com/newsletters/breadth_vs_depth_we_revisit_this_question.html) (summary)
  - *Implication for SubOne:* 11 sections × 3–6 tabs gives about 50 end destinations in two levels. That is the broad, shallow shape the evidence supports. Avoid a third level, such as sub-tabs inside tabs or groups nested inside groups.
- [Expert] NN/g compares flat and deep hierarchies. Their example flat hierarchy has 3 levels and 8 top categories; their deep one has 5 levels and 4 top categories. Both have pitfalls, and the browsing experience differs even when the content is identical. — [NN/g: Flat vs. Deep Website Hierarchies](https://www.nngroup.com/articles/flat-vs-deep-hierarchy/) (summary)
- [Guideline] NN/g says mobile tab bars are persistent and "work best for 3–5 top-level navigation destinations". The same article places tab bars at the top on Android, which is out of date: current Material 3 uses a bottom navigation bar. — [NN/g: Basic Patterns for Mobile Navigation](https://www.nngroup.com/articles/mobile-navigation-patterns/) (summary)
- [Guideline] Material 3 guidance on the navigation bar:
  - "Navigation bars can have three to five destinations." — [Material Components docs: Navigation bar](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomNavigation.md) (read)
  - Compact windows (under 600dp) should always use a navigation bar. With **more than five destinations**, Material suggests a **modal expanded navigation rail** for the rest. — [M3 Navigation bar guidelines](https://m3.material.io/components/navigation-bar/guidelines) (summary)
  - The default Android label mode ("auto") shows labels on every item only when there are 3 or fewer; with 4 or more, only the selected item gets a label. This conflicts with Apple's "include tab labels" (next finding). — [Material Components docs](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomNavigation.md) (read)
  - *Implication for SubOne:* With 11 sections, Material's model is 4–5 bar items plus a panel listing the rest, which is what SubOne already does. Show labels on every bar item and don't rely on icons alone.
- [Guideline] Apple's tab bar guidance (current, iOS 26):
  - "It's generally easier to navigate among fewer tabs."
  - "Use a tab bar to support navigation, not to provide actions."
  - Include tab labels, "single words whenever possible".
  - "Reserve badges for critical information."
  - "Avoid overflow tabs… The More tab makes it harder for people to reach and notice content on tabs that are hidden."
  - "Don't disable or hide tab bar buttons, even when their content is unavailable… If a section is empty, explain why."
  - Keep the tab bar visible across sections; hiding it makes people forget where they are.
  - In apps with many sections, let people choose which items go in the tab bar. On iPad, aim for 5 or fewer default tabs.

  — [Apple HIG: Tab bars](https://developer.apple.com/design/human-interface-guidelines/tab-bars) (read)
  - *Implication for SubOne:* Keep "+ New" and "Ask race engineer" out of the tab bar, because they are actions. Let each person swap which 4 sections appear, so a marketing lead can pin Marketing. Out of season, show Race with an empty state rather than removing it.
- [Expert] Items in a bottom bar should go straight to a destination rather than opening menus or pop-ups. — [Smashing Magazine: Golden Rules of Bottom Navigation Design (2016)](https://www.smashingmagazine.com/2016/11/the-golden-rules-of-mobile-navigation-design/); [UX Planet: Bottom tab bar best practices](https://uxplanet.org/bottom-tab-bar-design-best-practices-ef3ee71de0fc?gi=4e5a6f59e21b) (summary; which of these pages the summary drew this from is uncertain)

### Inferences
- **Top-level count.** About 11 sections works on desktop when they are visibly grouped (Build / Enterprise / People) and named with one word each. No study gives a hard maximum for sidebar items; the real limit is how easily people can scan the list.
- **Phone bar.** 4 sections plus More uses 5 slots, the top of the 3–5 range.
  - Pick default slots by how often each section is used. Plausible candidates are Today, Plan, Chat, plus Car or Race; confirm this with analytics.
  - Let users re-order or swap slots.
  - Don't change slots automatically by season. Apple warns that nav items appearing and disappearing make an interface feel unstable.
- **"More" as a mini sitemap.** More should open a full-screen or large-sheet list grouped exactly like the desktop sidebar, with a search field at the top and Team, Settings and profile at the bottom. It should not be an unlabelled menu.
- **Merging sections.** If analytics show some sections are rarely used (for example Pitch and Portfolio), consider merging them into one section to reduce breadth. Test that before doing it; there is no evidence on it here.

### Gaps
- NN/g's hidden-navigation data comes from 2016 and from content websites, not logged-in team apps. I found no newer replication.
- I found no controlled study that sets a maximum number of sidebar items for SaaS apps. The 3–5 limit for bottom bars is guideline consensus, not an experimental result.
- NN/g's "Beyond the Hamburger" articles on what makes navigation discoverable (mobile and desktop) could not be read in detail.
- There is no usage data for SubOne's sections, which is needed to choose the phone-bar slots.

---

## Q2. Sidebars in leading products: groups, favourites/pins, recents, counts/badges, team switchers

### Takeaway
Leading tools are converging on the same sidebar:
- It stays visible and people can customise it.
- A small "personal" block sits at the top (home, inbox, my work), with collapsible groups below.
- Users can pin, hide and reorder items.
- Badges are used sparingly.

The well-known failures came from changing stable navigation or adding taps to frequent switches: Figma's floating panels, Discord's mobile rearrangements, and the learning curve of Slack's split rail-and-sidebar.

### Cited Findings
- [Guideline] Apple's sidebar guidance:
  - "Show no more than two levels of hierarchy in a sidebar. When a data hierarchy is deeper than two levels, consider using a split view interface that includes a content list between the sidebar items and detail view."
  - Group items with disclosure controls and give groups short labels.
  - "Let people customize the contents of a sidebar."
  - Let people hide the sidebar, but "avoid hiding the sidebar by default to ensure that it remains discoverable."
  - Avoid critical information or actions at the bottom of a sidebar (macOS).
  - Consider automatically collapsing the sidebar when the window narrows.
  - On iPhone and iPad, "consider using a tab bar first".

  — [Apple HIG: Sidebars](https://developer.apple.com/design/human-interface-guidelines/sidebars) (read)
  - *Implication for SubOne:* The grouped sidebar is right. Make groups collapsible and remember each user's choice. Keep search and "New" at the top; the user menu at the bottom is fine. On narrower laptop windows, collapse to an icon rail automatically. For Car → Versions, use a list-plus-detail layout rather than a third sidebar level.
- [Product] Linear (changelog, 18 Dec 2024) added a personalised sidebar: right-click an item, or use "Customize sidebar", to hide items, and drag and drop to reorder. A later design refresh adjusted the sidebar, tabs, headers and panels "to reduce visual noise, maintain visual alignment, and increase the hierarchy and density of navigation elements". — [Linear changelog: Personalized sidebar](https://linear.app/changelog/2024-12-18-personalized-sidebar); [Linear: Behind the latest design refresh](https://linear.app/now/behind-the-latest-design-refresh); [Linear: How we redesigned the Linear UI](https://linear.app/now/how-we-redesigned-the-linear-ui) (summary)
  - *Implication for SubOne:* Let a student hide sections they never use, such as Money, while leaving them reachable through search. Make the sidebar quieter rather than adding more.
- [Product] Slack's August 2023 redesign:
  - A narrow left rail now holds Home, DMs, Activity, Later and More, plus a Create button and profile.
  - A wider secondary sidebar shows whichever category is selected.
  - Activity combines mentions, threads and reactions, each with its own sub-tab.
  - Home keeps Unreads, Threads, and Drafts & sent at the top.
  - Users can group channels into custom sidebar sections.

  — [Engadget](https://www.engadget.com/slacks-latest-redesign-has-a-dedicated-dm-tab-and-a-discord-style-activity-view-130032154.html); [Computerworld](https://www.computerworld.com/article/2503287/how-to-use-slacks-new-interface.html); [Stanford UIT](https://uit.stanford.edu/news/new-features-help-you-get-even-more-excited-about-slack%E2%80%99s-redesign); [Medium analysis](https://medium.com/design-bootcamp/slack-just-unleashed-its-new-ui-heres-what-we-learn-74f60f2132c5); [Slack help: custom sections](https://slack.com/help/articles/360043207674-Organize-your-sidebar-with-custom-sections) (summary)
  - *Implication for SubOne:* Put one "Activity/Inbox" entry that merges mentions, replies and approvals near the top of the sidebar, instead of scattering notifications across sections.
- [Product] Figma's 2024 redesign (UI3) initially made the navigation and properties panels float and collapse. For the full release, Figma reverted to fixed, resizable panels. Floating panels cramped the canvas, especially on smaller screens, and designs peeked out distractingly behind them. People who spend many hours a day in Figma were hit hardest. — [Figma blog: Our approach to designing UI3](https://www.figma.com/blog/our-approach-to-designing-ui3/); [Figmalion #184](https://figmalion.com/issue/184); [Bits Kingdom analysis](https://bitskingdom.com/blog/figma-floating-panels-ux-lesson/) (summary)
  - *Implication for SubOne:* For a tool people use every day, keep the navigation fixed and predictable. Offer "collapse sidebar" as an option, not as a floating default.
- [Product] Discord's mobile app has been redesigned several times:
  - **Dec 2023:** Servers and DMs were split into separate tabs (Servers, Messages, Notifications, You). Users said this made it hard to switch mentally between mobile and desktop. — [TechCrunch](https://techcrunch.com/2023/12/05/discord-app-redesign-mobile) (summary)
  - **Later:** Discord posted that it had reworked search and tab navigation based on feedback. — [Discord blog](https://discord.com/blog/refining-discords-mobile-experience-with-your-feedback) (summary)
  - **Most recent (reported in 2026; date not verified):** a redesign that mimics desktop drew backlash. It removed several always-visible tabs and collapsed menus that had been one tap away, and people who switch servers and channels "dozens of times per session" said it added steps. — [remio.ai](https://www.remio.ai/post/discord-redesign-backlash-reveals-mobile-app-tradeoffs); [Android Police](https://www.androidpolice.com/discord-mobile-app-redesign/) (summary)
  - *Implication for SubOne:* Keep the phone and desktop mental models the same: same section names, groups, icons and order. Don't bury frequent switches, such as Chat channels or today's tasks, behind extra taps. Changing a navigation model users have already learned is expensive, so get it right early.
- [Guideline] GitHub's design system, Primer:
  - Users "should always have a clear understanding of their location within the application."
  - Its sidebar list (NavList) uses a parent–detail pattern: the parent navigation stays on screen while the detail view changes.
  - On narrow screens, a sidebar that indexes pages becomes its own page with back navigation. A sidebar of filters becomes an action menu or a bottom sheet.
  - Use breadcrumbs when users are more than one level deep on narrow screens.

  — [Primer: Navigation pattern](https://github.com/primer/design/blob/main/content/ui-patterns/navigation.mdx) (read)
- [Guideline] Primer's tab component: "When loading multiple counters asynchronously, wait for all the data to be ready before displaying the counters, so you can avoid multiple layout shifts." — [Primer: UnderlineNav](https://github.com/primer/design/blob/main/content/components/underline-nav.mdx) (read)
- [Guideline] Apple: reserve badges for critical information "so you don't dilute their impact and meaning." — [Apple HIG: Tab bars](https://developer.apple.com/design/human-interface-guidelines/tab-bars) (read)
  - *Implication for SubOne:* Use number badges only where the user must act: unread @mentions, items awaiting my approval, tasks overdue for me. Use a dot, or nothing, for passive activity. Never put counts on every section.
- [Product] Users on the Asana forum ask for a pinned or starred "watchlist" widget on Home, which suggests demand for user-curated shortcuts. — [Asana forum request](https://forum.asana.com/t/home-tab-pinned-starred-tasks-widget-custom-watchlist/1139866) (summary)

### Inferences
- **Recommended SubOne sidebar, top to bottom:**
  1. Team switcher (compact)
  2. "Search or jump to… ⌘K" field and a "+ New" button
  3. Personal block: Today, Inbox/Activity, My tasks
  4. Pinned: records or views the user pinned, capped at about 5–7
  5. **Build** (Plan, Car, Race), **Enterprise** (Money, Marketing, Pitch, Portfolio), **People** (Chat, Team)
  6. Footer: Settings and user menu
- **Personalisation:** users can hide, reorder and pin; teachers or admins set the defaults for each role. Hidden sections stay reachable through ⌘K.
- **Team switcher:** most students belong to one team, so keep it small. Teachers and mentors running several teams need it at top-left. Slack, Discord and Linear appear to follow that convention, but I did not verify it here.
- **Medium widths:** use an icon rail with tooltips, and expand to show labels on click or hover.

### Gaps
- I could not read Notion's, Asana's or GitHub's own sidebar documentation (blocked), so details such as Notion's favourites and teamspaces are unverified.
- I found no quantitative data on how badges or counts affect behaviour, or on where a team switcher works best.
- Checkly's 2025 sidebar redesign case study, which was based on user research, could not be read.

---

## Q3. In-page tabs and view switchers (list/board/calendar/timeline)

### Takeaway
Tabs work when content splits into clearly labelled, independent sections with the most-used first. They fail when:
- they overflow the available width,
- they hide content people need to compare, or
- they mix "different pages" with "different views of the same data".

Give each true tab its own URL. Board, calendar and timeline are formats of the same data, and are better handled as a view switcher inside one tab.

### Cited Findings
- [Expert] NN/g: "The fewer tabs, the better." When tabs overflow the tab list, the row often becomes a carousel, so the hidden tabs are less discoverable and cost more effort to reach. Use tabs when long content has clear groupings. — [NN/g: Tabs, Used Right](https://www.nngroup.com/articles/tabs-used-right/) (summary)
- [Guideline] GOV.UK Design System on tabs:
  - Use tabs when content can be separated into clearly labelled sections and the first section is the most relevant for most users.
  - Don't use tabs when users need to read everything in order or compare information across tabs.
  - Don't use tabs as page navigation.
  - Avoid tab labels that wrap onto two lines, and order tabs by user need.
  - On small screens, the component shows all sections in order on one page with a table of contents.
  - The component "has not yet been tried in research with users".

  — [GOV.UK Design System: Tabs](https://design-system.service.gov.uk/components/tabs/) (read via [source file](https://github.com/alphagov/govuk-design-system/blob/main/src/components/tabs/index.md))
- [Guideline] UK government design systems also advise starting each tab panel with a heading that repeats the tab label, which helps on small screens and for screen-reader users. — [ONS Design System: Tabs](https://service-manual.ons.gov.uk/design-system/components/tabs) (summary; which page this came from is not certain)
- [Guideline] Primer on tabs:
  - Use linked tabs (UnderlineNav) when switching tabs changes the URL, and tab panels when it doesn't. "You can't mix tabs that change the URL with tabs \[that\] just switch the visible tab panel." — [Primer: Navigation](https://github.com/primer/design/blob/main/content/ui-patterns/navigation.mdx) (read)
  - "Each tab panel should have discrete content with a unique URL, not just different formats to view the same content."
  - When tabs overflow, the component hides leading icons first, then moves items into an overflow menu one at a time.

  — [Primer: UnderlineNav](https://github.com/primer/design/blob/main/content/components/underline-nav.mdx) (read)
  - *Implication for SubOne:* Plan's tabs mix two kinds of thing:
    - Separate content: Playbook, Risks, Workload.
    - Different formats of the same tasks and events: Calendar, Timeline, Board.

    Keep the first kind as URL-backed tabs. Present the second as a view switcher (segmented control or dropdown) inside one "Schedule" or "Tasks" tab. That cuts the visible tabs from 6 to about 4.
- [Product] Notion lets each database view open records as a side peek, a center peek or a full page. The defaults depend on the layout: table, board, timeline and list use side peek; calendar and gallery use center peek. The setting applies to everyone using that view. Side peek for databases launched in July 2022. — [Notion release notes, 20 Jul 2022](https://www.notion.com/releases/2022-07-20); [Bullet.so guide](https://bullet.so/blog/how-to-open-center-peek-notion/) (summary)
  - *Implication for SubOne:* Pick one default way to open records for each view type rather than one per record type. Side peek suits list and board views; a centred dialog suits calendar views.
- [Guideline] Apple: keep functionality the same across size classes. On larger screens, "consider taking advantage of larger spaces to switch from a tab bar to a sidebar or expose functionality that might otherwise be grouped into an overflow menu." — [Apple HIG: Layout](https://developer.apple.com/design/human-interface-guidelines/layout) (read)
  - *Implication for SubOne:* On phones, show the 3–4 most-used tabs and move the rest into a clearly labelled overflow menu. On desktop, show them all.

### Inferences
- Aim for 5 or fewer tabs per section on desktop, and 3–4 visible on phones with a clearly labelled overflow. Put the most-used tab first.
- Encode section, tab, view and key filters in the URL, for example `/plan/schedule?view=board&filter=mine`. Then links pasted into Chat, or produced by the race engineer, open exactly that state.
- When a URL doesn't specify a view, remember each user's last-used view per section. This is a common product pattern, but I didn't verify a primary source for it.
- Avoid tabs inside tabs. If a tab needs its own sub-navigation, it probably deserves its own page with a list-detail layout. Example: Car → Versions shows a list of versions, and each version page carries Aero, 3D viewer and Rules check.
- "3D viewer" and "Rules check" are tools, not content views. Consider presenting them as actions or side panels on a specific car version rather than as sibling tabs.

### Gaps
- I found no quantitative study on the maximum number of in-page tabs, or on whether remembering the last-used view helps. I couldn't verify how Asana or Linear persist views.

---

## Q4. Command palettes (⌘K) and search

### Takeaway
The best command palettes put navigation, record search and actions in one box that knows where you are. They offer prefixes as optional shortcuts and teach keyboard shortcuts as you use them. They add to visible navigation and a visible search field; they don't replace them. I found no public adoption data. For a mixed-age audience, show the palette as a visible search field and button rather than as a hidden shortcut.

### Cited Findings
- [Product] GitHub's command palette (documented as beta):
  - Open it with Ctrl/⌘+K or Ctrl+Alt/⌘+Option+K. Users can change the shortcut in their Accessibility settings.
  - It has three modes:
    - **Navigation** (the default).
    - **Search**, with prefixes: `#` issues, pull requests and discussions; `@` users and organisations; `/` files; `!` projects.
    - **Commands**, opened with `>` or Ctrl/⌘+Shift+K.
  - It "shows your location at the top left and uses it as the scope for suggestions". Issue and pull-request commands act on the current page.
  - Commands are grouped as global, organisation, repository, file, discussion, issue and pull request.

  — [GitHub Docs: Command Palette](https://docs.github.com/en/get-started/accessibility/github-command-palette) (read via [source file](https://github.com/github/docs/blob/main/content/get-started/accessibility/github-command-palette.md))
  - *Implication for SubOne:* Show the current team and section as the palette's scope. Support a few prefixes as optional shortcuts (`@` people, `#` tasks, `>` actions). Let users change the shortcut.
- [Product] Superhuman: "one shortcut rules them all: Cmd+K". It can run any action, and it shows the keyboard shortcut so you "learn the shortcut for next time". Its onboarding coaching sessions build keyboard habits on purpose. — [Superhuman blog: How to build a remarkable command palette](https://blog.superhuman.com/how-to-build-a-remarkable-command-palette/); [Superhuman onboarding](https://blog.superhuman.com/the-fastest-way-to-inbox-zero-a-single-coaching-session/) (summary). A secondary analysis argues that showing shortcuts next to commands teaches them passively. — [Blake Crosley on Superhuman](https://blakecrosley.com/guides/design/superhuman) (summary)
  - *Implication for SubOne:* Show each action's keyboard shortcut beside it in the palette, so frequent laptop users pick them up without training.
- [Expert] Command-palette pattern guides say:
  - Offer a consistent shortcut (⌘K / Ctrl+K) and a visible entry point, either a button or a search bar.
  - A palette is a keyboard-first launcher for actions, destinations and recent items. Add one only when there are enough actions to justify it.
  - A palette helps new and infrequent users discover features.

  — [uxpatterns.dev: Command Palette](https://uxpatterns.dev/patterns/advanced/command-palette); [uxpatterns.dev: Search field vs command palette](https://uxpatterns.dev/pattern-guide/search-field-vs-command-palette); [Medium: Command Palette UX Patterns](https://medium.com/design-bootcamp/command-palette-ux-patterns-1-d6b6e68f30c1); [UX Patterns (Outdraw)](https://outdraw-academy.gitbook.io/ux-patterns/command-palette) (summary)
- [Tested, indirect] In NN/g's navigation study, visible or combo navigation led more people to finish tasks without using search. — [NN/g](https://www.nngroup.com/articles/hamburger-menus/) (summary)
  - *Implication for SubOne:* Many people browse rather than search, so the palette complements the sidebar and tabs; it doesn't replace them.
- [Guideline] Apple (iOS 26): "A tab bar can include a dedicated search tab at the trailing end." — [Apple HIG: Tab bars](https://developer.apple.com/design/human-interface-guidelines/tab-bars) (read)
  - *Implication for SubOne:* On phones, give search a permanent entry point, such as a header button on every top-level screen or a search item. It should open a full-screen search-and-command sheet.

### Inferences
- **What SubOne's palette shows before anything is typed:**
  1. Recent records and pages.
  2. Suggested actions for the current section.
  3. "Go to…" all ~50 sections and tabs, with synonyms (for example "budget" → Money, "sponsors" → Marketing).
- **Once the user types:** results grouped by type (tasks, parts, events, sponsors, people, messages, files). The final fallback row is "Ask race engineer: ‹query›", so free-text questions go to the AI.
- **Actions to include:** New task, Log expense, Add sponsor, New event, Upload file, Message someone, Switch team, Change theme. Each shows its keyboard shortcut.
- **Discoverability:**
  - A visible "Search or jump to… ⌘K" field at the top of the sidebar.
  - Show Ctrl+K on Windows and ChromeOS. Many schools may use these; that is an assumption to check against analytics.
  - A one-time tip, and a "?" key that opens a shortcut cheat sheet.
- **Permissions:** results must respect roles. For example, students shouldn't see restricted Money records.

### Gaps
- I found no public usage or adoption numbers for command palettes (Linear, GitHub, VS Code, Raycast). I couldn't verify Raycast's or VS Code's documentation in this session.
- I couldn't retrieve the foundational research on why people rarely move from menus to keyboard shortcuts, or on techniques that speed up that shift.

---

## Q5. Creating and editing: quick capture, inline edit, dialogs vs side panels vs full pages, bottom sheets, undo, autosave

### Takeaway
Use the lightest container that fits the task:

| Task | Container |
|---|---|
| Changing a single field | Inline edit |
| Short creation or a confirmation | Modal dialog |
| Reviewing or editing records while keeping the list in view | Side ("peek") panel that doesn't block the page |
| Complex, multi-part records | Full page |

On phones, these become full-screen pages and bottom sheets. Prefer undo over "Are you sure?", and never mix autosave with a Save button in the same form.

### Cited Findings
- [Guideline] Apple on modal views:
  - Use them only when there is a clear benefit.
  - "Aim to keep modal tasks simple, short, and streamlined."
  - "Avoid creating a modal experience that feels like an app within your app."
  - Don't show a modal on top of another modal.
  - "Always give people an obvious way to dismiss a modal view."
  - If closing it "could result in the loss of user-generated content," explain the situation and give people ways to resolve it.

  — [Apple HIG: Modality](https://developer.apple.com/design/human-interface-guidelines/modality) (read)
  - *Implication for SubOne:* Editing in dialogs is fine for short records, such as a task, an expense or a sponsor contact. Rich records should move to full pages: car versions with the 3D viewer, pitch decks, portfolio pages.
- [Guideline] Apple on sheets:
  - Use sheets for scoped tasks. For "complex or prolonged user flows", use a full-screen modal instead.
  - Sheets rest at set heights: medium is about half the screen, large is full height. Compose sheets such as Mail use full height only.
  - Include a grabber so people can see the sheet resizes.
  - Support swiping down to dismiss. If there are unsaved changes, confirm with an action sheet.
  - Show only one sheet at a time.
  - Pair Done with Cancel (or Back), but never show all three.
  - Sheets that don't block the page suit tools that act on it, like formatting controls in Notes.

  — [Apple HIG: Sheets](https://developer.apple.com/design/human-interface-guidelines/sheets) (read)
- [Expert] NN/g on bottom sheets:
  - They are partial overlays for contextual details or controls, a form of progressive disclosure.
  - They are "not suited for displaying always needed information or tools".
  - They can block the page or not.
  - The common argument that they improve reachability is "largely incorrect".

  — [NN/g: Bottom Sheets](https://www.nngroup.com/articles/bottom-sheet/) (summary)
  - *Implication for SubOne:* On phones, use sheets for quick actions, filters and short forms. Use full pages for records people spend time in.
- [Guideline] Android's standard layouts:
  - **List-detail:** compact and medium windows show the list or the detail; expanded windows show both side by side.
  - **Supporting pane:** the main pane takes about 2/3 and the supporting pane about 1/3. Compact: supporting content goes in a sheet or below the main content. Medium: 50/50. Expanded: about 70/30.

  — [Android Developers: Canonical layouts](https://developer.android.com/develop/adaptive-apps/guides/canonical-layouts) (read)
  - *Implication for SubOne:* A task, sponsor or parts list with a detail panel on the right on wide screens is the list-detail layout. On phones, the detail becomes its own page. The race-engineer panel fits the supporting-pane layout.
- [Expert, foundational] Confirmation vs undo:
  - NN/g: don't overuse confirmation dialogs, and make them specific enough that users know what they are agreeing to. — [NN/g: Confirmation Dialogs](https://www.nngroup.com/articles/confirmation-dialog/) (summary)
  - Aza Raskin: "Never use a warning when you mean undo." — [A List Apart (2007)](https://alistapart.com/article/neveruseawarning/) (summary)
  - MSDN Magazine: routine confirmations become useless because people click through them on autopilot. — [MSDN Magazine (2005): To Confirm is Useless, to Undo Divine](https://learn.microsoft.com/en-us/archive/msdn-magazine/2005/march/%7B-end-bracket-%7D-to-confirm-is-useless-to-undo-divine) (summary)
  - *Implication for SubOne:*
    - Delete, archive or move a task, reorder items, mark done: act immediately and show an Undo toast.
    - Keep confirmation dialogs for irreversible, high-stakes actions: delete a team, remove a member, delete financial records. Name the object in the dialog.
- [Guideline] Primer on saving:
  - Use explicit save for inputs people fill in and review (text fields, checkboxes, radios, multi-selects).
  - Use automatic save for controls where people expect an instant effect (toggles, segmented controls, single-select dropdowns).
  - "Avoid mixing explicit and automatic save patterns on a single page with multiple forms, and never mix save patterns in a single form."
  - With autosave, "it should be obvious whether or not it saved".
  - Warn before navigating away with unsaved changes (the browser's `beforeunload` event).
  - Primer avoids toasts on github.com because of accessibility issues. This conflicts with the common undo-toast advice above; see the accessibility notes in Q9.

  — [Primer: Saving](https://github.com/primer/design/blob/main/content/ui-patterns/saving.mdx) (read)
  - *Implication for SubOne:* Autosaving peek panels show a "Saving… / Saved" status. Dialogs keep an explicit Save button. Never mix the two in one form.

### Inferences
- **Container rules for SubOne:**
  - **Inline:** status, assignee, due date and checkboxes directly in lists and boards.
  - **Modal dialog:** creating short records (about 5 fields or fewer), such as New task or Log expense, and confirming irreversible actions.
  - **Side peek (non-modal, wider screens, roughly 1024px and up):** opening any record from a list, board or calendar. Include next/previous, "Open as page", and per-field autosave.
  - **Full page:** car versions, pitch decks, portfolio pages, race-day plans, and anything with its own tabs.
  - **Phone:** records open as full-screen pages with a back button. Quick actions and filters go in half-height sheets; creation goes in a full-height sheet with Cancel and Save.
- **Quick capture:**
  - One global "+ New", available from the sidebar button, a palette action, and the phone header or a floating button.
  - It guesses the record type from the current section and pre-fills context: assignee = me, date = the selected or current day.
  - An inline "+ Add" row at the end of each list or board column.
  - Keep drafts when a dialog is dismissed, following Apple's data-loss guidance.
- **Race engineer:** a docked right-hand panel (about 30% wide) on desktop, and a full-height sheet on phones.

### Gaps
- I found no controlled study comparing modal dialogs, side panels and full pages for editing records; the guidance here is design-system consensus.
- I couldn't verify Linear's issue view, Asana's task pane, or Linear's and Todoist's quick-add details, including natural-language date entry.

---

## Q6. Personal home screens ("what needs me now")

### Takeaway
Leading home screens separate three things: "my work" (assigned items and due dates), "activity about me" (mentions and replies), and shortcuts or recents. They increasingly add an AI prompt box. The ones that avoid overload keep the screen short and mostly automatic, with light customisation.

### Cited Findings
- [Product] Asana Home is customisable. Users can drag, drop and resize widgets, including a snapshot of their tasks and a private notepad, add shortcuts to their most-used projects, tasks and forms, and change the background. It is available on desktop and mobile. — [Asana Help: Customize your Home](https://help.asana.com/s/article/how-to-customize-your-home-page); [Asana: Home features](https://asana.com/features/project-management/home) (summary). Users keep asking for more personal widgets, such as a pinned-tasks watchlist. — [Asana forum](https://forum.asana.com/t/home-tab-pinned-starred-tasks-widget-custom-watchlist/1139866) (summary)
- [Product] Slack's Activity view combines threads, mentions and reactions, each with its own sub-tab. Home keeps Unreads, Threads, and Drafts & sent at the top, and "Later" holds saved items. — [Engadget](https://www.engadget.com/slacks-latest-redesign-has-a-dedicated-dm-tab-and-a-discord-style-activity-view-130032154.html); [Computerworld](https://www.computerworld.com/article/2503287/how-to-use-slacks-new-interface.html) (summary)
- [Product] GitHub's personal dashboard contains:
  - **Recent activity:** "up to 4 updates made in the last two weeks".
  - **Top repositories:** generated automatically from commits, issues and pull-request activity. Users can't edit the list, and repositories drop off a year after the last activity.
  - **Feed:** activity from people you follow and repositories you watch.
  - **"For you":** recommendations.
  - **A new Home view (preview):** a Copilot prompt box, agent sessions, pull requests and assigned issues.

  Customisation is minimal. — [GitHub Docs: Personal dashboard (source file)](https://github.com/github/docs/blob/main/content/account-and-profile/reference/personal-dashboard.md) (read)
  - *Implication for SubOne:* GitHub's newest home pairs "assigned to me" lists with an AI prompt box, the same shape as SubOne's Today screen plus race engineer. Recents can be generated automatically; users don't need to curate them.

### Inferences
- **SubOne's Today screen:** one column on phones, two on desktop, with at most 5 modules:
  1. **Needs me.** My tasks that are overdue or due soon, items waiting for my approval (for teachers: expenses, submissions), and unread @mentions. Each can be acted on in place: done, snooze, open.
  2. **Next milestone.** A countdown to the next race or competition deadline, with checklist progress.
  3. **Team pulse.** The 3–5 latest meaningful updates, not a full feed.
  4. **Race engineer.** A prompt box with 2–3 suggestions based on context.
  5. **Jump back in.** Recent and pinned items.
- Set defaults for each role (student, team lead, teacher or mentor). Allow show, hide and reorder rather than Asana's free-form widget canvas; a canvas adds setup work that teens are unlikely to do (an inference).
- Keep notifications (Inbox/Activity) separate from the Today plan, as Slack and GitHub do. Make "all clear" feel rewarding.

### Gaps
- I couldn't verify Linear's Inbox and My Issues or Notion Home (blocked, and no search budget left).
- I found no study measuring when home dashboards overwhelm people versus help them.

---

## Q7. Responsive and adaptive layouts (phone → tablet → desktop) and PWA concerns

### Takeaway
Adapt layouts to the available window width, not the device type. Material's width breakpoints (600, 840, 1200 and 1600dp) map cleanly onto:
- navigation: bottom bar → side rail → full sidebar;
- content: single pane → list-detail → list-detail plus a supporting pane.

Apple says to keep functionality identical across sizes while switching between tab bar and sidebar. For a PWA:
- installation differs by platform: Chrome/Edge show an install prompt, while iPhone users install from the Share menu;
- the notch and home-indicator areas (safe areas) and the browser's pull-to-refresh need explicit handling.

### Cited Findings
- [Guideline] Android window size classes, from [Android Developers: Use window size classes](https://developer.android.com/develop/ui/compose/layouts/adaptive/use-window-size-classes) (read):

  **By width**

  | Class | Width | Typical devices |
  |---|---|---|
  | Compact | under 600dp | 99.96% of phones in portrait |
  | Medium | 600–840dp | 93.73% of tablets in portrait; most large unfolded foldables in portrait |
  | Expanded | 840–1200dp | 97.22% of tablets in landscape |
  | Large | 1200–1600dp | Large tablets |
  | Extra-large | 1600dp and up | Desktop displays |

  **By height:** compact is under 480dp (99.78% of phones in landscape); medium 480–900dp; expanded 900dp and up. Consider height too, because a landscape phone is compact in height and a two-pane layout won't fit.
- [Guideline] Android's adaptive navigation component (`NavigationSuiteScaffold`) uses a navigation bar when width or height is compact, or the device is in tabletop posture. It uses a navigation rail otherwise. A permanent drawer is a custom choice for expanded widths. — [Android Developers: Build adaptive navigation](https://developer.android.com/develop/ui/compose/layouts/adaptive/build-adaptive-navigation) (read)
- [Guideline] Material 3 Expressive (May 2025):
  - "The navigation drawer is being deprecated." Its replacement, the **expanded navigation rail**, "adapts better across window size classes." — [Material Components: Navigation drawer](https://github.com/material-components/material-components-android/blob/master/docs/components/NavigationDrawer.md) (read); [9to5Google](https://9to5google.com/2025/05/14/material-3-expressive-navigation/) (summary)
  - The bottom bar's height drops from 80dp to 64dp, and at 600dp and wider its items sit icon-beside-label. — [Material Components: Navigation bar](https://github.com/material-components/material-components-android/blob/master/docs/components/BottomNavigation.md) (read)
  - The collapsed rail holds 3–7 items. — [M3 Navigation rail](https://m3.material.io/components/navigation-rail/guidelines) (summary)
  - *Implication for SubOne:* At medium widths, a rail with 7 or fewer items can't show all 11 sections flat. Show the personal items and group headers, or make the rail expandable, and fall back to a modal list.
- [Guideline] Material defines three standard layouts: list-detail, supporting pane, and feed. A feed is a single scrolling column on compact windows and a multi-column grid on wider ones. — [Android Developers: Canonical layouts](https://developer.android.com/develop/adaptive-apps/guides/canonical-layouts) (read); [M3 Canonical layouts](https://m3.material.io/foundations/layout/canonical-examples/overview) (summary)
- [Guideline] Apple on layout:
  - "Determine layout based on size classes, not device type or orientation."
  - "Don't change your app's functionality based on the space it occupies"; you can change how much is visible.
  - On larger screens, consider switching from a tab bar to a sidebar.
  - Respect safe areas.
  - Support larger system text sizes (Dynamic Type), for example by stacking side-by-side views vertically as text grows.

  — [Apple HIG: Layout](https://developer.apple.com/design/human-interface-guidelines/layout) (read)
- [Guideline] Apple's current tab bars:
  - **iPad:** the tab bar sits near the top and can turn into a sidebar, and people can customise it.
  - **iPhone (iOS 26):** the tab bar floats over content with the new translucent ("Liquid Glass") style. It can shrink when people scroll down, keeping a small strip (an "accessory") visible above it, and it can have a dedicated search tab at its trailing end.

  — [Apple HIG: Tab bars](https://developer.apple.com/design/human-interface-guidelines/tab-bars) (read). Apple uses the accessory strip for mini-players and global status. — [Donny Wals](https://www.donnywals.com/exploring-tab-bars-on-ios-26-with-liquid-glass/); [jorgemrht.dev](https://jorgemrht.dev/2025/09/18/liquid-glass-tab-bar) (summary)
  - *Implication for SubOne:* A slim "race day live" or active-timer strip, or a race-engineer entry, sitting above the phone's bottom bar follows a pattern Apple itself uses.
- [Guideline] Installing a PWA, per MDN:
  - **Requirements:** a web app manifest with a name or short_name, icons (192px and 512px), start_url, display or display_override, and prefer_related_applications false or absent; plus HTTPS. A service worker is optional for installing but is used for offline support.
  - **Where install happens:**
    - Chrome and Edge on desktop: an install icon in the address bar.
    - Safari on macOS Sonoma and later: "Add to Dock".
    - Firefox desktop: no manifest-based install.
    - Android: Chrome and Samsung Internet install it as a real app (a WebAPK); other browsers add a home-screen shortcut.
    - iOS and iPadOS 16.4 and later: install through the Share menu in Safari, Chrome, Edge, Firefox or Orion.
  - `"display": "standalone"` makes the app look native, without browser controls.

  — [MDN: Making PWAs installable](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Guides/Making_PWAs_installable) (read via [source file](https://github.com/mdn/content/blob/main/files/en-us/web/progressive_web_apps/guides/making_pwas_installable/index.md))
- [Guideline] MDN on the custom install prompt: the `beforeinstallprompt` event is non-standard and experimental. The pattern is to suppress the browser's own prompt, keep the event, show your own Install button, call `prompt()` when it is clicked, and read the user's choice. — [MDN: beforeinstallprompt](https://developer.mozilla.org/en-US/docs/Web/API/Window/beforeinstallprompt_event) (read via [source file](https://github.com/mdn/content/blob/main/files/en-us/web/api/window/beforeinstallprompt_event/index.md))
  - *Implication for SubOne:* Build two install paths. On Chrome, Edge and Android, show a custom Install button after the person has seen value, for example when they turn on chat notifications. On iPhone and iPad, show illustrated "Share → Add to Home Screen" steps.
- [Guideline] MDN on safe areas: the CSS `safe-area-inset-*` variables mark a rectangle clear of notches and rounded corners; they are 0 on plain rectangular screens. Example: a sticky footer with `padding-bottom: calc(1em + env(safe-area-inset-bottom, 1em))`. There are also `keyboard-inset-*` variables (on-screen keyboard) and `titlebar-area-*` variables (installed desktop PWAs). — [MDN: Using environment variables (source file)](https://github.com/mdn/content/blob/main/files/en-us/web/css/guides/environment_variables/using/index.md) (read)
- [Guideline] MDN on scroll edges: the CSS property `overscroll-behavior: contain` stops scrolling from spilling into the page behind. It also "disables native browser navigation, including the vertical pull-to-refresh gesture and horizontal swipe navigation". Put it on `<html>` to block page-level refresh, or on dialogs and panels to stop the background scrolling. — [MDN: overscroll-behavior (source file)](https://github.com/mdn/content/blob/main/files/en-us/web/css/reference/properties/overscroll-behavior/index.md) (read)

### Inferences
- **SubOne breakpoints** (CSS pixels map closely to dp):

| Width | Typical device | Navigation | Content layout |
|---|---|---|---|
| < 600 | Phones | Bottom bar (4 + More), labelled | Single pane; records open as pages; filters and quick actions in sheets; AI in a full-height sheet |
| 600–839 | Tablet portrait, half-screen laptop windows | Rail with labels, or collapsed sidebar | List *or* detail (50/50 if the list is short) |
| 840–1199 | Tablet landscape, small laptops | Collapsible sidebar (or rail) | List-detail in two panes; AI panel overlays content |
| ≥ 1200 | Laptops and desktops | Full grouped sidebar | List + detail/peek; AI race engineer docked on the right (~30%) |

- Keep the same features and names at every size; change only how much is visible (Apple).
- For iOS web apps, the standard practice is to add `viewport-fit=cover` to the viewport meta tag so the safe-area insets take effect, then pad the bottom bar with `env(safe-area-inset-bottom)`. The requirement itself wasn't in the MDN text I retrieved, so check it.
- Offline: cache the app shell plus Today and Plan data for reading, queue edits, and show a visible sync status. This is a common PWA pattern, but I didn't verify a source for it.

### Gaps
- I couldn't verify two iPhone details:
  - Whether web push on iPhone requires the app to be installed to the home screen.
  - Whether iOS 27, expected September 2026, changed tab bars or Liquid Glass. Only leaks surfaced, and they are speculative.
- I found no data on how often custom PWA install prompts lead to installs.
- The m3.material.io details (rail of 3–7 items; more than 5 destinations → modal expanded rail) were seen only through search summaries.

---

## Q8. Phone-specific patterns for teens: reach, gestures, sticky actions, sheets, pull to refresh

### Takeaway
Platform guidance favours large, well-spaced, labelled touch targets (Apple's default is 44pt). Gestures should always have a visible alternative. Show one sheet at a time, dismissable by swiping down. Keep navigation persistent. The claim that the bottom of the screen is always easiest to reach is weaker than popular "thumb zone" advice suggests. **I could not retrieve teen-specific UX research in this session.**

### Cited Findings
- [Expert] NN/g: the common argument that bottom sheets improve reachability is "largely incorrect" because "users hold mobile devices in a variety of ways". — [NN/g: Bottom Sheets](https://www.nngroup.com/articles/bottom-sheet/) (summary)
  - *Implication for SubOne:* Put navigation at the bottom because it is the convention and stays visible, not because of "thumb reach" alone. Primary actions can sit top-right or bottom, as long as they are consistent.
- [Guideline] Apple on touch targets and gestures:
  - Controls are 44×44pt by default, with 28×28pt as the minimum (iOS and iPadOS).
  - Leave about 12pt of padding around controls with a visible border or background, and about 24pt around those without.
  - "If you use a swipe gesture to dismiss a view, also make a button available."
  - Use the simplest gesture for frequent actions, and avoid custom multi-finger gestures.

  — [Apple HIG: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) (read)
- [Standard] WCAG 2.2 success criterion 2.5.8, Target Size (Minimum), Level AA: targets must be at least **24×24 CSS pixels**, or spaced so that a 24px circle centred on each one doesn't overlap another target. Exceptions cover inline links in text, unmodified browser controls, and cases where size is essential. Aim for the stricter 2.5.5 criterion for important controls. — [W3C Understanding 2.5.8](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html) (read via [source file](https://github.com/w3c/wcag/blob/main/understanding/22/target-size-minimum.html))
  - *Implication for SubOne:* Make bottom-bar items and primary buttons at least 44px, well above the 24px legal floor, since younger students and phones used on the move need generous targets.
- [Guideline] Apple on sheets: people expect to swipe down to dismiss; include a grabber; confirm before discarding unsaved changes; show one sheet at a time. — [Apple HIG: Sheets](https://developer.apple.com/design/human-interface-guidelines/sheets) (read)
- [Guideline] Apple: keep the tab bar visible when moving between sections; the exception is a modal covering it. iOS 26 allows it to shrink on scroll. — [Apple HIG: Tab bars](https://developer.apple.com/design/human-interface-guidelines/tab-bars) (read)
- [Guideline] The CSS property `overscroll-behavior` controls the browser's native pull-to-refresh. — [MDN (source file)](https://github.com/mdn/content/blob/main/files/en-us/web/css/reference/properties/overscroll-behavior/index.md) (read)
- [Product] Discord's backlash shows that heavy chat users react strongly when tabs they rely on disappear or a one-tap action becomes two taps. — [remio.ai](https://www.remio.ai/post/discord-redesign-backlash-reveals-mobile-app-tradeoffs) (summary)
  - *Implication for SubOne:* Chat should be one tap from anywhere on the phone, which supports giving it a bottom-bar slot.

### Inferences
- Keep labels under bottom-bar icons, and make targets at least 44px.
- Pin the primary button (Save, Send, Log) to the bottom of long forms and sheets. Pad it for the safe area and the on-screen keyboard, and make sure it never covers the focused field (WCAG 2.4.11; see Q9).
- Offer pull-to-refresh on Today, Chat and feed-style lists, with live updates as the default. Turn off the browser's own pull-to-refresh inside chat scrollers, sheets and panels so a stray swipe doesn't reload the app.
- Swipe actions, such as swiping a task to complete it, should only be shortcuts; always have a visible button for the same action.
- Don't hide the bottom bar on scroll, except in immersive views like the full-screen 3D viewer. Shrinking it in the iOS 26 style is acceptable.
- School context to check: shared or school-managed devices, strict content filters, and limited mobile data may shape offline and install behaviour. These are assumptions, not findings.

### Gaps
- I couldn't access NN/g's research on teenage users, Pew or Ofcom statistics on teen device use, or Steven Hoober's observations of how people hold phones. There are no verified teen-specific findings here on expectations of app-like web apps, gesture discoverability, or preferences.
- There is also no verified data on how well gestures or pull-to-refresh are discovered by this age group.

---

## Q9. Keyboard shortcuts and accessibility of navigation (skip links, landmarks, focus management)

### Takeaway
Palettes and shortcuts must meet WCAG:
- single-key shortcuts need a way to turn them off or change them;
- repeated navigation needs a way to skip past it;
- sticky bars must not hide the focused element;
- modal dialogs must move keyboard focus in, keep it inside, and return it on close.

Side panels that don't block the page should not trap focus.

### Cited Findings
- [Standard] WCAG 2.1.4 Character Key Shortcuts (Level A): if a shortcut uses only letter, number, punctuation or symbol keys, users must be able to turn it off, or remap it to include a modifier key such as Ctrl, or it must only work when the relevant component has focus. The reasons: "Single-key shortcuts are disastrous for speech users", whose spoken words can trigger commands, and people with dexterity difficulties hit keys by accident. — [W3C Understanding 2.1.4](https://www.w3.org/WAI/WCAG22/Understanding/character-key-shortcuts.html) (read via [source file](https://github.com/w3c/wcag/blob/main/understanding/21/character-key-shortcuts.html))
  - *Implication for SubOne:* Linear-style single-letter shortcuts (such as `C` to create, `G` then `P` to go to Plan) are allowed only with a setting to turn them off or remap them. ⌘K / Ctrl+K is fine because it uses a modifier.
- [Standard] WCAG 2.4.1 Bypass Blocks (Level A): give people a way to skip blocks that repeat on every page, such as navigation. This helps screen-reader users avoid hearing "dozens of navigation links on every page", and lets keyboard and screen-magnifier users reach content faster. — [W3C Understanding 2.4.1](https://www.w3.org/WAI/WCAG22/Understanding/bypass-blocks.html) (read via [source file](https://github.com/w3c/wcag/blob/main/understanding/20/bypass-blocks.html)); the list of recommended techniques (skip links, headings, page regions) was not in the text I retrieved.
- [Standard] WCAG 2.4.11 Focus Not Obscured (Minimum) (AA): "when an item gets keyboard focus, it is at least partially visible." Sticky headers and footers and non-modal dialogs are the usual culprits. Fixes:
  - Add scroll padding so focused items aren't scrolled under a sticky bar.
  - Make overlays modal.
  - Have panels push content aside rather than cover it.
  - Allow Escape to dismiss.

  — [W3C Understanding 2.4.11](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum.html) (read via [source file](https://github.com/w3c/wcag/blob/main/understanding/22/focus-not-obscured-minimum.html))
  - *Implication for SubOne:* The sticky header, the phone bottom bar, sticky Save buttons and the peek panel need CSS `scroll-padding`. The peek panel should push the list aside rather than overlap it.
- [Standard] W3C's ARIA Authoring Practices, modal dialog pattern:
  - **When it opens,** move focus into the dialog, usually to the first focusable element. If the content is long or structured, focus a static element at the start instead. If the action is irreversible, focus the least destructive option.
  - **While open,** Tab and Shift+Tab cycle within the dialog, and Escape closes it.
  - **On close,** focus returns to the element that opened it, unless that element no longer exists.
  - **Markup:** `role="dialog"`, `aria-modal="true"`, and a label via `aria-labelledby` or `aria-label`.

  — [WAI-ARIA APG: Dialog (Modal)](https://www.w3.org/WAI/ARIA/apg/patterns/dialog-modal/) (read via [source file](https://github.com/w3c/aria-practices/blob/main/content/patterns/dialog-modal/dialog-modal-pattern.html))
- [Guideline] Apple: let people use the keyboard alone ("Full Keyboard Access"), and "avoid overriding system-defined keyboard shortcuts." — [Apple HIG: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) (read)
- [Product] GitHub lets users change the command-palette shortcut in their Accessibility settings. — [GitHub Docs (source file)](https://github.com/github/docs/blob/main/content/get-started/accessibility/github-command-palette.md) (read)
- [Guideline] Primer avoids toasts on github.com because of accessibility issues. — [Primer: Saving](https://github.com/primer/design/blob/main/content/ui-patterns/saving.mdx) (read). This conflicts with the common advice to show undo in a toast (NN/g, A List Apart; Q5).

### Inferences
- **Page structure:** mark up the page regions for screen readers: header (team switcher and search); navigation (sidebar or bottom bar, each labelled); main content; and a complementary region (peek or AI panel). Put a "Skip to content" link first. Mark the active nav item with `aria-current`. All of this is standard practice, though I didn't verify it from W3C technique pages here.
- **Peek panels:** they don't trap focus, but focus moves into the panel when it opens and back to the originating row when it closes. Escape closes it. Provide a keyboard shortcut to jump between the list and the panel.
- **Undo toasts, if used:**
  - Announce them to screen readers without stealing focus (a `role="status"` live region).
  - Keep them up long enough, and pause the timer on hover or focus.
  - Make Undo reachable by keyboard, and also available from the command palette ("Undo last action").

  This responds to Primer's accessibility concern.
- **Shortcut help:** a "?" shortcut sheet, shortcuts shown inside the palette, and a setting to turn off single-key shortcuts.

### Gaps
- The text I retrieved didn't include W3C's specific techniques for skip links and page regions; I didn't fetch the ARIA landmark guidance.
- I found no data on how often students use keyboard navigation or assistive technology. SubOne's own analytics or school accessibility requirements would be needed.
