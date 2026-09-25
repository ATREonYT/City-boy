# Youth/school team apps, sports team apps, performance and telemetry apps, and robotics data tools: what each does best, as models for SubOne

> **Method note (applies to every section).** Researched 25 Sep 2026. The session's egress policy blocked WebFetch on every host tried (help.spond.com, uscenterforsafesport.org, sportsengine.com, help.gc.com, help.remind.com, statbotics.io). The session-wide WebSearch budget, which is shared across the session, also ran out partway through this assignment, after about 50 queries. Every finding below therefore comes from search-engine extracts of the linked pages, not from reading the pages in full. Spot-check prices, counts and percentages on the linked page before quoting them.
>
> - "(vendor claim)" marks a company describing itself.
> - Facts I could only supply from background knowledge appear under **Gaps** as "unverified". They are never listed as findings.
> - Each "*Implication for SubOne*" line is a recommendation, not a sourced fact.

## Q1. Roles and safeguarding: how youth and school apps handle students, coaches/teachers and parents, and what schools and clubs require

### Takeaway
Sport-body rules and the better apps have settled on one pattern:
- No private adult-to-minor channel. Every adult–child message is visible to a second adult or to the parent.
- Younger children's accounts are guardian-linked. Under-13s receive messages but do not send them, or they act through a parent.
- Under-18s get high-privacy defaults: visible to followers only, no DMs, kept off public leaderboards.
- Message history cannot be edited or deleted.
- A teacher approves a child's content before it reaches families or the public.

The bar rose in 2025–26. Compliance with the amended US COPPA rule became mandatory in April 2026. ClassDojo and Google opened teacher-to-student messaging and AI for teens only behind admin switches, logging, scanning and teacher-chosen content.

### Cited Findings

