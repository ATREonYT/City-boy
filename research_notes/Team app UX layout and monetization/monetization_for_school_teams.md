# Monetization for team software used by minors and paid for by teachers, schools or sponsors (SubOne)

> **Evidence notes (read first).** Research date: 25 September 2026.
> - **Access limits.** The network proxy blocked WebFetch for almost every domain tried: chartmogul.com, growthunhinged.com, lennysnewsletter.com, substack.com, ico.org.uk, gov.uk, federalregister.gov, asa.org.uk, paddle.com, canva.com, hudl.com, teamsnap.com, heja.io, gc.com, onshape.com, seesaw.com, stemracing.com, docs.stripe.com, docs.github.com, support.google.com and wikipedia.org. Only Apple's App Review Guidelines were read in full.
> - **Search extracts.** Every other finding comes from search-engine extracts of the named pages. Extracts can compress or misstate a page, so a figure that rests on one extract should be checked on the live page before it is published.
> - **Search budget.** The session's web-search budget ran out part-way through, so some planned checks are listed under Gaps.
> - **Reused context.** Some STEM Racing context is reused from the sibling notes in `research_notes/STEM Racing car design marketing progress/`, cited to their original sources.
> - **Tags.** **[DATA]** is a measured survey or benchmark. **[PRICE]** is a list price. **[RULE]** is law, regulator or official guidance. **[OPINION]** is practitioner advice, or a claim with no disclosed method. **(P)** marks a publisher or primary source; **(S)** marks a secondary source (aggregator, blog, law-firm note).
> - **Currency.** GBP equivalents are indicative only. They use an assumed £1 = US$1.33 = €1.15, a round-number assumption rather than a sourced September 2026 rate.
> - **SubOne arithmetic used throughout.**
>   - Pro at £69 per school year ÷ £9 per month = 7.7 months to break even.
>   - £69 is 36% below 12 × £9 (£108).
>   - For 3–6 students, £69 is £11.50–£23.00 per student per season.

## 1. Free-to-paid benchmarks: freemium vs free trial vs reverse trial, and which fits a seasonal school-team product

### Takeaway
The best B2B self-serve benchmarks (2023–2026) put conversion at these levels:
- **Freemium:** about 3–5% ("good") and 8–12% ("great") of sign-ups.
- **Reverse trials:** 4–6% good and 8–12% great.
- **No-card trials:** about 8–12% good.
- **Card-required trials:** about 30%.

Card-required trials only look strong because the card pre-qualifies buyers. SubOne cannot use them, because its buyers are teachers, schools and sponsors, often paying by invoice, and students must never pay.

For a seasonal product with small teams, the best fit is team-level freemium plus Pro "tastes" timed to the adult buyer's moments of need, and possibly a short no-card reverse trial at the start of the season. Pure freemium should be expected to convert only a low single-digit share of teams, so school, trust and sponsor deals are needed on top.

### Cited Findings
- **ChartMogul, *SaaS Conversion Report* (2026):** median free-to-paid conversion across all products is 8%, "though very few products actually have an 8% conversion rate". One in five products (20%) are below 2.5%, and about 30% sit between 2.5% and 7.5%.
  - Sample: survey run January 2026, n = 200 software products. The typical respondent has $1–10M ARR, average revenue per customer of $50–249 a month, and 25–50% year-on-year growth. [DATA] (P, extract) — [ChartMogul](https://chartmogul.com/reports/saas-conversion-report/)
  - Implication for SubOne: the benchmark population is B2B firms with $50–249 monthly ARPA. SubOne's ARPA is £5.75 a month (£69 ÷ 12), with an adult buyer and a child user base. Treat these figures as an upper reference, not a target.
- **ChartMogul, same report:**
  - 57% of products use a free trial as the main entry point, more than twice the share using freemium (26%).
  - 14 days is the most common trial length (62% of products).
  - Trials that require a credit card convert at 30%, "more than 5x" trials that do not. [DATA] (P, extract) — [ChartMogul](https://chartmogul.com/reports/saas-conversion-report/)
  - Implication for SubOne: card-first trials are unsuitable. Schools buy on purchase orders (POs) and invoices (§4), minors are present, and UK subscription rules are tightening (§6). Measure conversion per team per season instead.
- **Kyle Poyar, "What is good & great free-to-paid conversion, 2026 edition":**
  - Freemium: good 3–5%, great 8–12%. Poyar notes that "great conversion is up vs. 2023".
  - Reverse trial: good 4–6%, great 8–12%.
  - Only 7% of products run a reverse trial.
  - Sample: built "with ChartMogul and ProductLed" on "new data from 200 self-serve products", so this is probably the same dataset as the ChartMogul report and not an independent check. [DATA] (P, extract) — [Kyle Poyar note](https://substack.com/@kylepoyar/note/c-209940962); [Growth Unhinged: guide to reverse trials](https://www.growthunhinged.com/p/your-guide-to-reverse-trials) (not opened)
  - Implication for SubOne: under plain freemium, plan on roughly 3–5% of active teams buying Pro. For every 1,000 active teams that is 30–50 paid teams, worth about £2,070–£3,450 a year at £69. At "great" (8–12%) it would be 80–120 teams, worth £5,520–£8,280. This is arithmetic, not a forecast.
- **Lenny Rachitsky with Kyle Poyar (OpenView) and Pendo, "What is a good free-to-paid conversion" (published 1 August 2023; survey of 1,000+ products):**
  - Self-serve freemium: good 3–5%, great 6–8%.
  - Sales-assisted freemium: good 5–7%, great 10–15%.
  - Free trial: good 8–12%, great 15–25%.
  - 20% of freemium products convert under 2.5%. The most common bucket, holding a third of products, is 2.5–5%. [DATA] (P, extract) — [Lenny's Newsletter](https://www.lennysnewsletter.com/p/what-is-a-good-free-to-paid-conversion); [Lenny on X](https://twitter.com/lennysan/status/1686421779479400448)
  - Implication for SubOne: sales assistance goes with roughly double the freemium conversion. For SubOne, "assisted buying" means quotes, PO-ready invoices, a data protection pack and a sponsor-payment link, not a sales team.
- **Aggregator figures (low confidence; method and sample not visible in the extract):**
  - Freemium converts at 2.6%, a no-card opt-in trial at 18.2%, and a card-required opt-out trial at 48.8% trial-to-paid.
  - By category: CRM 29%, AdTech 24.3%, HR software 22.7% trial-to-paid.
  - Source: SaaS benchmark compilations such as [First Page Sage](https://firstpagesage.com/seo-blog/saas-free-trial-conversion-rate-benchmarks/) and [vmobify](https://vmobify.com/blog/free-trial-conversion-rate). Which page each figure came from was not pinned down. [DATA?] (S)
- **Reverse trial defined:** "users start with a free trial, then downgrade to a basic freemium tier after 14 days (see @airtable). These are the best of both worlds." [OPINION] (P) — [Kyle Poyar on X, June 2022](https://x.com/poyark/status/1537064035052568578?lang=en)
- **Claimed reverse-trial uplift:** reverse trials reportedly "lift SaaS freemium-to-paid conversion by 10-40%" compared with standard freemium. No basis was shown. [OPINION] (S) — [SaaS Mag (2026)](https://www.saasmag.com/reverse-trials-replacing-freemium-saas/)
- **Consumer mobile apps (RevenueCat data on 115,000+ apps, reported by Airbridge):** hard paywalls convert 10.7% of downloads to paid by day 30, against 2.1% for freemium. [DATA] (S) — [Airbridge (2026)](https://www.airbridge.io/en/blog/hard-paywall-vs-freemium-2026)
  - Implication for SubOne: this is consumer mobile data and says little about B2B or education. A hard paywall is ruled out anyway by SubOne's "free all season" promise and its no-student-payment rule.
- **Season timing (from sibling notes):**
  - UK national finals: 24–26 March 2026 — [STEM Racing UK](https://www.stemracing.co.uk/stem-racing-uk-national-finals-2026)
  - USA regionals: registration 16 Sep–6 Nov, car due 25 Nov, project documents due 2 Dec (probably the 2026-27 dates) — [STEM Racing USA](https://www.stemracing.us/dates-registration-fees)
  - USA national finals: 12–15 April 2026 — [STEM Racing USA](https://www.stemracing.us/nationals)
  - World Finals 2026: Singapore, 3–7 October 2026 — [Verge Magazine](https://vergemagazine.co.uk/aramco-stem-racing-world-finals-2026-meet-the-future-stars-of-formula-1/)
  - Teams have 3–6 students — [STEM Racing Global](https://www.stemracing.com/aramco-stem-racing-world-finals)
  - Implication for SubOne: the moment of need for Pro (judge-ready packs, what-if simulation, full race-time engineering) falls in the weeks before submission deadlines, not at sign-up.

### Inferences
- **Model fit.** Opinion based on the findings above.
  - (a) **Freemium, SubOne's current model.** This is the right base. It matches free-for-education norms (Canva, Figma, Onshape, Autodesk Fusion; see §3) and the promise that students never pay.
  - (b) **Time-boxed reverse trial at sign-up.** This would show 3D comparisons early, but it would probably expire in September or October, before the late-season Pro features matter.
  - (c) **Event-based reverse trial (preferred).** Give a no-card Pro preview once per season, anchored to the team's first real deadline. For example, 14 days of full Pro in the run-up to regional submission, reverting automatically to Free with nothing deleted.
  - (d) **Card-required trial.** Reject it: it conflicts with invoice buying, the adult-only payer and the direction of UK subscription law.
- **Choice of metric.** B2B benchmarks count conversion per account. SubOne's account is one team with one adult buyer, so the headline metric should be "paid teams ÷ teams active this season", cut by country and by competition class. A second metric should be "paid teams ÷ teams that reached milestone X", where X is, for example, a first race-run log or a first portfolio draft.
- **Small market, so freemium alone won't pay.** Finals-level volumes in the sibling notes are small: 83 teams from 34 countries at the 2025 World Finals ([STEM Racing](https://www.stemracing.com/news/lunar-crowned-aramco-stem-racing-world-champions-2025)) and 27 teams at the 2025 North America national finals ([SCCCA](https://www.sccca.org/news/2025/05/01/cultural-express/charles-wu-leads-team-sw1ft-take-3rd-at-stem-racing-north-america-finals/)). The whole base is probably thousands of teams, not millions, so a 3–5% freemium conversion gives modest revenue. School, trust, organiser and sponsor bulk deals (§4, §5) are the likely levers.

### Gaps
- No conversion benchmark was found for education, extracurricular-team or strongly seasonal products.
- OpenView/High Alpha 2024–2026 product benchmark reports, ProfitWell/Paddle conversion studies and the full ChartMogul and Growth Unhinged articles could not be opened.
- The reverse-trial uplift figure is unverified.
- No data was found on how long free users take to convert (for example, the share converting in the first 30, 90 or 180 days).
- The total number of STEM Racing teams worldwide and by country was not found.

## 2. Pricing structure: per-team vs per-seat, tiers, annual vs monthly, seasonal passes and add-ons

### Takeaway
Pricing units split by market:
- **Youth-team apps** charge per team (TeamSnap, Heja, GameChanger's season Team Pass, Hudl club).
- **School products** charge per student, per teacher or per institution (Seesaw, Kahoot).
- **Collaboration tools** charge per seat (Notion), with flat-rate exceptions such as Basecamp.

For a team capped at 3–6 students, a flat per-team price is the norm and avoids policing seats. A third tier sold to institutions (school, trust or club, several teams on one invoice) is how Hudl, Heja and Seesaw sell to organisations.

SubOne's school-year price (£69) is a 36% discount on 12 months of monthly billing, close to TeamSnap's roughly 40%. But competition seasons often run only 6–8 months, so the £9 monthly plan can be cheaper for many teams, and the "annual" price needs to be designed as a season pass.

### Cited Findings
- **TeamSnap, per team:**

  | Plan | Monthly | Annual | ≈ GBP a year | Limits |
  |---|---|---|---|---|
  | Basic | $9.99 | $69.99 | £53 | 500 MB, 30 roster members |
  | Premium | $13.99 | $99.99 | £75 | 2 GB, 40 members |
  | Ultra | $17.99 | $129.99 | £98 | unlimited storage and members |

  A free version and a 21-day trial also exist. Prices from 2026 extracts. [PRICE] (S) — [TrustRadius](https://www.trustradius.com/products/teamsnap/pricing); [TeamSnap pricing page](https://www.teamsnap.com/pricing) (not opened)
  - By my calculation the annual prices are 40–42% below 12 monthly payments. For example, $69.99 ÷ $119.88 = 58%.
  - Implication for SubOne: £69 per team per year sits between TeamSnap Basic (≈£53) and Premium (≈£75). SubOne's 36% annual discount is in line with the closest per-team youth comparable.
- **Heja:**
  - The app is "free for everyone on the team to use", with no limit on players or guardians.
  - Team Pro and Pro Max are "priced per team", and with Team Pro "the entire team benefits from a single payment".
  - Teams upgrading 2 or more squads can ask for a custom club quote.
  - One App Store user review says the Pro version costs $12 a month (≈£9); this is unverified.
  - [PRICE model] (P, help centre extract; the price is S) — [Heja: Free vs Team Pro](https://help.heja.io/en/articles/3727834-heja-free-vs-team-pro-or-max); [Heja: upgrading](https://help.heja.io/en/articles/9235139-upgrading-to-team-pro-or-pro-max); [App Store reviews](https://apps.apple.com/us/app/heja/id1157335714?see-all=reviews&platform=iphone)
- **GameChanger:** Team Passes (Plus and Premium) are "a one-time purchase that last for an entire season". Premium adds season stats, spray charts, full videos and highlight clipping. Prices were not captured. [PRICE model] (P, extract) — [GameChanger Team Pass](https://gc.com/pricing/team-pass); [Team Pass FAQs](https://help.gc.com/hc/en-us/articles/7286489078413-Team-Pass-FAQs)
  - Implication for SubOne: a paid season pass is an established pattern in youth sport. "£69 per school year" can be presented as a "Season pass".
- **Hudl:**
  - High school program packages cost $1,500, $2,500 and $4,000 per program per year (≈£1,128, £1,880 and £3,008), where one program is one sport. The Athletic Department Package is quote-only and "consolidates every sport onto one invoice".
  - Club and youth basketball team plans cost $400, $1,000 and $1,600 per team per year (≈£301, £752 and £1,203), "as of July 2026".
  - [PRICE] (S) — [HoopBrief (2026)](https://hoopbrief.com/blog/how-much-does-hudl-cost-2026); [Hudl HS pricing](https://www.hudl.com/pricing/high-school) (not opened)
  - Implication for SubOne: institutions buy multi-team bundles on one invoice, which supports a SubOne "School" plan covering several teams (Entry, Development and Professional classes).
- **Basecamp:** $15 per user per month (≈£11), or a flat $299 per month (≈£225) for unlimited users. Per-seat is cheaper for small teams, and the flat plan wins at about 20 or more users. [PRICE] (S) — [Carly (2026)](https://www.usecarly.com/blog/basecamp-pricing/); [ProofHub](https://www.proofhub.com/articles/basecamp-pricing)
- **Annual-plan data from ProfitWell/Paddle:**
  - The share of subscriptions on annual plans varies with ARPU. Low-ARPU companies see "over 50%" on annual, mid-range companies about 20–30%, and high-ARPU companies a high share again.
  - Their claim: "Annual subscriptions can make a SaaS company profitable immediately with just 10% of customers switching to an annual plan and a 1-month discount."
  - [DATA]/[OPINION] (P, extract; sample and date not shown) — [ProfitWell: annual plans reduce churn](https://blog.profitwell.com/why-annual-plans-are-crucial-for-reducing-your-churn); [ProfitWell: why every SaaS needs an annual plan](https://blog.profitwell.com/here-is-why-every-saas-company-needs-an-annual-plan); [Paddle: annual plans](https://www.paddle.com/resources/annual-plans)
- **Size of annual discounts:** observed discounts range from 13% to 67%, averaging about 35%, and the most common is 17% (about "two months free"). [DATA] (S; method not shown) — [Subscription Index](https://www.subscriptionindex.com/guides/annual-vs-monthly-pricing)
- **Retention by billing period:** "Annual plans retain 92% of customers, while monthly plans retain only 68%." [DATA] (S; original study not identified) — [Baremetrics](https://baremetrics.com/blog/annual-vs-monthly-pricing-better-retention)
- **Per-student school licences (Seesaw):**
  - $11.95 per student at list (≈£9).
  - $7.75 through a consortium, and $7.50 on a two-year deal.
  - [PRICE] (S/P) — [Vita-Learn](https://vita-learn.org/seesaw/); [Seesaw help](https://help.seesaw.me/hc/en-us/articles/35336214537997-Subscribe-to-Seesaw)
  - Implication for SubOne: a school buying per student for a 6-student team would pay about $72 (≈£54). £69 per team is the same order of magnitude as per-student school software.

### Inferences
- **Season-length arithmetic (my calculation).**
  - Break-even between the plans is 7.7 months.
  - A UK team active October to March (national finals in late March) pays £54 on monthly billing, 22% less than £69.
  - A US team active September to April (finals mid-April) pays about £72, roughly the same.
  - Only World Finals teams, whose season runs to October, clearly gain from the school-year price.
  - So a teacher paying by card who cancels after finals will rationally choose monthly, and monthly cannibalises the season pass.
- **Options (opinion, untested):**
  - (1) Define the pass as "12 months from purchase" rather than "until 31 August". This covers World Finals in October and a mid-season purchase.
  - (2) Raise monthly to about £12, so 6 months (£72) exceeds the pass.
  - (3) Keep £9 a month but present the pass as the default for invoice and sponsor payments, where one payment matters more than the total.
  - Whichever option is chosen, test it against actual season lengths by country.
- **Per-team vs per-seat.**
  - Team size is fixed at 3–6 by competition rules, so per-seat pricing could at most double revenue, and it would make the teacher decide which students get a seat.
  - Per-team pricing fits the unit of competition and mirrors TeamSnap, Heja and GameChanger. Keep it.
- **Tiers.** A "good-better-best" set split by buyer fits better than one split by feature:
  - Free (whole team, all season).
  - Pro (one team).
  - School or Trust (N teams, one invoice or PO, a data processing agreement (DPA) and data protection impact assessment (DPIA) pack, admin view).
  - Optionally, an Organiser or Region licence (every team in a region, funded by a sponsor; see §5).
  - This follows the Hudl department, Heja club and Seesaw school patterns. It is opinion.
- **Add-ons.** Keep AI measured in "questions" rather than "credits", and let only the adult buyer purchase any top-up (§8, §9).
- **Local prices.** Show prices in the buyer's national currency (GBP, EUR, USD, AUD and so on). The EU guidelines on minors expect any purchase shown to minors to be priced in national currency (§9).

### Gaps
- No current prices were found for GameChanger Team Pass or Heja Team Pro, and the TeamSnap page could not be opened.
- No data was found on season-pass vs monthly uptake in youth sport.
- The ProfitWell annual-share figures lack a visible date and sample size.

## 3. Education and youth-team comparables: price points and who pays

### Takeaway
Two patterns dominate:
- **Free for verified schools, with institutions paying for admin tiers.** Canva, Figma, Onshape, Autodesk Fusion and GitHub are free to verified teachers and students. They are cross-subsidised by professional markets, or monetised through school and district licences (Seesaw, Kahoot, Onshape Education Enterprise, Figma K-12 Enterprise).
- **Free team apps with a per-team paid tier bought by the adult organiser.** TeamSnap, Heja, GameChanger and Hudl club work this way.

Parent-paid premiums exist (ClassDojo Plus, GameChanger family plans), but only in family-facing B2C settings.

The tools STEM Racing teams already use for CAD and CFD are free through sponsorship. SubOne's £69 per team per season sits in TeamSnap's band, far below Hudl, and close to per-student school licence costs for a 6-student team.

### Cited Findings

| Product | Who pays | Price point (original) | ≈ GBP | Date / status | Source |
|---|---|---|---|---|---|
| Canva for Education | Free (Canva) | Free for verified K-12 teachers and their students. Teachers verify with an education email or proof of employment; students must be invited by a teacher; school admins can disable premium features | £0 | 2026 | [Canva eligibility](https://www.canva.com/education/eligibility-guidelines/); [Canva for schools](https://www.canva.com/education/schools/); [Canva students](https://www.canva.com/education/students/) (P, extract) |
| Figma for Education | Free (Figma) | Free. K-12 gets the Enterprise plan "through their school or district"; secondary and higher-ed students get Professional. K-12 verification lasts 2 years, higher-ed 1 year. No commercial use | £0 | 2026 | [Figma Help](https://help.figma.com/hc/en-us/articles/360041061214-Figma-for-Education); [Figma Education](https://www.figma.com/education/) (P, extract) |
| Notion Education | Free for higher-ed individuals only | Education "Plus" plan free with a 1-member limit and up to 100 guests. Needs a school email listed in the World Higher Education Database (WHED); **K-12 not eligible**. AI is a 20-response trial; full AI requires Business at $20 per user per month, with no student discount | $20 = £15 | 2026 | [Notion Help](https://www.notion.com/help/notion-for-education) (P); [Professional's Toolkit](https://professionalstoolkit.com/articles/notion-pricing); [Primo Notes](https://primonotes.com/blog/notion-pricing-complete-breakdown-for-students) (S) |
| GitHub Education / Copilot | Free (GitHub) | Verified students: "Copilot Student" plan from 12 March 2026, with unlimited completions and an allowance of AI credits (200 a month per a secondary source). Verified teachers: free Copilot Pro | £0 | 2026 | [GitHub Docs](https://docs.github.com/copilot/how-tos/manage-your-account/free-access-with-copilot-student); [GitHub community](https://github.com/orgs/community/discussions/189268); [GitHub teachers](https://github.com/education/teachers) (P, extract); [Fast.io](https://fast.io/resources/github-copilot-free-access/) (S) |
| Onshape (PTC) | Free for individuals; institutions pay for Enterprise | Student and Educator plans free; the Educator plan covers "educators, coaches, mentors, and administrators", with eligibility "based on educational use—not email domain". Education Enterprise (single sign-on, bulk upload, analytics) is "a paid plan" for schools and districts. **Conflict:** PTC made Education Enterprise free in 2020 | n/a | 2026 page; 2020 press release | [Onshape plans](https://www.onshape.com/en/education/plans); [Onshape Enterprise](https://www.onshape.com/en/education/enterprise) (P, extract); [PTC 2020](https://www.ptc.com/en/news/2020/ptc-onshape-education-enterprise-plan-available-free-of-charge) |
| Autodesk Fusion (STEM Racing) | Sponsor (Autodesk) | Official CAD/CAE/CAM partner; "every student and teacher" gets free Fusion; free CAD/CAM training (CPD) for teachers in the UK, USA, Germany and India | £0 | 2025–26 | [Autodesk STEM Racing](https://www.autodesk.com/education/competitions/stem-racing); [STEM Racing: Autodesk](https://www.stemracing.com/partners/autodesk); [ETIH](https://www.edtechinnovationhub.com/news/stem-racing-and-autodesk-roll-out-free-computer-aided-design-and-manufacturing-training-for-teachers) (P, extract) |
| Ansys CFD (STEM Racing) | Sponsor (Ansys) | "Exclusive global partner for CFD simulation for STEM Racing teams providing access to free software". Synopsys cites 400,000+ students in 65 countries | £0 | 2025–26 | [Ansys](https://www.ansys.com/academic/students/student-teams/stem-racing) (via sibling notes) |
| Seesaw | Schools/districts; teachers on the free tier | Starter (free): 1 active class per teacher, 1 teacher per class, 35 students; after 30 June 2026 users over the limits "may need to delete content" to keep adding. Plus: $120/yr. School list price $11.95 per student; consortium $7.75. **Conflict:** Seesaw's help says licences are sold only to schools and districts, with "no paid teacher licenses" at present | $120 = £90; $11.95 = £9 | 2026 | [Seesaw Starter changes](https://seesaw.com/pricing-packages/free-changes/); [Seesaw help](https://help.seesaw.me/hc/en-us/articles/35336214537997-Subscribe-to-Seesaw) (P, extract); [Vita-Learn](https://vita-learn.org/seesaw/); [SaaSworthy](https://www.saasworthy.com/product/web-seesaw/pricing) (S) |
| ClassDojo Plus | **Parents** | $15.49/month or $109.99/year for existing US members (announced January 2024). Varies by region, reported at $8–15/month or $40–110/year. 7-day free trial | $109.99 = £83 | Jan 2024 (US); 2026 range | [ClassDojo Help (US update)](https://help.classdojo.com/hc/en-us/articles/23430793537293-ClassDojo-Plus-Updates-for-Existing-Members-in-the-United-States); [ClassDojo Plus](https://www.classdojo.com/plus/) (P); [BeeNet](https://beenet.app/blog/is-the-classdojo-app-really-free-what-it-costs-in-2026/) (S) |
| Kahoot! | Teachers or schools | One source: teacher plans "start at $228/yr" ($19/month billed annually). School tiers per teacher per month: EDU Plus $3–5, Premium $6–10, Premium+ $9–15. Districts buying for 50+ teachers "frequently" negotiate 15–30% off. **Low confidence** | $228 = £171 | 2026 | [Wooclap](https://www.wooclap.com/en/blog/kahoot-pricing/); [Vendr](https://www.vendr.com/marketplace/kahoot) (S) |
| Quizlet Plus for Teachers | Teacher | $35.99/year; 30-day free trial | £27 | 2026 | [Brighterly](https://brighterly.com/blog/quizlet-cost/); [Nibble](https://nibble-app.com/blog/quizlet-cost) (S) |
| Hudl | School athletic department or club | High school: $1,500–4,000 per program per year. Club/youth: $400–1,600 per team per year | £301–3,008 | July 2026 | [HoopBrief](https://hoopbrief.com/blog/how-much-does-hudl-cost-2026) (S) |
| TeamSnap | Coach, club or parents | $69.99–129.99 per team per year; $9.99–17.99 per team per month | £53–98 | 2026 | [TrustRadius](https://www.trustradius.com/products/teamsnap/pricing) (S) |
| GameChanger | Families or teams | Team Pass (Plus or Premium) is a one-time purchase per season; family plans exist; price not captured | n/a | 2026 | [GameChanger](https://gc.com/pricing/team-pass); [family plans](https://gc.com/pricing-family-plans) (P) |
| Heja | Team admin or club | Free for the whole team; Team Pro per team (a user review says about $12/month); club quotes | ≈£9/month (unverified) | 2026 | [Heja help](https://help.heja.io/en/articles/3727834-heja-free-vs-team-pro-or-max) (P); [App Store review](https://apps.apple.com/us/app/heja/id1157335714?see-all=reviews&platform=iphone) (S) |
| Spond | Free; **earns from payment fees** | "Spond is a free platform and only makes money when club and group users process their payments through Spond", with processing by Stripe. The group or its members can cover the fee | £0 plus fees | 2026 | [Spond help](https://help.spond.com/app/en/articles/118091-payments-costs-in-the-spond-app); [Spond blog](https://www.spond.com/news-and-blog/free-app-for-sports-club-payments/) (P) |
| Strava | Individual (adult or family) | UK: £54.99/year or £8.99/month. Family plan: $139.99/year for up to 4 people, annual only | £54.99 | 2026 | [Stamford Cycling](https://stamfordcycling.co.uk/blog/strava-discount-code/) (S); [Strava Family Plan](https://support.strava.com/hc/en-us/articles/26013043116173-Strava-s-Family-Plan) (P) |

- Implication for SubOne (CAD and CFD are free): teachers' reference price for "software for this competition" is £0, because Autodesk and Ansys give it away. Pro must therefore be justified by results the teacher can see, such as judge-ready packs, simulation and time saved. The free tier must stay genuinely usable for a whole season, as SubOne already promises.
- Implication for SubOne (Notion excludes K-12): large horizontal tools avoid the K-12 compliance burden. A tool that complies properly (§9) and sells to schools occupies a gap they leave open.
- Implication for SubOne (parent-pay models): ClassDojo Plus and GameChanger family plans show parent payment works in family B2C. SubOne should still not adopt it, because of the CAP rules on direct exhortation and pester power (§9) and its own no-student-payment promise.
- Implication for SubOne (Spond): a free product funded by payment fees is a distinct model. SubOne could process sponsor payments into team funds, but that adds regulated-payments complexity. This is noted as an option, not a recommendation.

### Inferences
- **Partner model.** The Autodesk and Ansys pattern ("official partner, free to every team, paid for by the partner's marketing budget") is the dominant way software reaches these teams. SubOne could pursue official "team workspace" partner status, with Pro free or discounted for all registered teams and funded by a sponsor or the organiser. That partner model could raise more money than team-by-team conversion (see §5). This is opinion.
- **Price anchors.** £69 per team per season falls in three familiar ranges:
  - The TeamSnap per-team range (£53–98).
  - Seesaw's per-student school licence for 3–6 students (≈£27–54).
  - About one Strava annual subscription for one athlete (£54.99).
  - It is not an outlier. The more important question is who pays (§4, §5).

### Gaps
- No data was gathered on Microsoft 365 or Google Workspace for Education, Padlet, Miro or Slack education pricing.
- Official price pages for Kahoot, Quizlet, Hudl, TeamSnap, Heja and GameChanger could not be opened, so their figures rest on secondary sources.
- Seesaw's Plus price conflicts with its own help text.
- Onshape Education Enterprise's current price is unknown.
- Minimum ages for Autodesk Education and Strava were not verified.

## 4. How schools buy software: UK (maintained schools, academies and trusts), the US, and elsewhere

### Takeaway
UK schools buy through authority delegated under each school's or trust's finance policy: named authorised signatories, an official order or purchase card before an invoice, and quotes above set limits. Maintained schools run April–March financial years; academies run September–August.

Since 9 July 2026, DfE guidance on procuring EdTech treats purchases as a governance decision covering data protection, safeguarding, AI, cyber security, contracts and oversight. A £69 purchase is normally within a budget holder's authority, but only once the supplier clears the data protection checks (DPIA support, DPA, privacy information) and can accept a PO and send an invoice.

US districts use requisition-to-PO workflows, approved-vendor lists and, increasingly, signed student data privacy agreements (the SDPC National Data Privacy Agreement). Many teachers also spend their own money on classroom needs.

### Cited Findings
- **DfE EdTech procurement guidance.** DfE published guidance on procuring educational technology on 9 July 2026, inside its "Data protection in schools" guidance. It covers what to consider "before, during and after procuring EdTech tools" and "the key points that you should discuss with a potential supplier".
  - It states: "When you buy or start using EdTech, you must make sure that the processing of personal data complies with data protection law." Data protection by design and by default should be built into the use of any tool.
  - Commentators describe EdTech procurement as "a connected governance decision involving data protection, safeguarding, AI, cyber security, contracts, vendor accountability, filtering and monitoring, and ongoing oversight". [RULE] (P, extract via commentary) — [GOV.UK: Procuring EdTech](https://www.gov.uk/guidance/data-protection-in-schools/procuring-educational-technology-edtech); [9ine](https://www.9ine.com/newsblog/dfe-edtech-procurement-guidance-the-department-is-joining-the-dots-for-schools)
  - Implication for SubOne: publish a downloadable "Schools pack" as a condition of entry to school budgets. It should contain:
    - A pre-filled DPIA template.
    - A DPA.
    - The sub-processor list and data-location statement.
    - The retention and deletion schedule.
    - An AI-use statement.
    - Safeguarding controls for adult–student chat.
    - A security summary.
    - An accessibility statement.
- **Buying for schools guidance.** GOV.UK's "Buying for schools" guidance was last updated on 16 October 2025 for the 2025–26 academic year. [RULE] (P, extract) — [GOV.UK: Buying for schools](https://www.gov.uk/guidance/buying-for-schools)
- **Get help buying for schools.** This is a free DfE procurement service for state-funded schools and multi-academy trusts. Schools can use frameworks run by the Crown Commercial Service (CCS), including "Education Technology", which DfE has approved for school use. [RULE] (P, extract) — [CCS](https://www.crowncommercial.gov.uk/news/get-help-buying-for-schools); [GHBS solutions](https://get-help-buying-for-schools.education.gov.uk/solutions); [DfE blog: frameworks](https://buyingforschools.blog.gov.uk/2023/05/25/a-beginners-guide-to-using-frameworks-for-school-buying/)
  - Implication for SubOne: at £69 per team, no framework is needed. Frameworks matter only for trust-wide or multi-year deals.
- **Possible certification.** A headline reports that DfE is working on an EdTech certification regime "as ICO flags data-protection issues" (PublicTechnology, 27 August 2026; headline only, article not read). [RULE?] (S) — [PublicTechnology](https://www.publictechnology.net/2026/08/27/education-and-skills/dfe-works-on-edtech-certification-regime-as-ico-flags-data-protection-issues/)
  - Implication for SubOne: watch for a certification scheme. Early compliance documentation could become a sales asset.
- **Financial years.**
  - Maintained schools follow the April–March financial year.
  - Academy trust boards must approve a balanced budget for 1 September–31 August and submit a budget forecast return.
  - Maintained schools' budget plans are commonly submitted between 1 May and 30 June.
  - March and April are busy months for spending decisions, contract renewals and next-year budgets.
  - [RULE]/[DATA] (P/S, extract) — [NGA](https://www.nga.org.uk/knowledge-centre/budget-setting-academy-trusts/); [AllSchools](https://allschools.co.uk/resources/understanding-school-budget-cycles); [Tes](https://www.tes.com/magazine/analysis/specialist-sector/how-do-school-budgets-work)
  - Implication for SubOne: time invoice and renewal pushes for September, which is both the academies' new year and the season start, and for February–March, the maintained schools' year-end. Allow "invoice now, start later" so schools can commit money inside their financial year.
- **Delegated authority.**
  - The headteacher, within powers delegated by the governing body, is responsible for all orders. A list of employees authorised to approve orders, with their limits, is certified each year.
  - Limits vary. Published policies found by search include a finance committee with authority up to £5,000, extra sign-off above £2,500 or £5,000, and petty cash up to £25.
  - Caveat: the exact document behind each figure was not pinned down, and one result was a university department, so treat these figures as illustrative.
  - Some trusts use purchase cards (Windsor Academy Trust purchase card policy, 2019).
  - [RULE] (P documents, extract) — [Richmond schools financial regulations](https://richmond.gov.uk/media/3227/pdf-schfinregs.pdf); [Ealing: orders and invoices](https://www.egfl.org.uk/finance-and-data/funding-and-finance/schools-financial-procedures/orders-and-invoices); [Suffolk MAT finance policy](https://d3hgrlq6yacptf.cloudfront.net/suffolkmat/content/pages/documents/mat-finance-policy-and-procedures-for-schools.pdf); [Milton Keynes procedures](https://www.milton-keynes.gov.uk/sites/default/files/2023-08/Financial%20Procedures%20for%20Schools%20Aug23_aa.pdf); [WAT purchase card policy](https://www.kingswinfordacademy.org.uk/assets/downloads/policies-and-procedures/Useful-Information_policies_windsor-academy-trust-policies_wat-purchase-card-policy-approved-f_a-13.09.19-1.pdf)
  - Implication for SubOne: £69 is usually below any extra sign-off threshold, but it still needs an official order or purchase card.
    - Accept PO numbers on invoices.
    - Offer bank transfer and card payment on the invoice.
    - Complete supplier-setup forms quickly.
    - Issue a PDF quote the teacher can attach to a requisition.
- **DfE Technology in Schools Survey 2024–25.** Run by IFF Research, it surveys headteachers and senior leaders, teachers and IT leads. It tracks progress towards DfE's aim that every school meets six core digital and technology standards by 2030. [DATA] (S, extract; sample size not captured) — [ETIH](https://www.edtechinnovationhub.com/news/dfe-tech-survey-reveals-major-shifts-in-school-ai-use-digital-strategy-and-infrastructure-gaps)
- **When the ICO Children's Code applies to EdTech.** The ICO's EdTech guidance says the Code applies where a service is accessed "on a direct-to-consumer basis", or is provided through a school but the provider "influences the nature and the purpose of the processing".
  - It does not apply only if all three conditions hold:
    - The service fulfils the school's public tasks, as "an integral function of the School rather than a helpful product".
    - Data is processed "solely on the instruction of the School", with no use beyond that, such as product development.
    - The service is not accessed direct-to-consumer.
  - The ICO "is willing to look beyond the terms of any contract". [RULE] (P, extract; S) — [ICO: Children's code and EdTech](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/the-children-s-code-and-education-technologies-edtech/); [Bates Wells](https://bateswells.co.uk/updates/edtech-and-the-application-of-the-ico-childrens-code/)
  - Implication for SubOne: teams sign up directly, SubOne improves its own product, and STEM Racing is often extracurricular. So SubOne is likely a controller for at least some processing and must meet the Children's Code itself. Offering schools a DPA helps, but it does not remove the Code duties.
- **UK teachers' own money.**
  - One in five primary and secondary teachers contributed their own money to pupils' pastoral or welfare needs, typically £74–83 between September 2023 and March 2024 (NFER, 2024). [DATA] (S) — [Fortune](https://www.fortune.com/europe/2024/06/05/uk-teachers-strike-severely-underpaid-spending-own-money-to-help-students-nfer-study)
  - Nearly half of 4,386 teachers surveyed by the NASUWT union had spent their own money on basic necessities in the previous year. [DATA] (S) — [Schools Week](https://schoolsweek.co.uk/teachers-buying-more-basic-equipment-for-pupils-survey-finds/)
  - 73% regularly bought stationery. [DATA] (S) — [Tes](https://tes.com/news/exclusive-teachers-are-spending-hundreds-pounds-year-classroom-supplies)
- **US teachers' own money.**
  - Average out-of-pocket spending in 2024–25 was $895 (≈£673), up 49% since 2015. 97% said their budget was not enough, and the median school-provided supply budget was $200 (≈£150). Source: AdoptAClassroom.org, Spring 2025 survey. [DATA] (P, extract; n not captured) — [AdoptAClassroom](https://www.adoptaclassroom.org/2025/06/09/2025-teacher-survey-spending-stats-classroom-needs/)
  - DonorsChoose reported $655. [DATA] (S) — [The 19th](https://19thnews.org/2025/08/teachers-spending-school-supplies-debt-crowdfunding/)
  - Implication for SubOne: a teacher paying by card is realistic, but it is often the teacher's own money. £69 is about 10% of a US teacher's typical annual out-of-pocket spend. Make reimbursement easy with expense-ready VAT receipts and a "send this invoice to my school's finance office" option, and never assume the teacher should absorb the cost.
- **US district purchasing.**
  - "Upon approval, the Central Office Accounting Department will convert the requisition to a purchase order".
  - Purchases above set amounts "frequently require approval by a district's board of education", and "in some states, only items on an approved list can be purchased".
  - Approved-vendor rules vary by state and by district.
  - [RULE/practice] (P district page; S) — [Needham Public Schools](https://www.needham.k12.ma.us/departments/business__operations/business_office/purchasing/procurement_information); [K12 Prospects](https://www.k12prospects.com/how-to-get-on-a-school-districts-approved-vendor-list/); [Digital Promise](https://digitalpromise.org/online-learning/digital-learning-playbook/purchasing-and-preparing-devices-and-software/)
  - A vendor-side source claims district audits find "100 to 200+ vendors, many adopted by individual teachers without any formal review". [OPINION/claim] (S) — [Career Clutch](https://careerclutch.ai/blog/procurement-checklist-for-district-edtech-contracts.html)
- **US student data privacy agreements (SDPC).**
  - The Student Data Privacy Consortium's National Data Privacy Agreement (NDPA) exists so vendors need not sign one-off contracts with each of "over 13,000 US school districts". Version 2 was released in April 2024.
  - The SDPC registry holds "130,000+ signed Data Privacy Agreements" between "more than 12,000 schools/districts and 6674 education application providers".
  - SDPC says the 275,000+ standard agreements executed since 2016 saved about $111M. That estimate assumes $250 an hour and 1 hour per agreement. [DATA] (P, extract) — [A4L: NDPA](https://home.a4l.org/the-student-data-privacy-consortium-announces-the-release-of-the-national-data-privacy-agreement/); [A4L: NDPA v2](https://a4l.org/student-data-privacy-consortium-sdpc-announce-the-release-of-the-national-data-privacy-agreement-version-2/); [SDPC](https://privacy.a4l.org/national-dpa/)
  - Implication for SubOne: before selling to US districts, sign the NDPA and any state variants and list in the SDPC registry. This is the US counterpart of the UK Schools pack.
- **Who influences US purchases.** An EdWeek Market Brief survey on security purchases (September 2026) found influence split as follows: school leaders 34%, district finance and budget leaders 31%, technology leaders 29%, operations leaders 26%. It notes that smaller needs "can originate with teachers or principals". [DATA] (S; a different product category) — [EdWeek Market Brief](https://marketbrief.edweek.org/meeting-district-needs/security-vendors-are-flooding-k-12-which-district-officials-have-influence-on-what-gets-bought/2026/09)
- **Elsewhere: Ireland.** A 2026 World Finals fundraising campaign was run on GoFundMe by the school's patron body, the Longford & Westmeath Education and Training Board. Education boards can therefore be a paying or fundraising entity. [DATA] (P) — [Westmeath Independent](https://www.westmeathindependent.ie/2026/07/03/apex-racing-launches-fundraising-campaign-for-singapore-world-finals/); [GoFundMe](https://www.gofundme.com/f/apex-racing-world-finals-2026)

### Inferences
- **What UK schools will ask a supplier for.** Opinion, built from the DfE and ICO findings and from standard school finance practice:
  - An official order or PO, or a purchase card.
  - Supplier details: company name and number, address, VAT status, bank details on the invoice.
  - An invoice showing the PO number.
  - A DPA if SubOne is the school's processor, or clear controller terms if it is not.
  - Support for the school's own DPIA.
  - A privacy notice written for students.
  - Data location and international transfers.
  - Retention and deletion at the end of the contract.
  - Security measures.
  - Safeguarding: how adult mentors who are not school staff can message students, moderation, and reporting.
  - AI disclosure: models used, retention, and no training on student data.
  - An accessibility statement.
- **Trust-level licences.** Multi-academy trusts centralise finance under a chief financial or operating officer, with higher sign-off thresholds. A trust licence (all teams across the trust's schools, one invoice, one DPA) fits their buying model better than many £69 purchases. This is inferred from trust finance policies and the Hudl and Heja institutional packages.
- **Who pays in STEM Racing specifically.** Teams run their own sponsorship income; the 2026-27 rules make the Resource Manager responsible for "tracking expenses and income generated and allocating funds" ([2026-27 regulations](https://static1.squarespace.com/static/6913005a89f25e1a2f5bcef5/t/6a1d9375a869f15bc0bbdf98/1780323189128/STEM+Racing+Competition+Regulations+2026-2027+DEV+PRO+(1).pdf), via sibling notes). For many teams, "the team's sponsor money pays" may therefore be easier than "the school pays". SubOne should support both paths from day one.

### Gaps
- **VAT.** Not researched. Open questions: the UK registration threshold, whether SubOne charges 20% VAT to schools, and how maintained schools (through their local authority) and academies recover VAT. SubOne should confirm its own VAT status and show it on the pricing page.
- **Evidence gaps.**
  - No survey data was found on what teachers can personally approve, for example a typical budget-holder limit.
  - No evidence was found on whether UK schools require an accessibility statement from suppliers. The public-sector accessibility regulations apply to schools' own sites; how they apply to vendors was not researched.
  - No sourced material was found on Keeping Children Safe in Education (KCSIE) expectations for adult–student messaging.
  - BESA and HolonIQ data on UK school EdTech budgets was not accessed.
  - Procurement norms were not researched for Australia, the UAE, Saudi Arabia, Singapore, the EU or Canada.
- **Leads not read.**
  - [UCL: why schools cannot procure the technology they need](https://discovery.ucl.ac.uk/id/eprint/10214426/1/Moss_Why%20are%20not%20schools%20able%20to%20procure%20the%20technology%20they%20need%20to%20support%20high-quality%20teaching_report.pdf)
  - [EdTech Magazine, June 2026](https://edtechmagazine.com/k12/article/2026/06/acquisition-accountability-new-era-k-12-technology-decisions)

## 5. Sponsor-, grant- and parent-funded models, and making "your sponsor can pay for Pro" work

### Takeaway
The competition itself runs on sponsorship:
- **Organiser:** a non-profit that relies on corporate sponsors (Aramco sponsors the World Finals title).
- **Software partners:** Autodesk and Ansys give free licences to every team.
- **Teams:** they raise their own money through tiered business sponsors, in-kind technical partners, community fundraising and school or education-board support. "Sponsorship & Return on Investment" is a judged portfolio criterion.

Against roughly €2,156 for one national-level season and €40–50k for a World Finals trip, £69 is a small line item that sponsors will readily fund. That holds only if SubOne lets a sponsor pay directly, with a proper receipt, and helps the team show the sponsorship as return on investment.

### Cited Findings
- **Organiser funding.** The organiser describes itself as a non-profit that relies on corporate sponsors. The 2025 event was billed as the "inaugural Aramco STEM Racing World Finals". [DATA] (P, via sibling notes) — [STEM Racing: Sponsor](https://www.stemracing.com/get-involved/sponsor); [ETIH](https://www.edtechinnovationhub.com/news/singapore-to-host-inaugural-aramco-stem-racing-world-finals)
- **Software partners.** Autodesk gives "every student and teacher" free Fusion and has launched free CAD/CAM CPD for educators. Ansys provides free CFD software to STEM Racing teams. [DATA] (P, extract) — [Autodesk](https://www.autodesk.com/education/competitions/stem-racing); [Autodesk and F1 in Schools press release](https://adsknews.autodesk.com/en/pressrelease/f1-in-schools-and-autodesk-partner-to-deliver-design-software-to-students-worldwide/); [Ansys](https://www.ansys.com/academic/students/student-teams/stem-racing)
- **Sponsorship is judged.** The 2025 World Finals Enterprise Portfolio criteria include "Sponsorship & Return on Investment". The Sponsorship & Marketing Award "recognises teams' ability to negotiate with relevant industry partners to develop mutually beneficial relationships". [RULE] (P/S, via sibling notes) — [SRWF 2025 regulations (Scribd)](https://www.scribd.com/document/878610006/STEM-Racing-World-Finals-Competition-Regulations-2025); [Haas F1 Team](https://www.haasf1team.com/news/moneygram-haas-f1-team-supports-sponsorship-marketing-award-aramco-stem-racing-world-finals)
- **Team budgets.**
  - Caravel Racing (Portugal), regional to national final: "Real cost incurred: 2,155.71€. Marketing budget: 1,555.06€" (≈£1,875 and ≈£1,352). [DATA] (P, team-authored) — [Caravel Racing (GitHub)](https://github.com/Caravel-Racing/CaravelRacing-f1/blob/3c5c12d179905556d9e5c70a08db93e88f3a27a1/server.js)
  - Irish teams going to the 2026 World Finals estimated €40,000–50,000 (≈£34,800–43,500). [DATA] (P news) — [Westmeath Independent, 26 June 2026](https://www.westmeathindependent.ie/2026/06/26/two-athlone-teams-seek-financial-backing-for-world-stem-racing-finals-in-singapore/)
  - Implication for SubOne: £69 is about 3.7% of a national-level season budget and about 0.16–0.20% of a World Finals trip budget. That is a very small sponsor ask.
- **How money flows.**
  - The US team SW1FT used a community non-profit's account, which "provided non-profit account for sponsorship and fund raising". — [SCCCA](https://www.sccca.org/news/2025/05/01/cultural-express/charles-wu-leads-team-sw1ft-take-3rd-at-stem-racing-north-america-finals/)
  - PCBWay's in-kind sponsorship programme hosts pages for STEM Racing teams. — [PCBWay](https://www.pcbway.com/project/sponsor/Ad_Astra_STEM_Racing_World_Finals_Team_92d9a3f0.html)
  - Teams sell tiered sponsorships ("SUPPORTER" up to "PLATINUM") and offer logos on the car, portfolio and social media. — [Team Blitz8 (GitHub)](https://github.com/teamblitz8/teamblitz8.github.io/blob/e76f66166486cf7a6356bdfcd045668b48c2e5af/sponsors/index.html)
  - [DATA] (P, via sibling notes)
- **Registration costs.** STEM Racing USA reportedly charges "no cost to register, participate, or enter the National Finals", but car manufacture and project elements do cost money. [DATA] (S, low-medium, via sibling notes) — [STEM Racing USA FAQ](https://portal.stemracing.us/faq)
- **Parent-paid and family models exist in adjacent markets:** ClassDojo Plus (parents), GameChanger family plans and Team Pass, and the Strava Family Plan. [PRICE] (P/S) — see the §3 table.
- **Payments-funded model.** Spond is free and earns only from payment processing, through Stripe. [DATA] (P) — [Spond help](https://help.spond.com/app/en/articles/118091-payments-costs-in-the-spond-app)

### Inferences
- **Design of "your sponsor can pay" (opinion).**
  - (1) The teacher or mentor creates a "Sponsor link" for the team. It opens a hosted checkout or invoice made out to the sponsor company, with company name, VAT number and PO field, and needs no SubOne account.
  - (2) Payment applies Pro to the team for the season or 12 months. The teacher is notified and stays the account owner.
  - (3) The sponsor receives a receipt or VAT invoice and an optional thank-you certificate ("Software partner of Team X, 2026-27") that the team can use as return-on-investment evidence in its Enterprise portfolio.
  - (4) SubOne shows no sponsor branding to students unless the team chooses to add its own sponsor acknowledgement. This keeps the "no ads" promise.
  - (5) Students never start or see a payment flow.
  - Stripe capabilities for this (Payment Links, hosted invoice pages payable by third parties, custom invoice fields for PO numbers, bank transfer) are believed to exist but were not verified, because Stripe's docs were blocked.
- **Organiser-level or regional sponsorship.** A corporate sponsor, a national STEM Racing operator or an education board could fund Pro for every team in a country or region. This follows the Autodesk and Ansys model and is the most plausible way to reach large numbers of paid teams given the small team counts (§1). This is opinion.
- **Parents.** Avoid parent-pay flows. They create pester-power dynamics, raise CAP Code issues (§9) and break the no-student-payment promise. If a school wants families to contribute, it can pay SubOne's invoice itself and collect from families through its own systems.
- **Grants.** Teams already use education boards (Ireland), community non-profits (US) and crowdfunding. Pro should be purchasable from any of these payers by invoice.

### Gaps
- FIRST robotics sponsor and software-donation programmes, and Formula Student or SolidWorks sponsorship, were not researched because the search budget ran out.
- UK grant sources were not researched. Candidates include Royal Academy of Engineering schemes, STEM Learning/ENTHUSE, local councils and industry trusts.
- No evidence was found of sponsors paying specifically for team software subscriptions, or of how often teams hold their own bank or non-profit account.
- National registration fees for 2025-26 and 2026-27 were not found (the sibling notes record the same gap).

## 6. Paywall and upgrade design: usage limits vs feature gates, moments of need, trials, grace periods and downgrades

### Takeaway
Practitioner evidence, mostly of low rigour, agrees on four points:
- Gate after users have experienced value.
- Combine usage limits (natural triggers) with a few feature gates.
- Trigger prompts on high-signal events: a limit hit, a click on a locked feature, sustained engagement, collaboration.
- Avoid gating so hard that users never reach the "aha" moment.

For a product used by children, regulators add firm limits:
- No manipulative nudges (ICO Children's Code standard 13; the CMA/ICO list of harmful design includes confirmshaming, biased framing and harmful nudging).
- No direct exhortation to children to buy or to persuade adults (CAP Code).
- Transparent pricing in national currency (EU guidelines on minors).
- Clear renewal reminders and easy exit (UK subscription regime from spring 2027).

So SubOne's upgrade prompts should go to the adult buyer, be factual and easy to dismiss, and never put the team's work at risk. A lapse should freeze data, not delete it.

### Cited Findings
- **Where to gate.**
  - Gates are "most effective when placed after a user has experienced clear value". "Gate too aggressively and you prevent users from reaching the aha moment, but gate too loosely and you remove the incentive to upgrade."
  - High-signal upgrade events: "seat limit hit, storage or usage cap reached, locked feature clicked, daily engagement for 10+ consecutive days, or external share or collaboration events".
  - One claim says a hybrid of feature gates and usage limits raised conversion from 3.8% to 7.4%, but no method was disclosed.
  - [OPINION] (S) — [Stackmatix](https://www.stackmatix.com/blog/freemium-to-paid-conversion); [Daydream](https://www.withdaydream.com/library/insights/freemium-conversion-rate); [SaaS Factor](https://www.saasfactor.co/blogs/freemium-vs-trial-models-in-saas-what-really-boosts-conversions)
- **Seesaw's downgrade-limit policy.** The free Starter plan allows 1 active class per teacher, 1 teacher per class and 35 students. After 30 June 2026, users over those limits "may need to delete content they do not need to continue adding new content beyond the Seesaw Starter limits". [DATA] (P, extract) — [Seesaw](https://seesaw.com/pricing-packages/free-changes/)
  - Implication for SubOne: never require a team to delete car versions or portfolio evidence to keep working. When Pro ends, keep over-limit items visible and exportable in read-only form.
- **CMA and ICO joint paper (9 August 2023).** "Harmful design in digital markets" names harmful online choice architecture practices including "harmful nudging", "confirmshaming", "biased framing", "bundled consent" and "default settings". It offers practical guidance for firms. [RULE] (P, extract) — [DRCF paper (PDF)](https://www.drcf.org.uk/siteassets/drcf/pdf-files/harmful-design-in-digital-markets-ico-cma-joint-position-paper.pdf?v=380506); [ICO news](https://ico.org.uk/about-the-ico/media-centre/news-and-blogs/2023/08/ico-and-cma-harmful-online-design-encourages-consumers-to-hand-over-personal-information/)
- **ICO Children's Code, standard 13 (nudge techniques).** Services should not use nudge techniques "to lead or encourage children to provide unnecessary personal data or to turn off privacy protections".
  - Examples given: a large green "yes" button beside a small-print "no"; framing one option more positively than another; making the low-privacy option one click and the high-privacy option six clicks.
  - Nudges towards high-privacy options and parental controls are permitted. [RULE] (P, extract) — [ICO standard 13](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/age-appropriate-design-a-code-of-practice-for-online-services/13-nudge-techniques/)
- **CAP Code and EU guidelines.** The CAP Code bans direct exhortation to children and encouraging pester power (§9). The EU's Article 28 guidelines on minors cover virtual currencies and require national-currency pricing (§9). [RULE] (S/P) — see §9.
- **UK subscription regime (Digital Markets, Competition and Consumers Act 2024).**
  - Traders must send reminder notices before renewals.
  - Consumers get two 14-day cooling-off periods: one at the start, and one on renewal after a free or discounted trial or after a contract of 12 months or more auto-renews.
  - Notices must be in writing, on a durable medium, with an immediately apparent purpose.
  - Commencement is now expected in spring 2027, later than the spring 2026 originally planned. [RULE] (S, law firms) — [Reed Smith](https://www.reedsmith.com/articles/dmcc-subscription-rules-delayed-to-spring-2027-key-takeaways-from-the-consultation-response/); [HSF Kramer (April 2026)](https://www.hsfkramer.com/notes/crt/2026-04/time-to-start-preparing-for-the-new-uk-subscription-contracts-regime); [Burges Salmon](https://www.burges-salmon.com/our-thinking/subscription-contracts-new-measures-to-protect-consumers/)
  - Implication for SubOne: a teacher paying personally may count as a consumer; whether they do is uncertain. Build renewal reminders, a 14-day no-quibble cancellation and one-click cancellation now. Trials should end without an automatic charge.
- **Apple Kids Category (guideline 1.3).** Kids Category apps "must not include links out of the app, purchasing opportunities, or other distractions to kids unless reserved for a designated area behind a parental gate". [RULE] (P, read in full) — [Apple App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/)
  - Implication for SubOne: even on the web, the same principle applies. Purchase opportunities belong in an adult-only area, the teacher's billing page, not on student surfaces.

### Inferences
Upgrade-design rules for SubOne. These are opinion, drawn from the rules and practitioner evidence above:
1. **Show different screens to students and adults.**
   - A student who reaches a Pro feature sees a neutral explanation: what the feature does, and "Your team's plan is managed by your teacher or mentor".
   - The student sees no buy button, no "ask your teacher to upgrade" wording and no countdown.
   - Upgrade calls to action, prices and payment options appear only in the teacher or mentor view. This reflects CAP's direct-exhortation rule and Apple's parental-gate principle.
2. **Trigger prompts to the teacher at moments of need:**
   - When a usage cap is hit: a 4th car version in 3D, an 11th AI question in a month, a 2nd judge-ready pack.
   - In deadline windows, for example 4–6 weeks before the team's regional or national submission date.
   - When the team repeatedly opens locked features, reported as a team-level count ("your team tried the what-if simulator 3 times this week"), never by named student.
   - Using team activity to market to the teacher is still processing children's data. Keep it aggregated, cover it in the DPIA and privacy notice, and do no individual profiling (Children's Code standard 12, profiling off by default).
3. **Make choices symmetric.** "Not now" should be as visible as "Upgrade". Do not use:
   - Confirmshaming ("No thanks, we don't want to win").
   - Fake scarcity or countdown timers.
   - Pre-selected annual plans.
   - Hidden monthly options.
   - Repeated prompts after a dismissal. Rate-limit them, for example once per feature per week.
4. **Offer no-card Pro previews.** Give an event-based preview (§1) that reverts automatically to Free. Warn the teacher a few days before it ends, and never auto-charge.
5. **Handle lapse and downgrade gently.**
   - Keep all data.
   - Freeze over-limit items read-only but viewable, for example car versions beyond 3 in 3D.
   - Keep judge-ready packs already generated downloadable.
   - Keep export free at all times.
   - Allow a grace period of, for example, 14–30 days after a failed payment or expiry before features lock.
   - Never delete a team's work for non-payment. It is children's work and competition evidence, and the best-interests standard applies.
6. **Mix limits and gates as SubOne already does.** Usage caps (3 car versions in 3D, 1 judge pack, 10 AI questions a month) plus one feature gate (the full simulator) already form the hybrid the practitioner evidence favours. Keep the free tier sufficient to finish a season, as promised.
7. **Price transparently.** Show prices in local currency, including VAT where applicable, per team, with plain units ("AI questions", not credits or tokens).

### Gaps
- No rigorous A/B test evidence on upgrade-prompt design in education or with child users was found.
- No data was found on how grace periods affect retention or recovery.
- Downgrade policies of Notion, Slack, Canva or Figma were not retrieved.
- No evidence was found on how often teacher-facing prompts convert compared with in-context prompts.

## 7. Pricing page design: plans side by side, FAQ and "who pays" clarity

### Takeaway
Only practitioner and vendor claims were found, none with a disclosed sample. They say multiple tiers are near-universal, that three tiers with a highlighted recommended plan lift mid-tier selection, and that clarity drives conversion.

For SubOne, the essentials that do rest on evidence come from the legal and buyer context instead:
- Say plainly who pays: students never pay; a teacher, mentor, school or sponsor can.
- Show per-team prices in local currency.
- Offer the invoice and PO route.
- Publish the school documents buyers need.
- Avoid choice-architecture tricks the CMA and ICO call harmful.

### Cited Findings
- "98% of SaaS companies use multiple tiers, with three being the sweet spot for conversion, while five or more creates paralysis." [OPINION/claim] (S) — [Growigami](https://growigami.com/blog/saas-pricing-page-best-practices); [Fungies (2026)](https://fungies.io/saas-pricing-page-best-practices-2026/)
- Further claims, none with a disclosed method [OPINION/claim] (S) — [LeadSuiteNow](https://leadsuitenow.com/blog/pricing-page-optimization-cro); [Art of Styleframe (2026)](https://artofstyleframe.com/blog/pricing-page-layouts-what-converts-2026/); [Advergize](https://www.advergize.com/anchoring-effect-pricing/):
  - "Recommended plan highlighting increases mid-tier selection by 30-40%."
  - One team went from 1.2% to 3.1% conversion after cutting 5 tiers to 3 and adding a "Most Popular" badge.
  - "Approximately 60-70% of SaaS customers select the middle tier when three options are presented."
  - Top-quartile pricing pages convert "6.5-12% versus a 2.8% average".
- Figma's resource library publishes pricing-page best practices. This is vendor guidance, not data. [OPINION] (P) — [Figma](https://www.figma.com/resource-library/pricing-page-best-practices/)
- **Legal overlays:**
  - The CMA and ICO list of harmful design (§6).
  - EU guidance that purchases shown to minors be priced in national currency (§9).
  - Future UK requirements for pre-contract information and reminders (§6).
  - [RULE] — see §6 and §9.

### Inferences
Pricing page checklist for SubOne (opinion):
- **"Who pays" first.** Put a short block at the top: "Students never pay. A teacher or mentor can buy Pro by card, a school can pay by invoice or purchase order, and a sponsor can pay with a sponsor link." This builds trust with teachers and avoids child-directed selling.
- **Plans side by side:** Free (whole team, all season) | Pro (one team) | School or Trust (several teams, one invoice). Label Pro factually. Show a "Most popular" badge only if it is true, because a false one is misleading under UK consumer law and would be a harmful design choice.
- **Clear season terms.** Offer "Season pass (12 months) / Monthly" with the total price, the dates covered, and what happens at the end: nothing is deleted, and the team keeps Free.
- **FAQ covering:**
  - What happens when Pro ends.
  - Data protection: UK GDPR, the Children's Code, DPA available, no ads, no third-party trackers.
  - VAT status.
  - Refunds and cancellation.
  - The AI allowance and what happens at the limit.
  - Safeguarding for adult–student chat.
  - Accessibility statement.
  - Which countries are supported and in which currencies.
- **Buying tools.**
  - A downloadable Schools pack (§4).
  - A PDF quote generator for requisitions.
  - Supplier details.
  - A "pay by invoice" form that captures a PO number.
- **No student-facing marketing.** Student accounts link to the page only for information, with no calls to action shown to them in the product.

### Gaps
- No large-sample or peer-reviewed evidence on pricing-page layout was found. All the numbers above are unverified practitioner claims.
- No education-specific pricing-page studies were found.

## 8. Pricing AI features: credits, caps, included allowances and margins (2025–2026)

### Takeaway
In 2025–26, AI in SaaS is usually priced through:
- A monthly allowance included in the plan.
- Hard caps or paid overage.
- Credit packs.

Education programmes give only small AI allowances. Notion's education plan offers a 20-response trial. GitHub's Copilot Student plan reportedly includes 200 AI credits a month.

Practitioner sources put AI product gross margins at about 50–60%, against 80–90% for classic SaaS, so caps matter. SubOne's 10 (Free) and 200 (Pro) questions per team per month is structurally in line. The risks are cost per heavy Pro team, free-tier AI cost at scale, and showing minors something that looks like a currency.

### Cited Findings
- **GitHub Copilot Student.** Complimentary Copilot access has been managed under the Copilot Student plan since 12 March 2026, with "unlimited code completions and an allowance of AI credits". Secondary sources put the allowance at 200 AI credits a month. Verified teachers get free Copilot Pro. [PRICE] (P extract; S for the number) — [GitHub community](https://github.com/orgs/community/discussions/189268); [GitHub Docs](https://docs.github.com/copilot/how-tos/manage-your-account/free-access-with-copilot-student); [Fast.io](https://fast.io/resources/github-copilot-free-access/)
- **Notion.** The free Education Plus plan includes "a limited AI trial of 20 responses per workspace". Ongoing AI needs the Business plan at $20 per user per month (≈£15), which has no student discount. [PRICE] (S) — [Professional's Toolkit](https://professionalstoolkit.com/articles/notion-pricing); [Primo Notes](https://primonotes.com/blog/notion-pricing-complete-breakdown-for-students)
- **Common AI pricing patterns.**
  - Plans include "a monthly amount of credits … with consumption beyond that amount priced separately". The overage rate is "typically two to four times the underlying cost". The rule is to "bundle baseline AI, monetize heavy AI".
  - Credit systems are said to have "won" for consumer and prosumer SaaS.
  - "92% of AI software companies now use mixed pricing models", citing an unnamed 2025 industry report.
  - [OPINION/DATA] (S; original study not identified) — [Stigg](https://www.stigg.io/blog-posts/overage-pricing); [Monetizely](https://www.getmonetizely.com/blogs/the-economics-of-ai-first-b2b-saas-in-2026); [Coommit](https://coommit.com/blog/saas-ai-pricing-2026); [Dodo Payments](https://dodopayments.com/blogs/ai-saas-monetization-2026)
- **Margins.** "AI product gross margins are around 50-60%, compared with 80-90% for traditional SaaS". [OPINION/DATA] (S, 2026 blogs; primary data not identified) — [The SaaS CFO](https://www.thesaascfo.com/your-ai-feature-is-quietly-destroying-your-gross-margin/); [Monetizely](https://www.getmonetizely.com/blogs/the-economics-of-ai-first-b2b-saas-in-2026)
- **EU guidance on virtual currencies.** Platforms should not expose minors to "techniques which reduce the transparency of economic transactions … such as a virtual currency", and in-app purchases shown to minors should be priced in national currency. [RULE] (S) — [Hunton](https://www.hunton.com/privacy-and-information-security-law/european-commission-issues-guidelines-on-the-protection-of-minors)

### Inferences
- **Cost ceiling. Illustrative arithmetic only; SubOne's per-question cost is unknown.**
  - A Pro team using its full allowance asks 200 × 12 = 2,400 questions a year. At £0.005, £0.01 and £0.03 per question, that costs £12, £24 and £72, which is 17%, 35% and 104% of the £69 price.
  - A free team using its full allowance asks 120 questions a year. At £0.01 per question, 1,000 free teams would cost about £1,200 a year.
  - To hold AI-product-like margins, per-question cost probably needs to stay well under about £0.01, or the caps need to scale.
- **Design (opinion).**
  - Keep the unit as "AI race engineer questions per team", not credits or tokens.
  - Use hard caps with no overage billing, so schools never get a surprise bill.
  - Show remaining questions to the team plainly, with no scarcity nudges.
  - If demand appears, sell top-ups ("+100 questions") only to the adult buyer, in local currency.
- **Seasonality.** AI use will peak before deadlines, and monthly allowances that reset penalise seasonal teams. A season allowance (for example 1,500–2,000 per season), or rollover within the season, suits the usage pattern better. This is opinion.
- **Procurement link.** The DfE procurement guidance names AI as part of the governance decision (§4). An AI-use statement (models, data retention, no training on student data, safety filtering) belongs in the Schools pack.

### Gaps
- SubOne's model provider and per-question cost are not known here.
- Canva, Figma and Microsoft AI-credit schemes and prices were not retrieved.
- No rigorous AI margin data was accessed, such as ICONIQ or Bessemer reports.

## 9. Legal and ethical limits when users are children, and what they rule out for monetization

### Takeaway
SubOne's current rules already avoid the sharpest prohibitions: no ads, no third-party trackers, students never asked to pay, and only an adult can buy. The remaining obligations are:
- **UK Children's Code:** 15 standards, including best interests, a DPIA, high-privacy defaults, profiling off by default and no nudges towards less privacy.
- **CAP Code:** no direct exhortation to children to buy or to pester adults.
- **EU GDPR Article 8:** national consent ages of 13–16 where consent is the lawful basis.
- **EU Article 28 guidelines on minors (July 2025):** the benchmark for compliance, with no exploitative commercial practices, national-currency prices and no virtual currencies.
- **US COPPA:** amended rules have required compliance since 22 April 2026, relevant if any under-13s use the product.
- **California Age-Appropriate Design Code:** in force in part only, with its dark-patterns clause still enjoined.
- **App-store kids rules:** relevant if an app ever ships.
- **UK subscription regime:** expected from spring 2027.

In practice these rules exclude:
- Student-facing upsells.
- Parent-pester prompts.
- In-app purchases by minors.
- Currency-like credits.
- Manipulative design.
- Profiling for targeting.
- Trial traps.

### Cited Findings
- **The Children's Code has 15 standards.**
  1. Best interests of the child.
  2. Data protection impact assessments.
  3. Age-appropriate application.
  4. Transparency.
  5. Detrimental use of data.
  6. Policies and community standards.
  7. Default settings.
  8. Data minimisation.
  9. Data sharing.
  10. Geolocation.
  11. Parental controls.
  12. Profiling.
  13. Nudge techniques.
  14. Connected toys and devices.
  15. Online tools.
  - [RULE] — [ICO: Code standards](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/age-appropriate-design-a-code-of-practice-for-online-services/code-standards/). The standard names come from background knowledge; the ICO page is linked but was not opened.
- **Standard 13 (nudges):** see §6. [RULE] (P, extract) — [ICO standard 13](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/age-appropriate-design-a-code-of-practice-for-online-services/13-nudge-techniques/)
- **The Code applies to EdTech unless the provider is purely the school's processor:** see §4. [RULE] (P, extract) — [ICO EdTech](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/the-children-s-code-and-education-technologies-edtech/)
- **ICO update (August 2026).** The ICO published a "Children's code strategy progress update – August 2026", which includes a section on its wider children's work. The page title was seen; the content was not read. [RULE] (P) — [ICO August 2026 update](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/childrens-information/childrens-code-guidance-and-resources/children-s-code-strategy-progress-update-august-2026/our-wider-childrens-work)
- **CAP Code (UK advertising rules).**
  - Marketers must not "actively encourage children to make a nuisance of themselves or undermine parental authority" (rule 5.4.1, pester power).
  - "Advertisements must not include a direct exhortation to children to buy or hire a product or service or to persuade their parents, guardians or other persons to buy or hire a product or service for them" (the direct-exhortation rule, numbered 5.9 in the ASA material found).
  - [RULE] (P, extract) — [ASA: Children, credulity and direct appeal](https://www.asa.org.uk/advice-online/children-credulity.html); [CAP Code Section 5 (PDF)](https://www.asa.org.uk/static/uploaded/6eb8845a-776a-4368-a1e1283488b69d44.pdf); [ASA: BCAP rule 5.9 amendment](https://www.asa.org.uk/news/amendment-to-bcap-code-rule-59-direct-exhortations-to-children.html)
  - Implication for SubOne: "Ask your teacher to get Pro" shown to a student is plausibly a direct exhortation to persuade another person to buy. Keep all purchase messages in the adult view.
- **EU Article 28(1) guidelines on minors (Digital Services Act).**
  - Adopted 14 July 2025. They are voluntary but "will be used by the European Commission as a benchmark for compliance with Article 28(1)".
  - They cover age assurance, registration, default settings, platform design, recommender systems, commercial practices, user reporting, content moderation, governance and transparency.
  - Minors should not be exposed to advertising or practices "that may take advantage of their lack of commercial literacy", nor to "a virtual currency that can be exchanged for real money". Any in-app purchases shown to minors should be "priced in the national currency".
  - [RULE] (S, law firms) — [Hunton](https://www.hunton.com/privacy-and-information-security-law/european-commission-issues-guidelines-on-the-protection-of-minors); [Freshfields](https://technologyquotient.freshfields.com/post/102kv4s/dsa-decoded-6-the-european-commission-finalises-guidelines-on-the-protection-of); [HLC](https://www.hlc.com/en/publications/the-longawaited-eu-guidelines-on-article-281-dsa-what-online-platforms-must-know)
  - Implication for SubOne: whether SubOne counts as an "online platform" under the Act at all is uncertain (see Gaps). Even so, adopting the commercial-practice measures (no virtual currency, local-currency prices, no exploitation of commercial inexperience) costs little and matches its promises.
- **GDPR Article 8 (age of consent for online services).**
  - The GDPR default is 16, and member states may lower it to no less than 13.
  - The extract lists Germany, Hungary, Lithuania, Luxembourg, Slovakia and the Netherlands at 16, Austria at 14, France at 15, and the UK at 13.
  - **Conflict:** the same extract also puts Spain, the Czech Republic, Ireland and Poland at 13. Other commonly cited charts, from background knowledge and unverified here, give Spain 14, the Czech Republic 15, Ireland 16 and Poland 16. Verify against [Practical Law's chart](https://uk.practicallaw.thomsonreuters.com/w-021-3094?transitionType=Default&contextData=%28sc.Default%29) or [EuConsent](https://euconsent.eu/digital-age-of-consent-under-the-gdpr/).
  - [RULE] (P/S) — [GDPR Art. 8](https://gdpr-info.eu/art-8-gdpr/); [GDPR Local](https://gdprlocal.com/digital-age-of-consent-under-the-gdpr/)
  - Implication for SubOne: a sign-up minimum of 13 matches the UK age. It does not make consent valid for 13–15-year-olds in countries set at 14–16. Do not rely on consent as the lawful basis for core processing (use contract or legitimate interests, or the school's public task where SubOne acts for a school), and keep consent-based extras, such as marketing emails, off for minors.
- **US COPPA amendments.**
  - Published 22 April 2025, effective 23 June 2025, with compliance required by 22 April 2026.
  - Personal information now includes biometric identifiers.
  - Operators need separate verifiable parental consent before disclosing children's data for purposes not "integral" to the service, such as targeted advertising.
  - Operators need a written information security programme and a written data retention policy.
  - The FTC did not codify school authorisation for EdTech ("not finalizing the proposed amendments … related to ed tech and the role of schools at this time") but "will continue to enforce COPPA in the ed tech context consistent with its existing guidance".
  - [RULE] (P, extract; S) — [Federal Register](https://www.federalregister.gov/documents/2025/04/22/2025-05904/childrens-online-privacy-protection-rule); [Securiti](https://securiti.ai/ftc-coppa-final-rule-amendments/); [Loeb & Loeb](https://www.loeb.com/en/insights/publications/2025/05/childrens-online-privacy-in-2025-the-amended-coppa-rule); [Public Interest Privacy Center](https://pipc.tech/new-coppa-update/)
  - A law-firm headline says the FTC "prioritizes COPPA enforcement as new compliance obligations take effect" (article not read). — [Davis Polk](https://www.davispolk.com/insights/client-update/ftc-prioritizes-coppa-enforcement-new-compliance-obligations-take-effect)
  - Implication for SubOne: the competition includes students aged 9 to 19 ([Autodesk and F1 in Schools press release](https://adsknews.autodesk.com/en/pressrelease/f1-in-schools-and-autodesk-partner-to-deliver-design-software-to-students-worldwide/)). The age gate at 13 must therefore be neutral, not nudging children to lie. Any future teacher-managed accounts for under-13s would bring in COPPA (in the US) and parental-consent rules (in the EU).
- **California Age-Appropriate Design Code.** On 12 March 2026 the Ninth Circuit narrowed the injunction against the Act.
  - NetChoice had not met the standard for facial relief against the Act's coverage definition or its age-estimation provision, so those are no longer enjoined on that basis.
  - The court agreed the data-use restrictions and the dark-patterns prohibition "likely are unconstitutionally vague", so those stay enjoined.
  - The case returns to the district court on age estimation and severability.
  - [RULE] (S, law firms) — [Cooley (30 March 2026)](https://www.cooley.com/news/insight/2026/2026-03-30-netchoice-v-bonta-ninth-circuit-narrows-injunction-against-californias-ageappropriate-design-code-act); [Holland & Knight](https://www.hklaw.com/en/insights/publications/2026/03/ninth-circuit-issues-mixed-ruling-on-california-age-appropriate-design); [DLA Piper](https://privacymatters.dlapiper.com/2026/03/the-ninth-circuits-latest-caadca-ruling-navigating-an-evolving-compliance-landscape/)
  - Implication for SubOne: this status is in flux. Build to the UK Children's Code, which is broadly similar and fully in force, and it will largely cover California.
- **Apple App Store Review Guidelines (read in full).**
  - Guideline 1.3: Kids Category apps may not include purchase opportunities except behind a parental gate. They "should not include third-party analytics or third-party advertising", with narrow exceptions, and "may not send personally identifiable information or device information to third parties".
  - Guideline 5.1.4: apps that collect personal information from a minor "must include a privacy policy and must comply with all applicable children's privacy statutes". The "parental gate requirement … is generally not the same as securing parental consent".
  - Guideline 2.3.8: terms such as "For Kids" and "For Children" in app metadata are reserved for the Kids Category.
  - [RULE] (P, read in full) — [Apple App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/)
  - Implication for SubOne: if a mobile app ever ships, it would probably sit outside the Kids Category because users are 13–19. Guideline 5.1.4 still applies. Do not describe the app as "for kids" in its metadata, and keep purchases in an adult-only area.
- **UK subscription rules and harmful design:** see §6. [RULE]

### Inferences
What these rules rule out for SubOne's monetization. This is analysis, not legal advice.
- **Advertising and tracking.** No targeted or behavioural advertising, and no third-party trackers or SDKs on student surfaces. SubOne already complies. The relevant rules are:
  - COPPA's separate consent for non-integral disclosures.
  - Children's Code standards 9 (data sharing) and 12 (profiling off by default).
  - Apple guidelines 1.3 and 5.1.4.
  - Article 28(2) of the Digital Services Act, which bans profiling-based ads to minors on platforms (background knowledge; text not opened here).
- **Student-facing selling.**
  - No upsell calls to action, prices or "ask your teacher or parents" prompts shown to students (CAP direct exhortation and pester power; Apple parental-gate principle; EU guidelines on commercial literacy).
  - No purchase flows reachable from student accounts.
- **Currencies and game mechanics.** No virtual currencies, credits, loot-box-like mechanics, or streaks and rewards tied to paying (EU guidelines; Children's Code standard 5 on detrimental use and standard 13 on nudges).
- **Manipulative design.** None in any flow, including the teacher's: no confirmshaming, biased framing, asymmetric buttons, countdowns or pre-ticked options (CMA/ICO paper; standard 13; UK consumer law). California's equivalent clause is enjoined, but UK and EU rules still apply.
- **Data use for selling.**
  - No profiling of individual students to target upsells.
  - Team-level usage signals sent to the adult buyer are lower risk, but need to be covered in the DPIA and privacy notice (standards 2, 4 and 12).
- **Subscription traps.** No auto-charging trials. Send renewal reminders, allow easy cancellation, and follow the 14-day cooling-off rules, which are expected to be mandatory for UK consumers from spring 2027.
- **What stays allowed.** Freemium with usage limits and feature gates; adult-only purchase by teacher, mentor, school or sponsor; season passes; invoices; team-level AI allowances; factual, easy-to-dismiss prompts to adults; and positive nudges towards privacy-protective choices, which standard 13 explicitly permits.

### Gaps
- **US.**
  - The FTC Negative Option ("click-to-cancel") rule status in 2026 could not be checked because the search budget ran out. Background knowledge suggests the Eighth Circuit vacated it in July 2025; this is unverified.
  - US state student privacy laws (such as SOPIPA) and state children's design codes other than California's were not researched.
- **EU Digital Services Act.** Two questions are unanswered. Does Article 19's exemption for micro and small enterprises exempt SubOne from Article 28 obligations? And is a private team workspace with chat an "online platform" at all? Both are unverified.
- **UK.**
  - Online Safety Act duties were not researched. SubOne's chat makes it a user-to-user service likely to be accessed by children, so Ofcom's children's risk-assessment and protection codes may apply. This is highly relevant to school procurement (safeguarding).
  - The CAP Code's definition of a child (believed to be under 16) and the exact current rule numbers were not verified. How the ASA applies CAP to in-app messages about a service's own paid tier was not researched.
- **Other jurisdictions.** Children's data laws were not researched for Australia (Children's Online Privacy Code, in development), the UAE, Saudi Arabia, Singapore (PDPA advisory guidelines for children) and Canada.
- **Google Play.** Families policy text could not be accessed.