**Rules SubOne's users already operate under**
- **US Center for SafeSport, Minor Athlete Abuse Prevention Policies (MAAPP):**
  - Electronic communication with minor athletes must be open and transparent.
  - An adult's message to more than one minor must copy another adult participant, or all the minors' parents/guardians.
  - If a parent is copied, a parent must be copied for every minor on the team.
  - Sources: [U.S. Center for SafeSport: communicate safely with minor athletes](https://uscenterforsafesport.org/how-to-safely-communicate-with-minor-athletes/); [MAAPP Electronic Communications one-pager (PDF)](https://uscenterforsafesport.org/wp-content/uploads/2021/03/MAAPP_OnePagers_Communication.pdf)
  - Clubs put this into practice through app configuration. One club's June 2025 "Communication Policy – SafeSport Compliance" is a how-to-use-TeamSnap guide — [TBK policy (PDF, 2025)](https://www.teambrecksportsclub.com/wp-content/uploads/sites/2330/2025/06/How-to-use-TeamSnap.pdf).
  - Vendors such as CrewLAB and Onform sell "SafeSport-compliant" messaging as a feature — [CrewLAB](https://crewlab.io/blog/how-do-clubs-keep-athlete-communication-safesport-compliant/); [Onform](https://onform.com/blog/staying-safesport-compliant-with-onform/)
- **UK CPSU (NSPCC Child Protection in Sport Unit), WhatsApp guide:** coaches and leaders should not message any child directly in an individual chat. A group chat with under-18s needs:
  - an in-person discussion with parents and young people about safe use and a code of conduct;
  - two monitoring staff, both DBS-checked, safely recruited and trained in basic safeguarding;
  - a staff code of conduct and an online-safety policy;
  - signposting of online-safety resources for young people.
  - Sources: [CPSU: WhatsApp go-to guide for sports](https://thecpsu.org.uk/resource-library/tools/whatsapp-go-to-guide-for-sports/); [FAW safeguarding: communication](https://faw.cymru/safeguarding/communication/)
- **FIRST Youth Protection Program (robotics; the closest analogue to STEM Racing):**
  - Coaches and mentors should not start electronic contact with students unless it concerns a FIRST project or activity.
  - Direct messages through social media or unofficial platforms are discouraged; teams should use official systems.
  - Parents/guardians and other mentors should be included "whenever possible/practical".
  - From the 2026–27 season, more team roles require YPP clearance.
  - Sources: [FIRST YPP](https://www.firstinspires.org/programs/youth-protection-program); [FIRST YPP Program Guide (PDF)](https://www.firstinspires.org/hubfs/web/about/policy/FIRST-YPP-ProgramGuide.pdf?hsLang=en); [FIRST: key YPP updates](https://community.firstinspires.org/updates-to-first-youth-protection-for-mentors-volunteers)
  - *Implication for SubOne:* make the rule these three bodies share the default in Chat:
    - no 1:1 threads between an adult and a student;
    - any thread containing an adult and a student must include a second adult, or be visible to all team adults;
    - an optional "copy guardians" mode copies every student's guardian, never just some.
- **US COPPA amendments:** published 22 Apr 2025, in force 23 Jun 2025, compliance required by 22 Apr 2026. The changes:
  - "Personal information" now includes biometric identifiers.
  - Disclosure to third parties needs separate verifiable parental consent.
  - New data-retention requirements.
  - New obligations for the "support for internal operations" exception.
  - More prescriptive security requirements.
  - Sources: [Federal Register, 22 Apr 2025](https://www.federalregister.gov/documents/2025/04/22/2025-05904/childrens-online-privacy-protection-rule); [Mayer Brown](https://www.mayerbrown.com/en/insights/publications/2025/04/ftc-announces-significant-amendments-to-coppa); [Latham & Watkins](https://www.lw.com/en/insights/ftc-publishes-updates-to-coppa-rule); [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/coppa-rule-amendment-compliance-deadline-approaches)
- **UK ICO Children's Code (Age Appropriate Design Code), which applies to edtech:**
  - Settings must be "high privacy" by default, with geolocation and profiling off by default.
  - No "nudge techniques" that lead children to give unnecessary data or weaken their privacy. The ICO's example is a large green "yes" beside a small "no".
  - Collect and keep the minimum data.
  - Privacy information must be concise and suited to the child's age.
  - Sources: [ICO standard 13: nudge techniques](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/age-appropriate-design-a-code-of-practice-for-online-services/13-nudge-techniques/); [ICO: protect children's privacy by default](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/designing-products-that-protect-privacy/childrens-code-design-guidance/protect-children-s-privacy-by-default/); [ICO: introduction to the Children's code](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/introduction-to-the-childrens-code/); [Stevens & Bolton: Children's code and edtech](https://www.stevens-bolton.com/site/insights/articles/ico-the-childrens-code-and-education-technologies-edtech)
  - *Implication for SubOne:*
    - Publish a short data-retention schedule, for example archive at season end and delete after a stated period.
    - Document "no third-party disclosure" as a default.
    - Write the privacy text for 11–13-year-olds.
    - SubOne's choice of no streaks and no points already meets the ICO's anti-nudge standard; say so in material aimed at schools.
- **Aspen Institute national youth-sports parent survey (fall 2024, 1,848 parents):**
  - 94% of parents prefer background checks for coaches.
  - More than half say a trustworthy coach would raise their enthusiasm to commit their child long-term.
  - Sources: [Aspen Institute survey (PDF, 2025)](https://www.aspeninstitute.org/wp-content/uploads/2025/06/National-Youth-Sports-Parent-Survey-FINAL.pdf); [Project Play: State of Play 2024 coaching trends](https://projectplay.org/state-of-play-2024-coaching-trends)
  - *Implication for SubOne:* show each adult's role and who vouched for them in Team and Chat, for example "Teacher, confirmed by school admin" or "Mentor, invited by Ms X". SubOne cannot run background checks, but it can make vouching visible.

**How the youth and school apps design roles**
- **Spond:**
  - Group types: a "children/youth" group gives children no profile of their own; a "mixed" group gives profiles to both children and guardians — [Spond Help: parents and children](https://help.spond.com/app/en/articles/139608-parents-and-children-in-spond).
  - Younger children are added with no email or phone; contact details sit on the guardian. One guardian profile can respond for unlimited children across groups — [Spond Help: correct registration](https://help.spond.com/app/en/articles/301491-correct-registration-of-children-and-guardians-in-spond-app).
  - Every junior member is linked to at least one verified guardian, who sees communication, event invites and payment tracking.
  - Messages, events and responses are "channelled through the guardian", with two-way communication only "with full oversight" in the team context.
  - Spond claims GDPR and COPPA compliance (vendor claim).
  - Sources: [Spond: parental control features](https://www.spond.com/news-and-blog/parental-control-features/); [Spond: Add Guardians](https://www.spond.com/news-and-blog/add-guardians-spond-safeguarding-and-transparency/); [Spond: child-safe sports team app](https://www.spond.com/en-us/news-and-blog/child-safe-sports-team-app/); [Spond Help: safeguarding in Spond](https://help.spond.com/app/en/articles/291678-safeguarding-in-spond)
  - *Implication for SubOne:* let a teacher create email-less student profiles, linked to a guardian email, for the youngest members (11–12). Offer a "mixed" mode in which students aged 13+ hold full accounts.
- **TeamSnap:**
  - A Household Organizer (an adult) invites and removes family members.
  - Contacts added under a member's profile get the same access as that member.
  - Siblings are separate roster spots under one login.
  - Sources: [TeamSnap: add family or contacts](https://helpme.teamsnap.com/article/108-add-family-or-contacts-to-a-profile); [siblings / multiple roster spots](https://helpme.teamsnap.com/article/280-set-up-multiple-roster-spots-on-a-team); [account settings](https://helpme.teamsnap.com/article/1229-managing-your-teamsnap-account-settings)
- **Heja:**
  - Player and Parent are separate roles.
  - A parent requests connection to a listed child, and an existing parent/guardian or team admin must approve it.
  - Heja collects phone number, name and date of birth, plus any child information parents supply.
  - Sources: [Heja Help: parent account](https://help.heja.io/en/articles/9618901-setting-up-your-parent-account-on-heja-connecting-to-your-child-team); [Heja Help: Player to Parent role](https://help.heja.io/en/articles/2465240-change-from-the-player-to-parent-role); [Heja privacy](https://heja.io/privacy)
  - *Implication for SubOne:* a guardian link should need approval from the teacher or an existing guardian, not just self-declaration.
- **GameChanger:**
  - Staff set the live-stream audience: anyone with the link, or only confirmed team family and fans.
  - Staff also set who may stream: "Only Staff" or "Confirmed Members".
  - Team stats have three privacy levels:
    - Fan Access: anyone.
    - Confirmed – Team: confirmed family and players.
    - Confirmed – Player: confirmed family and players see only their own player's stats.
  - Sources: [GC: Team Stats Privacy Settings](https://help.gc.com/hc/en-us/articles/360038142452-Team-Stats-Privacy-Settings); [GC: live-streaming permissions](https://gc.com/post/family-and-player-live-streaming); [GC: scorekeeping and live-streaming permissions](https://help.gc.com/hc/en-us/articles/33827901166605-Scorekeeping-and-Live-Streaming-Permissions); [GC: Team Roles](https://help.gc.com/hc/en-us/articles/42602635189901-Team-Roles)
  - *Implication for SubOne:* give race data, photos and video a three-level visibility switch: team only / team + guardians / public share link. Add a "guardians see only their own child" option, and default to team only.
- **SportsEngine:**
  - SportsEngine HQ added team chat.
  - Help pages cover guardians taking part in team chat and moderating chat media. A community thread covers adding teenage children to the app.
  - I found no named "Rule of Three" feature.
  - Sources: [SportsEngine HQ: team chat update](https://www.sportsengine.com/blog/sportsengine-hq-product-update-team-chat/); [SE Mobile: moderate team chat media](https://mobile-help.sportsengine.com/en/articles/8264227-how-to-interact-with-and-moderate-team-chat-media); [SportsEngine Community: adding teenage kids](https://community.sportsengine.com/topic/781-adding-teenage-kids-to-the-app/)
- **BAND:**
  - Rated 12+, with a separate "BAND for Kids" app for ages 12 and under.
  - Accounts for ages 13–17 are private by default, with some features restricted.
  - A parent "Supervisor" setting can turn off discover/search and list the Bands the child belongs to.
  - Parental-control reviewers warn that public Bands can expose children to adult content. These sources are commercial parental-control vendors.
  - Sources: [Bark](https://www.bark.us/app-reviews/apps/band-app-review/); [BAND for Kids (App Store)](https://apps.apple.com/us/app/band-for-kids/id1527684503); [FamiSafe](https://famisafe.wondershare.com/app-review/band-app-review.html)
  - *Implication for SubOne:* keep workspaces invite-only, with no discovery, search or public directory of teams or students.
- **Remind:**
  - Two-way messaging is only for students aged 13+.
  - Under-13s must enter a parent/guardian email, need parent permission, and can only receive messages from teachers. The parent then receives all messages too.
  - Contact details stay private, because messages go through Remind numbers and emails.
  - Messages cannot be edited or deleted, every user can download their history, and anyone can report guideline violations.
  - Sources: [Remind: trust and safety](https://help.remind.com/hc/en-us/articles/203744719-Trust-and-safety-on-Remind); [Remind parent overview (PDF)](https://assets.remind.com/marketing/pdfs/remind-overview-parents.pdf); [Remind community guidelines](https://www.remind.com/terms/community-guidelines); [Tech & Learning](https://www.techlearning.com/how-to/what-is-remind-and-how-does-it-work-for-teachers)
  - A help article titled "Coming soon: I want to let students under 13 send messages at my school" signals a school-authorised opt-in — [Remind Help](https://help.remind.com/hc/en-us/articles/18336192636685-Coming-soon-I-want-to-let-students-under-13-send-messages-at-my-school)
  - *Implication for SubOne:*
    - an append-only chat log that the teacher can export;
    - hidden phone numbers and emails;
    - a report button;
    - for under-13s, receive-only or guardian-copied chat unless the school opts in.
- **Google Classroom:**
  - A teacher or admin invites guardians at any email address; the invitation must be accepted within 120 days.
  - Guardians choose daily or weekly automatic email summaries covering missing work, upcoming work and recent class activity (announcements, assignments, questions).
  - Summaries only work if the student uses a Workspace for Education account.
  - Sources: [Classroom Help: about guardian email summaries](https://support.google.com/edu/classroom/answer/6386354?hl=en); [get Classroom email summaries](https://support.google.com/edu/classroom/answer/6388136?hl=en); [guardian summaries FAQ](https://support.google.com/edu/classroom/answer/7126518?hl=en)
  - **Gemini in Classroom** (announced at ISTE, June 2025):
    - Students under 18 get a separate experience with extra content guardrails and AI-literacy resources.
    - Teachers can base the AI's answers on class materials they select, and can see how students engage.
    - Admins switch it on or off for the whole domain or for specific groups.
    - Google says the data is not human-reviewed or used to train models.
    - Sources: [Google blog: Gemini tools, ISTE 2025](https://blog.google/outreach-initiatives/education/gemini-iste-2025/); [Google for Education: Gemini](https://edu.google.com/intl/ALL_us/ai/gemini-for-education/); [Chrome Unboxed](https://chromeunboxed.com/gemini-is-now-available-for-all-education-users-with-extra-safeguards-for-younger-students/). Critical view: [Common Sense Youth AI Safety Institute](https://institute.commonsensemedia.org/what-to-know-about-google-turning-on-gemini-for-schools)
  - *Implication for SubOne:* the AI race engineer needs:
    - an on/off switch per team, controlled by the teacher or mentor;
    - answers grounded in the team's own data and the rulebook;
    - stricter content rules for under-18s;
    - a plain statement that student data is not used for training.
- **ClassDojo:**
  - Teacher-to-student messaging is piloting for high school. The help-page titles say grades 9–12 in one place and 6–12 in another.
    - Chats can be 1:1 or group.
    - District leaders turn it on or off; school leaders toggle it per school; teachers toggle it per class.
    - Teachers can download their own history, and school or district leaders can request it from ClassDojo support.
    - Quiet hours still apply.
    - Messages that include a student are automatically scanned for child-safety concerns, and flagged messages go to district or ClassDojo staff.
    - Sources: [ClassDojo: teacher-to-student messaging FAQ](https://help.classdojo.com/hc/en-us/articles/42702434157069-Teacher-to-Student-Messaging-FAQ-For-Teachers-and-School-Leaders); [student messaging (grades 6–12) FAQ](https://help.classdojo.com/hc/en-us/articles/42702434157069-Student-Messaging-for-grades-6-12-FAQ-For-Teachers-and-School-Leaders); [what school leaders can see and do](https://help.classdojo.com/hc/en-us/articles/207813176-What-Can-School-Leaders-See-and-Do)
  - Teachers set their own quiet hours for parent messages — [ClassDojo blog: quiet hours](https://blog.classdojo.com/introducing-quiet-hours-for-teachers/); [Help: set quiet hours](https://help.classdojo.com/hc/en-us/articles/207359446-How-to-Set-or-Edit-Quiet-Hours)
  - *Implication for SubOne:* a market leader opened 1:1 teacher–student chat only behind layered switches, logging and automated scanning. SubOne's simpler rule, no 1:1 adult–student DMs, is easier to defend to schools. Add quiet hours as a default, for example no student push notifications late at night.
- **Seesaw:**
  - Student work is private to the class by default.
  - Teachers can require approval before a student's post reaches the journal and connected family members.
  - Teachers decide whether families can view, like, share or comment, and whether students can see or comment on classmates' work.
  - Family members who join through an invite link need teacher approval.
  - Seesaw notes it cannot prevent screenshots.
  - Sources: [Seesaw: privacy for student journals](https://help.seesaw.me/hc/en-us/articles/203008899-Privacy-for-student-journals); [approving family connections](https://help.seesaw.me/hc/en-us/articles/204410545-Approving-Family-connections); [classroom privacy settings](https://help.seesaw.me/hc/en-us/articles/44428120804749-Managing-Classroom-Settings-for-Privacy); [Seesaw children's privacy policy](https://seesaw.com/privacy-policy/childrens-privacy-policy/)
  - *Implication for SubOne:* anything leaving the team goes through a teacher/mentor approval queue. That includes Marketing posts, sponsor emails, public portfolio and share links, and photos or video showing students.
- **Strava** (benchmark for how a performance app treats teens). For under-18 accounts created after 3 Sep 2021:
  - Only followers see the full profile, and new followers need approval.
  - Activities are visible only to followers and are kept off segment and challenge leaderboards.
  - The first and last 400 m of maps are hidden.
  - There is no access to Messaging.
  - Uploading or analysing heart-rate data requires age 16+.
  - Sources: [Strava Help: privacy defaults under 18](https://support.strava.com/hc/en-us/articles/4412328250893-Your-Privacy-Control-Defaults-When-You-re-Under-18-on-Strava); [Strava Help: under 16](https://support.strava.com/en-us/articles/15401925-can-i-use-strava-if-i-m-under-the-age-of-16); [Internet Matters: Strava](https://www.internetmatters.org/advice/apps-and-platforms/stay-active/strava/)
  - *Implication for SubOne:* no public student profiles, no location data, no biometric or health data. Reaction times are performance data, not health data, but keep them team-private by default.

### Inferences
- **Age bands differ by app.** The observed bands are:
  - under 13: guardian-mediated or receive-only (Remind, Spond);
  - 13–17: own account with restrictions (BAND, Remind);
  - 16+: Strava's heart-rate threshold;
  - 18+: adult.

  SubOne's 11–19 range crosses every band. It includes 18–19-year-old students who are legally adults on teams with minors, so SubOne needs a policy on whether adult students follow the "adult" chat rules. SafeSport-style rules would suggest yes.
- **The school is usually the gatekeeper.** STEM Racing teams are school-based, so the school's safeguarding lead, data-protection officer or IT approval process will probably decide adoption more than any sport body's rules. This is inferred from the edtech approval and overload findings in Q6.
- **The shared pattern can be published as a safeguarding checklist:**
  - adult–student chat in groups only;
  - two adults per thread;
  - optional guardian copy;
  - append-only, exportable log;
  - quiet hours;
  - teacher approval for public output;
  - invite-only spaces;
  - high-privacy defaults;
  - an admin switch for AI.

### Gaps
- **Full texts not read (fetch blocked):**
  - exact MAAPP exceptions, such as emergencies;
  - Spond's exact ages for own profiles and chat;
  - TeamSnap's and Heja's handling of under-13s and COPPA;
  - SportsEngine's chat rules;
  - Hudl's and GameChanger's policies on minors.
- **Not researched (search budget exhausted):**
  - STEM Racing / F1 in Schools' own safeguarding and communication rules for teams;
  - UK school requirements: online-safety duties in Keeping Children Safe in Education (KCSIE), DfE data-protection guidance, data protection impact assessments (DPIAs);
  - US state student-privacy laws and district data-privacy agreements (e.g., SDPC).
  - Unverified background: UK and US schools commonly ask vendors for a data processing/privacy agreement and a DPIA before approval.
- **COPPA and school authorisation:** one edtech-law blog says the amended rule "tightened" consent authorised by schools — [Promise Legal](https://blog.promise.legal/coppa-april-2026-amendments-edtech/). This is unverified. My background understanding is that the FTC declined to codify the proposed school-authorisation provisions in the final rule. Check the Federal Register text.

## Q2. Daily and weekly loops: what brings coaches, players and parents back, and what admin the apps take off a coach's hands

### Takeaway
The loops that bring people back are small, frequent and addressed to one person:
- "Are you coming?": a one-tap RSVP from a reminder.
- "What changed?": a schedule notification.
- "How did it go?": results, stats and live video for families.
- A weekly digest: Google Classroom guardian summaries, the WHOOP Monday assessment.
- A daily brief: Garmin Morning Report.

The admin removed is repetitive chasing and conversion work: reminders, attendance, payments, translation, film breakdown and parent updates.

### Cited Findings
- **Availability/RSVP loop (TeamSnap):**
  - Members answer Yes/No/Maybe in the app, on the web, or by clicking links in automatic reminder emails.
  - They can add a note explaining absence or lateness.
  - Coaches use past availability as an attendance record, and admins can lock changes.
  - Capterra reviewers most often mention automated reminders and availability tracking, which replaced reminder emails coaches used to write by hand.
  - Sources: [TeamSnap: set availability from automatic reminder emails](https://helpme.teamsnap.com/article/95-set-availability-from-automatic-reminder-emails); [track event availability](https://helpme.teamsnap.com/article/660-track-event-availability); [send availability reminders](https://helpme.teamsnap.com/article/258-send-availability-reminders); [TeamSnap blog: lock changes and track attendance](https://www.teamsnap.com/blog/how-to/availability-tips-how-to-lock-changes-and-track-attendance); [Capterra: TeamSnap](https://www.capterra.com/p/123208/TeamSnap/)
  - *Implication for SubOne:* one-tap "coming / not / maybe + note" for build sessions, test-track days and competition travel, answerable from the notification or email without logging in. Answers feed Plan and Today, e.g., "3 of 5 can make Thursday's paint session".
- **Heja:**
  - Free: team schedule, important messages, automatic reminders, group chat with photo/video, attendee limits.
  - Paid tiers add attendance stats, payment tracking, unlimited admins, desktop access, RSVP updates and "powerful reminders".
  - Sources: [Heja (App Store)](https://apps.apple.com/us/app/heja/id1157335714); [Heja Help: Team Pro features](https://help.heja.io/en/articles/4358964-team-pro-features)
- **Spond:** free scheduling and attendance, plus in-app payment collection and fundraising, which is where Spond makes its money (see Q7) — [Spond: payment costs](https://help.spond.com/app/en/articles/118091-payments-costs-in-the-spond-app); [Spond is free to use](https://help.spond.com/en/articles/25998-spond-is-free-to-download-and-use)
- **Digest for the adult at home (Google Classroom):** guardians choose a daily or weekly email covering missing work, upcoming work (today and tomorrow, or the coming week) and recent class activity — [Classroom Help](https://support.google.com/edu/classroom/answer/6386354?hl=en)
  - *Implication for SubOne:* a weekly teacher/mentor digest, plus an optional guardian digest, in the same three parts:
    - overdue;
    - due next week;
    - what the team did: runs logged, car version saved, sponsor secured.

    Send it by email first, so adults stay informed without opening the app.
- **Monday review (WHOOP):**
  - Every Monday, members get a Weekly Performance Assessment, unlocked after 14 recovery scores.
  - It shows the week's strain-versus-recovery balance in three zones: Restoring, Optimal, Overreaching.
  - Sleep and activity are compared with the member's own 3-week average, plus a comparison with the WHOOP community.
  - Monthly Performance Assessments have been delivered by email since the June 2025 report.
  - Sources: [WHOOP Support: WPA](https://support.whoop.com/hc/en-us/articles/360019454194-What-is-the-Weekly-Performance-Assessment-WPA-); [WHOOP: the Weekly Performance Assessment](https://www.whoop.com/thelocker/new-weekly-performance-assessment/)
  - *Implication for SubOne:* compare the team's week with its own recent weeks (a rolling 3-week average), not with other teams. Hold back insights until there is enough data, and state the minimum, e.g., "needs 5 logged runs".
- **Daily brief (Garmin):** Morning Report is a single summary on waking of the night's and previous day's key metrics, for planning the day — [Garmin Wiki: Morning Report](https://wiki.garminrumors.com/Morning_Report); [the5krunner: Morning Report](https://the5krunner.com/2022/06/28/garmin-morning-report/)
  - *Implication for SubOne:* supports the existing "Today: one next move per person" design. Keep it to one card per person, not a feed.
- **Event-day loop (The Blue Alliance):**
  - "myTBA" favourites for teams, events and matches.
  - Subscriptions per event or per year, with a choice of notification types such as upcoming match and results.
  - Real-time scores, plus webhooks and an open API that teams pipe into their own tools.
  - Sources: [TBA (Google Play)](https://play.google.com/store/apps/details?id=com.thebluealliance.androidclient&hl=en_US); [TBA webhooks](https://www.thebluealliance.com/apidocs/webhooks); [TBA API v3](https://www.thebluealliance.com/apidocs/v3)
  - *Implication for SubOne:* a "competition day" mode across Race, Pitch and Team. It holds the schedule of heats, judging slots and pit-display checks, with push reminders such as "verbal presentation in 30 min — slides checked?".
- **Family loop sold as a product (GameChanger):** families follow stats and watch live streams. After five free baseball/softball streams, watching requires a paid plan — [GC family plans](https://gc.com/pricing-family-plans); [GC live streaming](https://gc.com/app-features/live-streaming)
- **Admin removed (Hudl Assist):**
  - Coaches upload games, and Hudl's analysts tag them around the clock.
  - Stats come back linked to the video, with automatic reports.
  - Hudl says coaches who break down two or more games a week spend about 136 hours (more than five days) a season on it (vendor claim).
  - Sources: [Hudl Assist](https://www.hudl.com/products/assist); [Hudl: coaches on Assist as a time saver](https://www.hudl.com/blog/the-time-saving-tool-you-need-coaches-speak-out-about-hudl-assist); [Hudl: 5 annoying tasks](https://www.hudl.com/blog/5-annoying-tasks-coaches-dont-have-to-put-up-with-anymore); [Assist by the numbers](https://www.hudl.com/resources/assist-by-the-numbers)
  - *Implication for SubOne:* find the most tedious manual job of the season and automate it. Candidates: turning run logs into statistics, collecting portfolio evidence as the season goes, and assembling sponsor reports. The AI race engineer can do the "breakdown" step.
- **Admin removed (ClassDojo):** automatic message translation into 130+ languages (2025–26 district release) and teacher quiet hours — [PR Newswire: ClassDojo for Districts 2025–26](https://www.prnewswire.com/news-releases/classdojo-for-districts-unveils-new-features-for-202526-school-year-302510766.html); [ewa.org copy](https://ewa.org/members-news/press-releases/classdojo-districts-unveil-new-features-school-year-education); [ClassDojo: quiet hours](https://blog.classdojo.com/introducing-quiet-hours-for-teachers/)
- **Social loop (Strava):** 14 billion kudos were given in 2025, 20% more than in 2024 — [Strava press: Year in Sport 2025](https://press.strava.com/articles/strava-releases-12th-annual-year-in-sport-trend-report-2025)

### Inferences
- **Four cadences recur:**
  - daily: Garmin Morning Report;
  - weekly: WHOOP's Monday assessment, Google Classroom's weekly digest;
  - event-driven: The Blue Alliance, GameChanger;
  - seasonal/annual: Strava Year in Sport, Track Titan's yearly recap (Q4).

  SubOne can map these onto Today (daily), a Monday team review/digest (weekly), competition-day mode (event) and a season recap that feeds the Portfolio (seasonal).
- **The big time sinks are chasing people and processing raw material.** In these apps the coach's largest savings come from not chasing people (reminders, RSVPs) and from turning film and stats into something usable. For STEM Racing teachers, the equivalents are chasing students on deadlines across the judged categories, and turning build and test activity into portfolio evidence.

### Gaps
- No figures found on RSVP response rates, notification open rates or retention for TeamSnap, Spond or Heja.
- Unverified: GameChanger's auto-written game recaps and Hudl's automatic highlight reels. Background knowledge says these exist, but I could not confirm details or dates because the search budget ran out.

## Q3. Data to insight: how Strava, TrainingPeaks, WHOOP, Garmin and the sim-racing coaches turn raw data into a few actionable insights (progress, comparison, "one thing to work on", uncertainty, praise and complaints)

### Takeaway
Users praise tools that do one of three things:
1. Reduce the data to one score or traffic light with its inputs visible: WHOOP Recovery, Garmin Training Readiness, TrainingPeaks compliance colours.
2. Name one ranked, specific cause of lost time and how to fix it: Track Titan Coaching Flows/TimeKiller, Coach Dave Delta Auto Insights.
3. Compare by default against a meaningful reference: the session's best lap in RaceChrono, ghosts and reference laps in Garage 61 and VRS.

Users mock generic AI text that restates numbers or guesses wrongly: Strava Athlete Intelligence at launch, Garmin Active Intelligence. The mockery is harsher when the feature is paid. Only the robotics tool Statbotics publishes its accuracy and calibration. Consumer fitness apps rarely explain uncertainty, which produces "my score doesn't match how I feel" complaints.

### Cited Findings

**One score or traffic light, with its inputs shown**
- **WHOOP Recovery:**
  - Scored 1–100%. Green 67–100 means ready for high strain, yellow 34–66, red 1–33.
  - Inputs: sleep, heart-rate variability (measured as RMSSD during deepest sleep), resting heart rate and respiratory rate.
  - Sources: [WHOOP: how Recovery works](https://www.whoop.com/us/en/thelocker/how-does-whoop-recovery-work-101/); [WHOOP developer docs](https://developer.whoop.com/docs/whoop-101/)
  - User posts such as "What if my score doesn't match how I feel?" show the friction when one number contradicts experience — [blog.melissau.com](https://blog.melissau.com/p/whoop-recovery-score)
- **Garmin Training Readiness:**
  - Scored 0–100 in named bands: Prime 95–100, High 75–94, Moderate 50–74, Low 25–49, Poor 1–24.
  - Built from six factors that the user can see: sleep score, HRV status, recovery time, acute load, sleep history and stress history.
  - Sources: [the5krunner](https://the5krunner.com/garmin-features/training/training-readiness/); [Garmin Wiki](https://wiki.garminrumors.com/Training_Readiness); [Should I Train](https://www.shoulditrain.com/blog/garmin-training-readiness-explained)
- **TrainingPeaks compliance colours (planned vs completed):**
  - Green: within ±20% of plan.
  - Yellow: 50–79% or 121–150% of plan.
  - Orange: more than 50% off plan.
  - Red: not completed.
  - Grey: unplanned work.
  - Each colour is based on duration, distance or Training Stress Score (TSS). An indicator shows which of these drove it and whether the athlete went over or under.
  - Sources: [TrainingPeaks: workout card](https://help.trainingpeaks.com/hc/en-us/articles/204861204-Workout-Card-Overview); [BaseCamp: compliance colours](https://www.joinbasecamp.com/support/compliancecolors); [TrainingPeaks athlete guide](https://www.trainingpeaks.com/learn/trainingpeaks-athlete-user-guide/)
  - *Implication for SubOne:* Plan can colour each task or milestone by planned versus actual, with explicit thresholds and a grey "unplanned work" state that credits useful work nobody scheduled. Always show which measure drives the colour.
- **TrainingPeaks Performance Management Chart:**
  - Fitness (CTL): an exponentially weighted average of TSS over the last 42 days.
  - Fatigue (ATL): the same over the last 7 days.
  - Form (TSB): Fitness minus Fatigue. Negative Form means likely tired; positive means rested.
  - Plain names ("Fitness", "Fatigue", "Form") appear next to the acronyms.
  - Coaches warn against treating the Fitness line as a target, e.g., a coach's post titled "Don't chase the blue line".
  - Sources: [TrainingPeaks: what is the PMC](https://www.trainingpeaks.com/learn/articles/what-is-the-performance-management-chart/); [TP Help: Form (TSB)](https://help.trainingpeaks.com/hc/en-us/articles/204071764-Form-TSB); [The Threshold Coach](https://www.thethreshold.coach/single-post/don-t-chase-the-blue-line)
  - *Implication for SubOne:* name statistics plainly ("Consistency", "Typical time", "Best time"), keep the technical term (standard deviation, mean) one tap away, and don't let one chart become the goal.

**"The one thing to work on" (sim-racing coaching)**
- **Track Titan Coaching Flows (Nov 2025):**
  - Instead of making the driver read telemetry corner by corner, it shows "the single biggest area of time loss across your lap", where it happens and what to do differently.
  - It diagnoses the root cause. Example: whether late throttle on exit is really caused by a botched entry. It works across whole corner combinations.
  - "TimeKiller" shows the mistake that costs the most time, counting the later mistakes it causes.
  - December 2025: generation time fell from about 9 s to under 4 s after the "hundreds of simulations" run per corner were sped up.
  - Reviewers describe the insights as clear and easy to follow.
  - Sources: [Track Titan: Nov 2025 update](https://www.tracktitan.io/post/november-2025-update-coaching-flows); [Track Titan: Dec 2025 update](https://www.tracktitan.io/post/december-2025-track-titan-update-faster-coaching-flows-social-leaderboards-bigger-team); [Track Titan](https://www.tracktitan.io/); reviews: [iRacerHUB](https://iracerhub.com/track-titan-iracing-review/), [DeClom](https://declom.com/track-titan/), [Trustpilot](https://www.trustpilot.com/review/www.tracktitan.io)
- **Coach Dave Delta Auto Insights:**
  - Splits every corner into four phases: braking, entry, apex, exit.
  - Tells the driver "you're braking too early into turn 5 … getting on the throttle too late exiting turn 11" rather than "you're 0.8 seconds slower in sector 2".
  - Starts tracking after the out-lap.
  - Recommended loop: a few laps, back to the garage to review, then out again to apply the change.
  - Built into Share & Compare, so a teammate or coach sees the AI's insights next to the telemetry. Included in the Delta subscription.
  - Sources: [Coach Dave: how to use Auto Insights](https://coachdaveacademy.com/documentation/how-to-use-auto-insights-ai-coaching-in-delta/); [Auto Insights announcement](https://coachdaveacademy.com/announcements/sim-racing-ai-coaching-with-delta-auto-insights/); [Share & Compare guide](https://coachdaveacademy.com/tutorials/a-delta-guide-learning-through-share-and-compare-data/)
  - *Implication for SubOne:* the AI race engineer should give one ranked, specific, physical cause, with its evidence and the expected gain. Example: "Your reaction times vary more than your car's track time does; practise starts before re-sanding the wheels."
    - Split a 20 m run into phases the team can actually measure (reaction, launch/track time, any intermediate split), mirroring Delta's four corner phases.
    - Say so when nothing stands out.

**Comparing against a meaningful reference by default**
- **RaceChrono Pro:**
  - Smooth-scrolling analysis with synchronised graph, X/Y graph, map, video and comparison video.
  - Predictive lap timing and a time-delta graph.
  - Deltas are measured against a selected comparison lap, which by default is the session's best lap.
  - Sources: [RaceChrono Pro (App Store)](https://apps.apple.com/us/app/racechrono-pro/id1129429340); [RaceChrono change log](https://racechrono.com/article/2025); [RaceChrono](https://racechrono.com/)
- **Garage 61 (iRacing):**
  - Free core, with an optional Pro plan from about $7/month.
  - Compares laps against ghosts and reference laps from a large pool of drivers in the same car and session type.
  - Braking and throttle traces.
  - Team support with analysis notes, and one-click invites for iRacing teammates.
  - In-sim overlay, plus ghost laps synced automatically into iRacing.
  - Size: one source reports 100,000+ users and 700M+ laps; another says "50+ million laps", presumably an older figure (conflict unresolved).
  - Sources: [Garage 61: about](https://garage61.net/about); [usage docs](https://garage61.net/docs/usage); [ghosts](https://garage61.net/docs/usage/ghosts); [SimLauncher](https://simlauncher.com/apps/garage-61/); [FUSION Racing guide](https://www.fusion-racing.org/iracing/iracing-apps/iracing-apps-garage61.php); comparison written by a competitor: [Coach Dave vs Garage 61](https://coachdaveacademy.com/tutorials/coach-dave-delta-vs-garage-61-which-is-best-for-you/)
- **VRS (Virtual Racing School):**
  - Telemetry is uploaded to the cloud and processed automatically.
  - The Driving Analyzer shows laps with a track map and racing-line overlays, and compares braking, throttle and steering against coach or pro reference laps.
  - Lap tutorials give pro drivers' corner-by-corner explanations.
  - VRS Teams shares telemetry between teammates; 1:1 coaching is available.
  - Data packs are tied to each iRacing season.
  - A free tier keeps 3 months of history; the paid tiers are Dedicated and Competitive.
  - Sources: [VRS FAQ](https://virtualracingschool.com/faq/); [VRS data packs](https://vrs.racing/data-packs); [VRS coaching](https://vrs.racing/coaching); [FUSION Racing: VRS](https://www.fusion-racing.org/iracing/iracing-apps/iracing-apps-vrs.php); [SimLauncher: VRS](https://simlauncher.com/apps/vrs/)
  - *Implication for SubOne:*
    - By default, Race compares the latest run with the best run for the same car version (or session), and Car compares each version with the previous one.
    - Let the team pin a "reference run".
    - Let people attach notes to specific runs and versions, as Garage 61 and VRS teams do.

**Professional tools (for contrast)**
- **MoTeC i2:**
  - Channels can be tiled or overlaid, toggled with a single key.
  - A Time Variance plot shows where time was gained or lost between laps.
  - i2 Pro adds advanced maths (e.g., the `ref:` prefix refers to the reference lap), multiple overlay laps, and unlimited workbooks and worksheets.
  - A sim-racing guide says MoTeC "is built for engineers, not for a friendly first-run wizard". It advises installing i2 Pro from the start, since it is the same free download.
  - Sources: [MoTeC i2 highlights](https://www.motec.com.au/i2/i2highlights/); [SimRacer Central guide](https://simracercentral.com/motec-sim-racing-telemetry-guide/); [MoTeC forum: overlays](https://www.motec.com.au/forum/viewtopic.php?f=26&t=1661)
- **AiM Race Studio 3 + SmartyCam:**
  - Logged channels (RPM, throttle, gear, 3-axis acceleration, temperatures, pressures) are overlaid on video.
  - Paired with a Solo 2 DL lap timer, it adds delta, predictive and split times.
  - Graphic sets can carry a team logo and track map.
  - Tracks are recognised automatically, or can be created by hand.
  - Sources: [AimShop: SmartyCam 3 Sport](https://www.aimshop.com/blogs/newest-releases/aim-smartycam-3-sport-capture-replay-overlay); [AimShop: video analysis in RS3](https://www.aimshop.com/pages/smartycam-hd-setup-configuration-video-analysis-in-race-studio-3); [SmartyCam 3 GP](https://www.aimshop.com/products/smartycam-3-gp)
  - *Implication for SubOne:* offer an optional "engineer view" for older students who want depth: a raw run table, overlaid charts, CSV export, and a MoTeC-style "where did the time go" chart comparing versions. The default screen still shows one insight.

**Explaining uncertainty and accuracy**
- **Statbotics EPA (FRC robotics):**
  - Expected Points Added (EPA) estimates a team's average point contribution to a match. It is measured in points, so it reads like OPR (Offensive Power Rating, a common FRC team-strength rating).
  - Statbotics publishes its accuracy at picking match winners: EPA 70%, OPR 68%, Elo 69%, a wins-only baseline 65%.
  - Another write-up cites about 72% over 2016–2022 backtests. The two figures cover different season ranges.
  - Win probabilities are calibrated: a 70% favourite wins about 70% of the time, so about 3 in 10 such matches are upsets "by design".
  - Sources: [Statbotics: evaluating FRC rating models](https://www.statbotics.io/blog/models); [Statbotics: the EPA model](https://www.statbotics.io/blog/epa); [Statbotics: gentle introduction](https://www.statbotics.io/blog/intro); [Statbotics GitHub](https://github.com/avgupta456/statbotics); [LearnFRC](https://learnfrc.com/blog/what-is-statbotics-frc-epa)
  - *Implication for SubOne:*
    - Express car and driver effects in real units (seconds, thousandths), not abstract scores.
    - State confidence, e.g., "Version 4 is probably faster: about 0.012 s ± 0.009 s over 6 runs each".
    - If SubOne predicts race times, show how often its predictions came true.
- **Zwift Racing Score:**
  - Became Zwift's default race categorisation in October 2024.
  - Score "decay" was switched off at that point, then reintroduced. After 30 days without racing, the displayed score slowly drifts down and the system's uncertainty rises, so returning riders are matched fairly.
  - Further refinements came in November 2025.
  - Sources: [Zwift Insider: Racing Score](https://zwiftinsider.com/racing-score/); [Zwift Insider: ZRS changes](https://zwiftinsider.com/tsoz-closer-look-zrs-changes/); [Zwift Forums, Oct 2024](https://forums.zwift.com/t/zwift-racing-score-update-october-29-2024/637779); [Zwift Forums, Nov 2025](https://forums.zwift.com/t/racing-score-update-nov-12-2025/659342)
  - *Implication for SubOne:* show when an estimate is stale, e.g., "no runs logged for 3 weeks; car changed since". Widen the stated uncertainty as data ages.
- **Data integrity:** Strava announced in May 2024 that it uses AI to weed out leaderboard cheats — [TechCrunch](https://techcrunch.com/2024/05/16/strava-taps-ai-to-weed-out-leaderboard-cheats-unveils-family-plan-dark-mode-and-more)
  - *Implication for SubOne:* flag implausible entries, such as a timing-gate glitch or a typo like 0.12 s, before they enter statistics. Ask the student to confirm rather than silently dropping them.

**AI summaries: praise, complaints, and what users want**
- **Strava Athlete Intelligence:**
  - AI summaries were announced in May 2024, and coverage of the subscriber rollout appeared in October 2024.
  - Forbes headline: the feature "promises insights but provides bland pep talks".
  - It made wrong assumptions, e.g., congratulating a runner on a "run in China" because the activity title mentioned a restaurant called "Great Wall".
  - Redditors called it pointless or a meme; one said it "doesn't add value and probably costs them a ton of money".
  - Strava's CEO called it an early beta aimed at newer users who struggle to understand their data.
  - Sources: [Forbes, Oct 2024](https://www.forbes.com/sites/cyrusfarivar/2024/10/12/strava-upsets-fans-with-new-ai-feature-that-promises-insights-but-provides-bland-pep-talks/); [Fortune](https://fortune.com/2024/10/11/strava-app-artificial-intelligence-fitness-athletic-memes); [TechRadar week-long test](https://techradar.com/health-fitness/i-used-stravas-new-athlete-intelligence-ai-feature-for-a-week-heres-what-happened); [TechCrunch, May 2024](https://techcrunch.com/2024/05/16/strava-taps-ai-to-weed-out-leaderboard-cheats-unveils-family-plan-dark-mode-and-more); [Strava Help: Athlete Intelligence](https://support.strava.com/en-us/articles/15401629-athlete-intelligence-on-strava)
- **Academic study (arXiv, April 2026) of how users react to AI fitness feedback.** It found four tensions:
  - numerical evaluation versus contextual understanding;
  - isolated session summaries versus an ongoing training story;
  - a fixed AI tone versus users' varied emotional states;
  - one AI voice versus different kinds of athlete.

  Users did not treat AI summaries as definitive; they checked them against their own knowledge.
  - Sources: [arXiv 2604.23830](https://arxiv.org/pdf/2604.23830); [Pith summary](https://pith.science/paper/2604.23830)
- **Garmin Connect+ "Active Intelligence":**
  - Connect+ was announced 27 Mar 2025 at $6.99/month or $69.99/year.
  - Its AI insights were mocked on r/Garmin as "basic maths, generic platitudes, and outright incorrect information".
  - TechRadar headline: "11 insights that prove Garmin has no right to charge for its AI subscription feature".
  - Garmin's CEO said on the Q1 2025 and Q4 2025 earnings calls that more features will be reserved for subscribers.
  - An April 2026 review: "still not worth it" for most.
  - Sources: [TechRadar: backlash live blog](https://www.techradar.com/health-fitness/live/live-garmin-connect-backlash-tell-us-what-you-think-about-garmins-new-premium-tier); [TechRadar: 11 insights](https://www.techradar.com/health-fitness/smartwatches/garmins-new-subscription-ai-feature-is-hilariously-bad-so-far); [TechRadar: more paywalled features](https://www.techradar.com/health-fitness/smartwatches/garmin-quietly-confirms-our-worst-fears-about-garmin-connect-says-more-features-will-likely-be-paywalled-in-the-future); [the5krunner, Apr 2026](https://the5krunner.com/2026/04/20/garmin-connect-plus-review/); [Garmin support: Active Intelligence](https://support.garmin.com/en-US/?faq=kWi5DoaMPZ4VCJBA0lFWP7)
- **WHOOP Coach** (announced 26 Sep 2023, built on OpenAI's GPT-4): answers members' questions conversationally, using their own Recovery, Strain, Sleep, Health and Stress data plus WHOOP's algorithms, in 50+ languages — [WHOOP press release](https://www.whoop.com/us/en/press-center/whoop-unveils-the-new-whoop-coach-powered-by-openai/); [BusinessWire](https://businesswire.com/news/home/20230926899032/en/WHOOP-Unveils-the-New-WHOOP-Coach-Powered-by-OpenAI-the-First-Wearable-to-Deliver-Highly-Individualized-Performance-Coaching-on-Demand); [OpenAI case study](https://openai.com/index/whoop/)
  - *Implication for SubOne:* the AI race engineer succeeds by being specific and grounded (Track Titan, Delta) and fails by being generic and chirpy (Strava and Garmin at launch). It should:
    - cite the runs, versions or rule clause behind every statement;
    - connect to the season story (previous weeks, the next competition) rather than summarising one session;
    - use a neutral, adjustable tone;
    - let a student or teacher correct it;
    - never congratulate by default.

**Robotics: data work done by students**
- **The Blue Alliance:**
  - Event schedules, match results, team pages, myTBA notifications and yearly "Insights" pages.
  - Detailed match breakdowns. For 2025: game pieces scored by level (L1–L4), algae counts, per-robot endgame, and a scoring map.
  - Open API, webhooks and community data submission.
  - Sources: [TBA (Google Play)](https://play.google.com/store/apps/details?id=com.thebluealliance.androidclient&hl=en_US); [TBA 2025 Insights](https://www.thebluealliance.com/insights/2025); [TBA API v3](https://www.thebluealliance.com/apidocs/v3); [TBA: add your own data](https://www.thebluealliance.com/add-data)
- **Scouting apps:**
  - ScoutingPASS is a web page pre-loaded on any phone, tablet or laptop, and needs neither Wi-Fi nor mobile data at the event.
  - It has five swipeable pages (Pre-Match, Auto, Teleop, End Game, Post-Match), set by a configuration file.
  - Data is transferred by QR code, read by a webcam or hand scanner into an Excel database.
  - QRScout (FRC team 2713) is designed for tablets, offline use and slow connections.
  - Sources: [ScoutingPASS (GitHub)](https://github.com/PWNAGERobotics/ScoutingPASS); [QRScout (GitHub)](https://github.com/FRC2713/QRScout)
- **Chief Delphi (the FRC community forum):**
  - Student leads write their teams' scouting and strategy guides.
  - Strategy subteams teach game analysis, match strategy and "data fluency", and practise statistics in the off-season.
  - One team documents moving from Google Forms to a custom website with better visualisation (2026).
  - Sources: [FRC 5409 scouting & strategy guide](https://www.chiefdelphi.com/t/5409-s-scouting-strategy-guide-2024-25/504731); [what does your strategy subgroup do?](https://www.chiefdelphi.com/t/what-does-your-strategy-subgroup-do/418233); [FRC 5572 scouting system 2026](https://www.chiefdelphi.com/t/frc-5572-scouting-system-data-and-strategy-overview-2026/519045)
  - *Implication for SubOne:* run logging at the track must work offline on a phone, with a fixed short form (pre-run / run / post-run) that syncs later. Give students a named data role (e.g., "race data lead") with teaching aids, rather than assuming the teacher analyses the data.

### Inferences
- **A common "insight ladder".** The best tools share five steps:
  1. status at a glance, with its inputs;
  2. one ranked problem with a physical fix;
  3. comparison against a meaningful reference;
  4. honest uncertainty;
  5. raw data on demand.

  SubOne's Race and Car sections could follow this order top to bottom.
- **Small differences may be noise.** A STEM Racing run lasts about 1–1.2 s, so differences of a few thousandths between car versions may fall within run-to-run variation. SubOne should not call a version "faster" until the run count supports it, applying the Statbotics lesson. This is my inference; I found no measurement of STEM Racing timing variance.
- **AI output should be shared.** Coaching tools increasingly pair an AI diagnosis with the underlying data and share both with the coach and teammates (Delta's Share & Compare). That fits SubOne's team model: the race engineer's output should be a shared item the team can discuss, not a private chat.

### Gaps
- No quantitative evidence (A/B tests, retention) that "one thing to work on" views improve outcomes. The evidence is vendor claims and reviews.
- Not verified (budget exhausted): the 2025–26 status of Strava Athlete Intelligence, and WHOOP's newer AI and "Advanced Labs" features.
- User numbers not found for Track Titan or Coach Dave Delta.

## Q4. Engagement mechanics: kudos, segments and leaderboards, badges, streaks, challenges, annual recaps, progress reports — what works and what is criticised, especially for teenagers and teams

### Takeaway
- **Well supported:** peer acknowledgement (kudos is associated with more activity), collaboration and narrative (meta-analyses), and annual recaps (Spotify Wrapped and Strava Year in Sport drive enormous engagement and sharing).
- **Harmful for many teens:** public leaderboards (they demotivate low-ranked students), streaks (linked to problematic phone use and fear of missing out) and public behaviour points (ClassDojo is criticised as humiliating).
- **Resented:** putting a beloved recap behind a paywall (Strava, December 2025).
- **Conclusion:** the evidence supports SubOne's "no streaks, points or leaderboards" stance and points to a team-level season recap as the strongest compatible mechanic.

### Cited Findings
- **Strava's scale (Year in Sport 2025 report):**
  - 180M users, 35M more than a year earlier (about 3M a month in 2025).
  - 4B activities and 14B kudos (+20%).
  - Survey of 30,000+ people.
  - Subscribers were active for an hour for every 2 minutes spent in the app.
  - More than half of Gen Z say they plan to use Strava more in 2026.
  - Sources: [Strava press](https://press.strava.com/articles/strava-releases-12th-annual-year-in-sport-trend-report-2025); [PR Newswire](https://www.prnewswire.com/news-releases/strava-releases-12th-annual-year-in-sport-trend-report-revealing-that-doomscrolling-is-out-movement-is-in-302631107.html); [BikeRadar](https://www.bikeradar.com/news/strava-year-in-sport-2025)
  - *Implication for SubOne:* Strava advertises little time in the app, not engagement minutes. SubOne can do the same: measure success by team progress, not time in the app, which suits schools.
- **Kudos research:**
  - A network study of Strava ("Kudos make you run!", *Social Networks*) associates receiving kudos with running more often — [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0378873322000909)
  - A 2026 mixed-methods study of club runners:
    - larger Strava networks went with higher self-efficacy;
    - kudos, comments and visibility felt motivating;
    - Strava also brought pressure, comparison and stress, especially during injury or poor form.
    - Source: [Behavioral Sciences 2026, via PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC12938745/)
  - An earlier qualitative paper describes the "Strava-sphere" in terms of kudos, community and (self-)surveillance — [ResearchGate](https://www.researchgate.net/publication/346678505_Reflections_from_the_'Strava-sphere'_Kudos_community_and_self-surveillance_on_a_social_network_for_athletes)
  - One search summary says users motivated by peer recognition are more prone to obsessive running and burnout. I could not confirm which paper says this.
  - *Implication for SubOne:* a light "nice work" reaction within the team (on a run, a CAD version, a sponsor email) is well supported. Don't show public counts or totals per person.
- **Segments and leaderboards:**
  - Commentators credit Strava segments with giving structure to local, similar-level competition that athletes already improvised, rather than distant global rankings (opinion) — [Behavioral Strategy](https://behavioralstrategy.com/cases/strava/); [Trophy](https://trophy.so/blog/how-strava-uses-segmented-leaderboards-to-drive-engagement)
  - Strava keeps under-18s off segment and challenge leaderboards by default (Q1).
  - Since 2020, Strava's weight, age-group and club leaderboards have been paid; only the top-10 men's and women's lists are free — [the5krunner, 2020](https://the5krunner.com/2020/05/18/strava-turn-off-key-features-welcome-to-the-paywall/)
- **Leaderboard research in education.** Four studies, taken together, report that:
  - for low-ranked students, leaderboards act as negative feedback and social pressure;
  - they lower perceived competence and intrinsic motivation and reduce effort;
  - negative leaderboard feedback can be worse than none;
  - students who dislike competition are stressed by them.

  The four studies are a 2024 systematic review of leaderboards in higher education, a 2025 experiment ("The winner takes it all"), a 2023 study of leaderboard positions, and a 2022 trial in an EFL course. The extract merged their findings, so I did not check which paper says what.
  - Sources: [Li et al. 2024, JCAL](https://onlinelibrary.wiley.com/doi/10.1111/jcal.13077); [ScienceDirect 2025](https://www.sciencedirect.com/science/article/pii/S1041608025002122); [Emerald 2023](https://www.emerald.com/intr/article/33/7/1/178330/How-leaderboard-positions-shape-our-motivation-the); [ScienceDirect 2022, EFL course](https://www.sciencedirect.com/science/article/pii/S0360131522001762); [longitudinal quasi-experiment](https://www.sciencedirect.com/science/article/abs/pii/S1041608024001651)
- **Gamification meta-analyses:**
  - Sailer & Homner (2020, *Educational Psychology Review*): small positive effects on cognitive (g = .49), motivational (g = .36) and behavioural (g = .25) learning outcomes. Game fiction, and competition combined with collaboration, were especially effective for behavioural outcomes — [ERIC](https://eric.ed.gov/?id=EJ1245270); [Semantic Scholar](https://www.semanticscholar.org/paper/The-Gamification-of-Learning:-a-Meta-analysis-Sailer-Homner/be6769b967370c9852210e2fb7a34e499902f814)
  - A 2023 meta-analysis: gamification raises intrinsic motivation and perceived autonomy and relatedness, but has "minimal impact on competency" — [Educational Technology Research and Development, 2023](https://link.springer.com/article/10.1007/s11423-023-10337-7)
- **Streaks:**
  - Research on Snapchat streaks links them with problematic smartphone use and fear of missing out among early adolescents — [ScienceDirect 2023](https://www.sciencedirect.com/science/article/pii/S2772503023000476)
  - Commentary describes Duolingo's streak as a loss-aversion mechanism (opinion) — [JustAnotherPM](https://www.justanotherpm.com/blog/the-psychology-behind-duolingos-streak-feature); [Medium / Bootcamp](https://medium.com/design-bootcamp/how-duolingo-got-me-hooked-the-power-of-loss-aversion-33c4399b95c4)
  - A parental-app vendor claims about 70% of middle schoolers on Snapchat feel "obligated" to keep streaks alive (vendor source, unverified) — [Screenwise](https://screenwiseapp.com/guides/snapchat-streaks-and-social-pressure)
- **Behaviour points (ClassDojo):**
  - Brigitte Vittrup, a child-development professor at Texas Woman's University, told Coda Story that public point displays "can be humiliating for children" and don't change behaviour in the long run — [Coda Story](https://www.codastory.com/authoritarian-tech/classdojo-schools-bias/)
  - The Conversation (2019): digitally tracking behaviour "encourages compliance, not learning" — [The Conversation](https://theconversation.com/digitally-tracking-student-behaviour-in-the-classroom-encourages-compliance-not-learning-110181)
  - A 2025 paper in *Learning, Media and Technology* critiques ClassDojo as a behaviour-management and home–school communication tool — [Taylor & Francis](https://www.tandfonline.com/doi/full/10.1080/17439884.2025.2553184)
  - Critics also object to how long behaviour records are kept, and a researcher argues ClassDojo harms teachers' behaviour-management approach — [EducationHQ](https://educationhq.com/news/classdojo-harms-teachers-behaviour-management-approach-researcher-188825/)
- **Annual recaps:**
  - **Spotify Wrapped 2025:**
    - 200M engaged users within 24 hours, 19% more than the year before; 2024 took 62 hours to reach that mark.
    - 250M engaged users within 65 hours.
    - More than 500M shares in the first 24 hours, up 41%.
    - Coverage framed it as a recovery after 2024's "AI flop".
    - Sources: [Music Business Worldwide](https://www.musicbusinessworldwide.com/spotify-wrapped-campaign-hit-200m-engaged-users-in-24-hours-a-19-yoy-increase/); [Variety](https://variety.com/2025/music/news/spotify-wrapped-breaks-own-record-250-million-engagements-1236603493/); [IBTimes](https://www.ibtimes.co.uk/record-breaking-spotify-wrapped-2025-sees-200m-engage-500m-shares-day-1760640); [TechBuzz](https://www.techbuzz.ai/articles/spotify-wrapped-2025-hits-200m-users-in-24-hours-after-last-year-s-ai-flop)
  - **Strava** moved its personal Year in Sport recap, free since 2016, behind the subscription ($79.99/year) in December 2025, drawing complaints. One outlet says it was following Garmin — [Slashdot](https://news.slashdot.org/story/25/12/19/2158235/strava-puts-popular-year-in-sport-recap-behind-an-80-paywall); [Gadgets & Wearables](https://gadgetsandwearables.com/2025/12/20/strava-year-in-sport/); [T3](https://www.t3.com/tech/dear-strava-we-have-a-paywall-problem-thats-gone-a-step-too-far)
  - **Track Titan**, a coaching tool, added a yearly recap and "social leaderboards" in December 2025. The leaderboards rank achievements completed, not lap times — [Track Titan, Dec 2025](https://www.tracktitan.io/post/december-2025-track-titan-update-faster-coaching-flows-social-leaderboards-bigger-team)
  - *Implication for SubOne:* an end-of-season "Season Recap" is the strongest mechanic compatible with "no streaks, points or leaderboards". It would show:
    - runs logged, the fastest time and how much it improved;
    - car versions, sponsors won, events attended, photos.

    It should be team-level, private by default and shareable only after teacher approval, and it doubles as material for the portfolio and sponsor reports. Keep it free for every team; Strava's paywall backlash is the warning.
- **Zwift:**
  - The Companion app lets riders send "Ride Ons" to encourage each other — [Zwift: cost and what's included](https://www.zwift.com/news/33635-how-much-does-zwift-cost-and-whats-included-everything-you-need-to-know)
  - Racing Score matches riders of similar ability for races and accounts for uncertainty (Q3).

### Inferences
- **The evidence supports SubOne's stance.**
  - Leaderboards demotivate low-ranked teens.
  - Streaks create loss-aversion anxiety.
  - Public behaviour points humiliate.
  - The mechanics that do help (collaboration, narrative, peer acknowledgement, recaps of real progress) fit a team workspace naturally.
- **If comparison is ever wanted, three forms are defensible:**
  - against the team's own past (team personal bests);
  - ability-matched and uncertainty-aware (like Zwift's Racing Score);
  - cooperative team milestones.

  Individual rankings inside a team should never be shown.

### Gaps
- No study found on leaderboards or streaks in team-based school STEM competitions specifically.
- No Nielsen Norman Group (NN/g) article on gamification or streaks was retrieved (budget exhausted).

## Q5. Video and visual analysis: how Hudl and the sim-racing tools overlay or annotate data, and lessons for showing a car's versions and runs

### Takeaway
The common mechanism is linking every number to the moment that produced it:
- Hudl links every stat to video and lets coaches draw on it.
- Delta, RaceChrono and AiM sync telemetry with video frame by frame, including side-by-side comparisons.
- Garage 61 turns the comparison into a ghost to race against.
- MoTeC overlays laps and plots where the time went.

For SubOne, the key data-model decision is linking each run, car version, clip and note together.

### Cited Findings
- **Hudl:**
  - Assist links every data point to video, filterable across games and seasons — [Hudl Assist](https://www.hudl.com/products/assist)
  - Coaches can add text and drawings to the full game video for whole-team feedback — [Hudl blog](https://www.hudl.com/blog/text-and-drawings-on-the-full-video-are-here)
  - Hudl Studio telestration (lines, circles, arrows, dynamic graphics) is replicated automatically across camera angles — [Hudl Studio](https://www.hudl.com/products/studio); [Hudl blog: Studio](https://www.hudl.com/blog/everything-you-need-to-know-about-the-key-features-of-our-new-product-studio)
  - Players review their own clips with coach comments and drawings.
  - Playlists gather clips for a team presentation or one player's improvement, and can be shared to any device.
  - Sources: [Hudl coaching software](https://www.hudl.com/products/hudl); [Hudl: the power of video analysis](https://www.hudl.com/blog/the-power-of-video-analysis-in-sport)
- **Coach Dave Delta video analysis** (introduced in 5.5, in 6.0):
  - Onboard video with brake, throttle, steering, speed and gear traces synced underneath, frame by frame, input by input.
  - Scrub, pause and loop.
  - Side-by-side comparisons with your own laps, peers' laps, a pro lap, or anyone on Delta's global leaderboards, with audio.
  - Sources: [Delta 6.0](https://coachdaveacademy.com/delta/); [video analysis lands in Delta 5.5](https://coachdaveacademy.com/announcements/video-analysis-lands-in-delta-5-5/); [video analysis levels up](https://coachdaveacademy.com/announcements/video-analysis-levels-up/); [how to use video analysis](https://coachdaveacademy.com/documentation/how-to-use-video-analysis-in-delta/)
- **RaceChrono Pro:**
  - Synchronised video and comparison video alongside graphs and map.
  - Hardware-accelerated export with a configurable data overlay, and an overlay editor.
  - Multi-camera picture-in-picture export.
  - Sources: [RaceChrono Pro](https://apps.apple.com/us/app/racechrono-pro/id1129429340); [RaceChrono change log](https://racechrono.com/article/2025)
- **Harry's LapTimer:**
  - Select a lap and press Overlay to add telemetry to the video for YouTube.
  - Real-time overlay on playback.
  - A timer view shows lap and predicted lap times while video records in the background.
  - Video recording and overlay come in the higher (Petrolhead) edition.
  - Sources: [Harry's products](https://www.gps-laptimer.de/products); [Harry's documentation](https://www.gps-laptimer.de/documentation); [OBDLink: Harry's](https://obdlink.nl/en/obd-apps/harrys-lap-timer)
- **AiM SmartyCam / Race Studio 3:** data overlays on camera footage, customisable with a team logo and track map (Q3) — [AimShop](https://www.aimshop.com/blogs/newest-releases/aim-smartycam-3-sport-capture-replay-overlay)
- **Garage 61:** comparisons appear as an in-sim overlay while driving and as ghost laps to race in practice — [Garage 61: ghosts](https://garage61.net/docs/usage/ghosts)
- **MoTeC i2:** channels tiled or overlaid, plus the Time Variance plot (Q3) — [MoTeC i2](https://www.motec.com.au/i2/i2highlights/)
- *Implications for SubOne:*
  - **Race:** attach a phone slow-motion clip to each run log entry. Sync two clips at the start signal to compare two runs or two car versions side by side, or as a "ghost" (the Delta / Garage 61 pattern). Allow drawing on a frame, e.g., to mark wheel lift or wobble on the tether line (the Hudl pattern).
  - **Car:** show versions as a timeline. Each version carries its 3D model, key aero numbers, and the spread of its run times overlaid on the previous version's (the MoTeC overlay pattern), plus a "what changed → what it did" note.
  - **Marketing / Pitch:** export a branded clip with a time overlay and sponsor logo (the AiM / RaceChrono pattern), with teacher approval where students are visible.
  - **Portfolio / Pitch:** Hudl-style playlists of annotated clips and charts, reusable as evidence for the portfolio and the verbal presentation.

### Inferences
- **Numbers and footage belong together.** Numbers without their clip, or clips without their numbers, lose most of their teaching value. SubOne already models versions and runs, so the linking layer (run → version → clip → note) is where most of the visual-analysis value lies.
- **Short runs make this easy.** A run takes about a second, so a synced pair of slow-motion clips is cheap to produce and easy to read. The sim-racing "ghost" idea may transfer to STEM Racing more easily than long-lap telemetry does.

### Gaps
- Not verified this session: Hudl's automatic highlights, and any AI clipping features in Hudl or GameChanger.
- No sources found on the video tools STEM Racing / F1 in Schools teams actually use to film 20 m runs.

## Q6. What coaches and teachers value most (time saved, fewer messages, clear records), and what makes them abandon a tool

### Takeaway
**What they value:**
- time saved on repetitive admin: reminders, attendance, film breakdown;
- fewer and calmer messages: quiet hours, translation, one channel;
- clear records: history that can be downloaded and not edited.

**Why they leave:**
- too many tools;
- forced migrations that remove features they rely on;
- paywalls on features that used to be free;
- broken promises;
- complexity.

Fitness apps also show seasonal churn: users say "I'll see you in the winter".

### Cited Findings
- **Time saved:**
  - Reviewers praise TeamSnap's automated reminders and availability tracking, which replaced manual emails — [Capterra](https://www.capterra.com/p/123208/TeamSnap/)
  - Hudl says Assist saves coaches an average of 136 hours of breakdown per season (vendor claim) — [Hudl](https://www.hudl.com/blog/the-time-saving-tool-you-need-coaches-speak-out-about-hudl-assist)
- **Records and boundaries:**
  - Remind: messages cannot be edited or deleted, and history can be downloaded — [Remind](https://help.remind.com/hc/en-us/articles/203744719-Trust-and-safety-on-Remind)
  - ClassDojo: teachers set quiet hours, and leaders can request message history — [ClassDojo](https://help.classdojo.com/hc/en-us/articles/42702434157069-Teacher-to-Student-Messaging-FAQ-For-Teachers-and-School-Leaders)
- **Too many edtech tools.** The figures below are reported across the four articles cited. Pages could not be opened, so which article gives which figure is not verified.
  - Nearly two-thirds of teachers, principals and district leaders surveyed said the number of tools exhausted them (EdWeek, 2022).
  - The average district used 841 edtech tools in 2018 and 2,739 in 2023–24.
  - 65% of district administrators have dropped a tool they had adopted.
  - A 2025 survey found 54% of K-12 schools use 10–15 different apps.
  - About a third of educators say there are too many tools to use efficiently.
  - Educators want more time to learn tools (32%), better funding (28%) and more training (22%).
  - Sources: [eSchool News, Apr 2025](https://www.eschoolnews.com/digital-learning/2025/04/28/too-many-apps-for-that-in-schools/); [District Administration](https://districtadministration.com/briefing/are-there-too-many-edtech-tools-for-teachers-to-master/); [Edutopia](https://www.edutopia.org/article/technology-integration/); [EdSurge, Apr 2026](https://www.edsurge.com/news/2026-04-02-too-many-tools-not-enough-impact-districts-rethink-their-edtech-stacks)
  - 2026 headlines describe an "ed-tech backlash" — [EdWeek, Apr 2026](https://www.edweek.org/technology/the-ed-tech-backlash-is-here-what-it-means-for-schools/2026/04); [Jacobin, May 2026](https://jacobin.com/2026/05/educational-technology-children-learning-iready)
  - Schools are also tackling parent "app fatigue" — [The Learning Standard](https://thelearningstandard.org/news/how-schools-are-tackling-parent-app-fatigue-and-tech-overload)
  - *Implication for SubOne:* position SubOne as replacing several tools (WhatsApp/Discord group, spreadsheets, shared drive, email threads), not adding one. Keep the teacher's weekly time cost visibly small, e.g., a 5-minute Monday digest.
- **Forced migration that removed features (TeamSnap ONE, 2024–25).** App-store and review-site users report that:
  - the new app dropped positions, email, photos/files, phone numbers and proper chat;
  - coaches can't create schedules on desktop, and admins must use desktop for everything;
  - the calendar syncs only at midnight.

  They call it "TeamSnap Zero" and "a major step backwards" that favours organisation admins over coaches' daily needs.
  - Sources: [App Store reviews](https://apps.apple.com/us/app/teamsnap-one/id6670517733?see-all=reviews&platform=iphone); [Google Play](https://play.google.com/store/apps/details?id=com.teamsnap.android.fusion&hl=en_US); [Capterra reviews](https://www.capterra.com/p/123208/TeamSnap/reviews/); [Trustpilot](https://www.trustpilot.com/review/teamsnap.com)
  - *Implication for SubOne:* never remove a feature coaches or students rely on during a season. Ship big changes between seasons with an opt-in period. Keep laptop and phone equally capable for teacher tasks.
- **Paywalling what used to be free:**
  - Garmin Connect+ (March 2025) drew immediate backlash — [TechRadar](https://www.techradar.com/health-fitness/live/live-garmin-connect-backlash-tell-us-what-you-think-about-garmins-new-premium-tier)
  - Strava moved leaderboards beyond the top 10 behind its subscription in 2020 — [the5krunner](https://the5krunner.com/2020/05/18/strava-turn-off-key-features-welcome-to-the-paywall/) — and Year in Sport in December 2025 — [T3](https://www.t3.com/tech/dear-strava-we-have-a-paywall-problem-thats-gone-a-step-too-far)
  - Remind tightened its free limits and is reportedly being folded into ParentSquare, with migrations through 2026. These claims come from competitors' blogs (lower reliability) — [Cronote](https://www.cronote.com/blog/remind-app-alternative-2026.html); [FRANSiS](https://www.fransis.ai/articles/remind-alternatives-for-schools)
  - *Implication for SubOne:* publish a "free forever for the team" list and never move anything off it. Pro should add capability for teachers, not take features away from students.
- **Broken promises (WHOOP 5.0 / MG, launched 8 May 2025):**
  - Existing members were asked for $49 or $79 upgrade fees, or a 12-month extension, despite earlier statements that upgrades were free.
  - Reddit reacted with threads such as "Whoopgate: The Receipts", and Bloomberg noted WHOOP was "trending for all the wrong reasons".
  - WHOOP reversed on 10 May: free upgrades for members with 12+ months remaining, and refunds.
  - Sources: [Athletech News](https://athletechnews.com/whoop-clarifies-updates-policy-after-member-pushback/); [TechRadar](https://www.techradar.com/health-fitness/fitness-trackers/whoop-has-broken-a-promise-on-free-hardware-upgrades-and-users-arent-pleased); [The Shortcut](https://www.theshortcut.com/p/whoop-5-upgrade-isnt-free-to-users); [Plunge](https://plunge.com/blogs/blog/whoop-launches-5-0-and-mg-devices)
- **Price rises and seasonal churn (Zwift):**
  - From 6 June 2024, the monthly price rose from $14.99 to $19.99 (UK £12.99 to £17.99) and the annual price from $149.99 to $199.99.
  - Users replied "I'll see you in the winter", meaning they would subscribe only for the indoor season.
  - Sources: [DC Rainmaker](https://www.dcrainmaker.com/2024/05/increases-prices-hardware.html); [road.cc](https://road.cc/content/news/zwift-accused-taking-users-granted-price-hike-308245); [Cyclingnews](https://www.cyclingnews.com/news/zwift-hikes-subscription-price-by-over-a-third/); [Zwift support FAQ](https://support.zwift.com/en_us/subscription-price-increase-faq-H1w618m1R)
  - *Implication for SubOne:* STEM Racing is seasonal. Price Pro per season or academic year, to match school budgets, rather than monthly, and let a team pause off-season without losing data.
- **Complexity:** MoTeC i2 on first open "looks like a cockpit you have no manual for" — [SimRacer Central](https://simracercentral.com/motec-sim-racing-telemetry-guide/)
- **Trust in the adult matters to parents** (Aspen Institute, see Q1) — [Aspen Institute](https://www.aspeninstitute.org/wp-content/uploads/2025/06/National-Youth-Sports-Parent-Survey-FINAL.pdf)

### Inferences
- **Teacher adoption has two gates and two exits.**
  - Gates: the school approving privacy and safeguarding, and a visible net time saving.
  - Exits: disruption mid-season, and a sense of betrayal over price or features.
- **SubOne's pricing model carries a specific risk.** "Free for the whole team; Pro paid by a teacher or mentor" is especially exposed to the second exit if anything ever moves from free to Pro.
- **Seasonality cuts both ways:** engagement peaks around competitions, and paid plans churn off-season.

### Gaps
- No primary survey found of teachers who run extracurricular STEM or competition teams. The evidence covers K-12 edtech generally and youth-sport coaching.
- No survey data found on youth coaches' burnout from communication load. The Aspen 2024 figures cover parents' views, not coaches' time.

## Q7. Per-app snapshot: what each does best, role design, and business model (who pays)

### Takeaway
- **Youth and school apps** are mostly free for students and families. They make money from the organiser (TeamSnap, Hudl, Heja's paid tiers), from families buying extras (ClassDojo Plus, GameChanger) or from payment fees (Spond).
- **Performance apps** charge the athlete, or the coach, who can also cover athletes (TrainingPeaks). TrainingPeaks is the closest precedent for SubOne's teacher-paid Pro.
- **Sim-racing coaches** offer a free core, with paid AI insights and pro comparisons.
- **Robotics data tools** are free and open source.

(A separate researcher covers monetisation in depth. This section records only who pays.)

### Cited Findings

| App | What it does best | Roles / data design | Business model and who pays | Sources |
|---|---|---|---|---|
| TeamSnap | Availability + automated reminders; attendance history | Household organiser; family contacts get the member's access | Coach pays per team: Premium from $9.99/mo, Ultra $17.99/mo (listing prices; annual figures differ by source); clubs and leagues get custom quotes. Claims 25M users in 196 countries (vendor claim) | [TeamSnap pricing](https://www.teamsnap.com/pricing); [GetApp](https://www.getapp.com/industries-software/a/teamsnap/pricing/); [Capterra](https://www.capterra.com/p/123208/TeamSnap/) |
| Spond | Youth groups built around guardians; free scheduling, attendance, payments | Children-only or mixed groups; guardian responds for children | Free core. Revenue from payment-processing fees (via Stripe), club websites and a share of fundraising. Claims "2 million-plus users" and ">1.5 million people across the UK every month": the two vendor figures don't reconcile | [Spond: payment costs](https://help.spond.com/app/en/articles/118091-payments-costs-in-the-spond-app); [Spond: free team app](https://www.spond.com/news-and-blog/best-team-app-thats-free-to-use/); [Spond: payment collection](https://www.spond.com/news-and-blog/best-sports-club-payment-collection-app/) |
| Heja | Simple team chat + schedule + reminders | Player vs Parent roles; guardian or admin approves links | Free for the whole team. Heja Plus / Team Pro / Team Pro Max are paid by coach or admin (prices not found). "Ad-free" is a paid feature, which implies the free tier shows ads | [Heja (App Store)](https://apps.apple.com/us/app/heja/id1157335714); [Heja tiers](https://help.heja.io/en/articles/8061610-what-is-the-difference-between-heja-plus-team-pro-team-pro-max) |
| SportsEngine | Club and league admin + team chat | Guardians in team chat; admins moderate media | Not verified this session | [SportsEngine: team chat](https://www.sportsengine.com/blog/sportsengine-hq-product-update-team-chat/) |
| BAND | General-purpose group communication | Ages 13–17 private by default; parent Supervisor mode; BAND for Kids for 12 and under | Not verified | [Bark](https://www.bark.us/app-reviews/apps/band-app-review/) |
| Hudl | Video linked to data; Assist breakdown; telestration | Coach → athlete clips, comments, playlists | The school's athletic department pays: $1,500 / $2,500 / $4,000 per sport per year. Department-wide packages are quote-only. Focus camera about $3,000. Booster clubs sometimes fund it | [Hudl HS pricing](https://www.hudl.com/pricing/high-school); [HoopBrief](https://hoopbrief.com/blog/how-much-does-hudl-cost-2026); [PLSouthside Scroll](https://plsouthsidescroll.com/686/sports/hudl-keeps-costly-eye-on-athletes/); [Nebraska News Service](https://www.nebraskanewsservice.net/unlimitedsports/hudl-s-new-smart-camera-is-revolutionizing-sports-analytics/article_b7cfa349-7335-56a6-806c-4d9dcd915193.html) |
| GameChanger | Live scoring, stats and streaming for families | Staff / player / family / fan roles; three-level stats privacy | Families and fans pay: Plus $39.99/yr ($9.99/mo); Premium $99.99/yr; Family plan $179.99/yr for 4 people, or $24.99/mo. Team Pass also offered; first 5 live streams free | [GC family plans](https://gc.com/pricing-family-plans); [GC subscription FAQ](https://help.gc.com/hc/en-us/articles/28521445314957-Individual-Subscription-FAQs); [Team Pass](https://gc.com/pricing/team-pass) |
| Google Classroom | Assignments + guardian email summaries; teacher-grounded Gemini for teens | Teacher / student / guardian (guardians get email only) | Not verified this session | [Classroom Help](https://support.google.com/edu/classroom/answer/6386354?hl=en) |
| ClassDojo | Home–school messaging with translation and quiet hours; points (criticised) | Teacher / parent / student; district and school leaders control switches | Free for teachers and schools, which are "never prompted to pay". Parents can buy ClassDojo Plus, reportedly $15.49/mo or $109.99/yr from January 2024; more than 1M families have upgraded (vendor claim) | [ClassDojo: how it's free](https://help.classdojo.com/hc/en-us/articles/205924206-How-is-ClassDojo-free-for-all-schools); [Plus FAQ](https://help.classdojo.com/hc/en-us/articles/360018137732-ClassDojo-Plus-FAQ); [ClassDojo Plus](https://www.classdojo.com/plus/); [Wikipedia](https://en.wikipedia.org/wiki/ClassDojo) |
| Seesaw | Student journals with teacher approval; family view | Teacher approves posts and family connections | Not verified | [Seesaw Help](https://help.seesaw.me/hc/en-us/articles/203008899-Privacy-for-student-journals) |
| Remind | Safe school texting; history that can't be edited | Under-13s receive only, with parent copied | Freemium, with districts on paid plans. Reportedly being folded into ParentSquare (competitors' blogs) | [Cronote](https://www.cronote.com/blog/remind-app-alternative-2026.html); [FRANSiS](https://www.fransis.ai/articles/remind-alternatives-for-schools) |
| Strava | Social feed, kudos, segments; Year in Sport | High-privacy defaults for under-18s | Freemium: $79.99/yr or $11.99/mo. Family plan (2024). Year in Sport paywalled December 2025. 180M users | [Strava press](https://press.strava.com/articles/strava-releases-12th-annual-year-in-sport-trend-report-2025); [Slashdot](https://news.slashdot.org/story/25/12/19/2158235/strava-puts-popular-year-in-sport-recap-behind-an-80-paywall); [TechCrunch](https://techcrunch.com/2024/05/16/strava-taps-ai-to-weed-out-leaderboard-cheats-unveils-family-plan-dark-mode-and-more); [Wikipedia](https://en.wikipedia.org/wiki/Strava) |
| TrainingPeaks | Planned-vs-done compliance colours; Performance Management Chart | Coach plans, athlete executes | Coach pays the platform: Coach Edition $21.99/mo (includes 1 coach-paid Premium athlete + 4 Basic); Unlimited $54.99/mo; $99 activation fee. Coach-paid Premium athletes cost $9 each, falling to $4.50 each above 1,000. Alternatively athletes pay for Premium themselves (about $19.95/mo, or about $12/mo billed annually) | [TP coach pricing](https://www.trainingpeaks.com/pricing/for-coaches/); [TP Help: coach billing](https://help.trainingpeaks.com/hc/en-us/articles/204072544-TrainingPeaks-Coach-Account-Pricing-and-Billing); [TP blog: coach pricing](https://www.trainingpeaks.com/blog/trainingpeaks-coach-edition-pricing/); [TP Help: Basic vs Premium athletes](https://help.trainingpeaks.com/hc/en-us/articles/204072624-Basic-Athlete-vs-Premium-Athlete-account-for-Coaches) |
| Garmin Connect | Morning Report; Training Readiness with its factors shown | Individual | Free with the watch. Connect+ $6.99/mo or $69.99/yr (March 2025) | [TechRadar](https://www.techradar.com/health-fitness/live/live-garmin-connect-backlash-tell-us-what-you-think-about-garmins-new-premium-tier) |
| WHOOP | Recovery traffic light; Monday assessment; WHOOP Coach | Individual | Subscription membership that includes the hardware; upgrade-fee row in May 2025 | [Athletech News](https://athletechnews.com/whoop-clarifies-updates-policy-after-member-pushback/) |
| Zwift | Social virtual riding; Ride Ons; Racing Score categories | Individual + events | $19.99/mo or $199.99/yr since June 2024 | [DC Rainmaker](https://www.dcrainmaker.com/2024/05/increases-prices-hardware.html) |
| Track Titan | "Single biggest time loss" Coaching Flows; TimeKiller | Individual; social leaderboards of achievements | Free community membership "forever"; paid plans needed for AI insights and pro comparisons; 7-day trial. Sells setups for many sims. Announced a $5M funding round | [Track Titan pricing](https://app.tracktitan.io/pricing); [Track Titan funding post](https://www.tracktitan.io/post/funding-round-track-titan-update-5-million-reasons-to-get-even-more-excited-about-track-titan) |
| Garage 61 | Free iRacing telemetry; team sharing; ghosts | Teams, notes, one-click invites | Free core; Pro from about $7/mo | [Garage 61](https://garage61.net/about); [SimLauncher](https://simlauncher.com/apps/garage-61/) |
| Coach Dave Delta | Setups + telemetry + Auto Insights (4 phases per corner) + synced video | Share & Compare with teammates or coach | Subscription, with Auto Insights included | [Delta](https://coachdaveacademy.com/delta/); [Auto Insights](https://coachdaveacademy.com/documentation/how-to-use-auto-insights-ai-coaching-in-delta/) |
| VRS | Reference laps + pro corner-by-corner tutorials + teams | Teams; 1:1 coaching | Free tier (3-month history); paid Dedicated and Competitive tiers; data packs for each season | [VRS FAQ](https://virtualracingschool.com/faq/); [SimLauncher: VRS](https://simlauncher.com/apps/vrs/) |
| RaceChrono | Phone lap timer; synced video, graph and map; delta against the session's best lap | Individual | Free app plus a separate paid Pro app (price not found) | [RaceChrono](https://racechrono.com/); [RaceChrono (Google Play)](https://play.google.com/store/apps/details?id=com.racechrono.app&hl=en) |
| Harry's LapTimer | Predictive timing; video overlay | Individual | Paid editions (Rookie, Petrolhead, and higher) | [Harry's products](https://www.gps-laptimer.de/products) |
| MoTeC i2 | Engineering-grade analysis; maths channels; Time Variance plot | Engineers | Free download (a guide says i2 Pro is the same free download for sim use) | [SimRacer Central](https://simracercentral.com/motec-sim-racing-telemetry-guide/) |
| AiM Race Studio 3 | Logger + video overlay | Engineers and drivers | Tied to AiM hardware (software pricing unverified) | [AimShop](https://www.aimshop.com/pages/smartycam-hd-setup-configuration-video-analysis-in-race-studio-3) |
| The Blue Alliance | Results, schedules, notifications, insights, open API | Public | Free; open API; community-submitted data | [TBA API v3](https://www.thebluealliance.com/apidocs/v3); [TBA: add data](https://www.thebluealliance.com/add-data) |
| Statbotics | EPA ratings and calibrated match predictions | Public | Free and open source | [Statbotics GitHub](https://github.com/avgupta456/statbotics) |
| FRC scouting apps (ScoutingPASS, QRScout) | Offline, QR-code-based scouting by students | Student scouts → strategy lead | Free and open source, built by teams | [ScoutingPASS](https://github.com/PWNAGERobotics/ScoutingPASS); [QRScout](https://github.com/FRC2713/QRScout) |

- *Implication for SubOne (who pays):*
  - **TrainingPeaks is the clearest precedent for "the adult pays and covers the team".** The coach pays a platform fee and can buy Premium for each athlete, with volume discounts, while athletes keep a free Basic tier.
  - **ClassDojo is the opposite model:** parents pay and teachers are never asked. SubOne has rejected this for minors.
  - **GameChanger shows families will pay to follow their child,** but that clashes with SubOne's teacher-paid stance and its private-by-default design.

### Inferences
- **Paid AI must earn its price.** Sim-racing tools put AI insights behind subscriptions, and the Garmin and Strava backlash shows people resent paying for generic AI. If SubOne's race engineer sits in Pro, Pro must be visibly better than the free insight. The free tier should still show the basic "one thing to work on", so free teams are not left with raw numbers.

### Gaps
- Business models not verified this session: SportsEngine, BAND, Google Classroom, Seesaw, AiM.
- Exact prices not found: Heja, RaceChrono Pro, Harry's LapTimer, Track Titan, Coach Dave Delta, VRS.
- Not verified: whether Garmin put a year-in-review recap behind Connect+, which one outlet implies.
