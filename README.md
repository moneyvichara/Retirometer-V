
RETIROMETER V
From Retirement Corpus to Regular Pension

Plan Your Meaningful Retirement
PFRDA HACKATHON 2026
India's Most Comprehensive NPS Retirement Planning Tool
9 Intelligent Modules   ·   27 Interactive Charts   ·   3 Proprietary Scores
Full Bilingual EN / Hindi   ·   PFRDA-Compliant   ·   100% Offline Single-File Tool

Submitted by  

Vishweshwar Mensumane
Associate Professor
Presidency College, Bengaluru
Money Vichara - https://moneyvichara.blogspot.com/
February 2026
 
1. Executive Summary
Retirometer V is a professional-grade, browser-based retirement planning suite built specifically for India's National Pension System (NPS) ecosystem. It is the only tool that combines NPS accumulation projection, holistic multi-asset corpus integration, annuity strategy comparison, multi-dimensional risk scoring, and sustainability simulation into a single coherent planning journey — fully governed by PFRDA regulatory rules.

Delivered as a single self-contained HTML file, it requires no installation, no server, and no account. A subscriber opens the file in any modern browser and has immediate access to nine intelligent modules, 27 interactive Chart.js visualisations, three proprietary retirement health scores, full bilingual support in English and Hindi, and a one-click print-to-PDF personalised report.

9
Planning Modules	27
Interactive Charts	3
Proprietary Scores	10
Asset Classes	EN/हि
Bilingual

💡	Core Mission
Transform the abstract complexity of NPS retirement planning into a clear, actionable, deeply personal picture — empowering every Indian pension subscriber to understand exactly where they stand, what they need, and how to get there.

Key Specifications
Specification	Detail
Format	Single-file HTML — no server, no install, works fully offline after first load
File Size	~248 KB — loads instantly in any modern browser
Visualisations	27 interactive Chart.js charts with tooltips, animations, and custom data labels
Languages	Full bilingual toggle — English and Hindi (187 translated strings, instant switch)
Regulatory Compliance	PFRDA rules enforced at UI level — 40% annuity minimum hard-coded into every slider
Data Sync	Global Profile Sync (GPS) propagates user inputs across all 9 modules in real time
Report Export	One-click print-to-PDF generates a personalised multi-page retirement planning report
Tax Transparency	NPS 60% lump-sum tax-free, annuity taxed at slab rate — displayed as inline notes
 
2. The Problem Being Solved
India's NPS subscriber base has crossed 7.5 crore accounts. Yet the vast majority of subscribers plan retirement with one of three inadequate tools: a basic online corpus calculator that returns a single number, a financial advisor who speaks in jargon, or a spreadsheet last updated years ago.

The real challenge of retirement planning is not computing a corpus — it is understanding the interplay between multiple variables across a 50-year time horizon. Most existing tools fail to address these six critical questions:

•	What is the difference between nominal corpus and real purchasing power — and why does it matter in practice?
•	Why is guaranteed income (annuity, EPF pension) fundamentally different from market-linked corpus drawdown?
•	How does a market crash in Year 1 of retirement permanently damage a corpus more than one occurring 10 years later?
•	Which annuity structure — life, joint, return-of-premium, or inflation-linked — actually fits a specific family situation?
•	What is the compounding cost of delaying NPS contributions by even two or three years?
•	Is a subscriber's full financial ecosystem — EPF, PPF, mutual funds, FD, property — sufficient or dangerously concentrated?

Retirometer V addresses all six gaps simultaneously, in one coherent and sequenced planning journey.
 
3. Unique Architecture
3.1 Global Profile Sync (GPS)
A persistent sticky bar below the navigation contains 10 fields: Name, Current Age, Retirement Age, Plan-To Age, NPS Balance, Monthly Contribution, Step-Up %, Monthly Expenses, Inflation %, and Expected Return %. Any change propagates instantly to the corresponding input in all nine modules — no page reload, no copy-paste. This eliminates the most common planning error: using inconsistent assumptions across different calculators.
3.2 Module Progress Tracker
A row of nine colour-coded dots sits below the GPS bar. Each dot turns saffron when its module is active, and teal-green once Calculate has been clicked and results generated. At a glance, users can see exactly which modules have been run and which remain pending — useful during demos and self-guided exploration.
3.3 Module Data Flow — "Push to" Architecture
One-click transfer buttons pass computed outputs directly between modules: Push to Risk Dashboard (M3 to M5), Push to Annuity Optimizer (M3 to M4), Use in Goal Finder (M1 to M2), and Pull from NPS Simulator or Corpus Integrator (M1/M3 to M8). This creates a directed data flow mirroring the natural planning sequence, ensuring downstream modules use upstream-computed values.
3.4 Full Bilingual Support — English and Hindi
A single-click toggle in the header switches 187 text strings across all nine modules — chart titles, gauge labels, metric names, button text, tab names, and card descriptions — instantly without a page reload. The Noto Sans Devanagari font is pre-loaded specifically for Hindi rendering quality.
3.5 Print-to-PDF Personalised Report
The print button triggers a CSS @media print stylesheet that hides all navigation and interactive elements, renders a personalised header with the user's name from the GPS field, and shows all nine modules sequentially with clean page breaks. Charts render as static images. The result is a professional multi-page retirement planning document ready to share with a financial advisor.
3.6 PFRDA Compliance Enforced at the UI Level
Retirometer V actively prevents users from modelling regulatory violations rather than merely warning about them:

•	All annuity allocation sliders have a hard minimum of 40% — the PFRDA mandatory purchase floor. Values below this are impossible to set.
•	When GPS age is 65 or above, a real-time alert appears noting the NPS entry age cap.
•	When retirement age is below 60, Module 9 surfaces the 80% annuity rule for premature NPS exit.
•	Tax notes explain 60% lump-sum tax-free treatment and annuity income taxed at the subscriber's income slab rate.
 
4. Nine Modules — Detailed Walkthrough
Each module is fully independent but designed to flow naturally into the next. All inputs stay consistent via the GPS bar.

MODULE 1	NPS Growth Simulator  —  Accumulation Phase Engine

The foundation module. Projects NPS corpus under three scenarios aligned to PFRDA's Lifecycle Fund classifications: Conservative (LC-25, ~8% p.a.), Moderate (LC-50, ~10% p.a.), and Optimistic (LC-75, ~12% p.a.). The core formula is the Future Value of a Growing Annuity (FVGA) with annual step-up compounding:

FV = PV x (1+r)^n  +  PMT x sum of [(1+g)^i x (1+r)^(n-1-i)]  for i = 0 to n-1
Where r = annual return, g = step-up rate, n = years to retirement. This correctly models salary-linked NPS contributions that increase each year — unlike simple SIP calculators that assume flat contributions throughout.

Key Outputs and Charts
•	Three-scenario corpus cards — Conservative, Moderate, and Optimistic — each showing nominal and real (inflation-adjusted) corpus side by side
•	Uncertainty band chart — a shaded range across all three scenarios, not a single projected line, giving an honest picture of the range of plausible outcomes
•	Retirometer Risk Gauge — a 6-band colour instrument measuring the Safe Withdrawal Rate (SWR) from Comfortable at under 2% to Critical at over 7%
•	Withdrawal Coverage Ratio (WCR) — percentage of the full retirement period the corpus sustains inflation-adjusted withdrawals at a 7% post-retirement return
•	Contributions vs Investment Returns stacked chart — shows exactly how much of the final corpus is the subscriber's own money versus compounding gains
•	Retirement Journey Milestones — visual timeline with corpus estimates at 25%, 50%, 75%, and 100% of the accumulation period

⚠️	Scope Note in Module 1
The gauge measures risk based on NPS corpus alone vs total retirement expenses. A clear orange warning box above the gauge and a teal reminder below it both direct users to Module 3 (Corpus Integrator) for their complete multi-asset score.







MODULE 2	Goal Finder  —  Reverse Calculator

Most calculators answer how much will I accumulate. Module 2 inverts the question entirely: what corpus and monthly contribution do I need today to achieve my desired monthly pension? The full calculation chain is displayed verbatim in the UI, making every assumption visible and auditable.

Today's pension (today's Rs) → inflated to retirement date → PV-annuity corpus → total corpus at 40% NPS allocation → required monthly SIP

The annuity corpus uses a proper Present Value of Annuity formula for a finite retirement horizon — not a perpetuity approximation, which overstates the required corpus by 15–30%.

Key Outputs and Charts
•	Pension Adequacy Arc Gauge — an animated SVG semicircle showing current plan adequacy as a percentage against the stated pension goal
•	Cost of Delay chart — shows precisely how the required monthly SIP increases if the subscriber waits 2, 5, 8, or 10 more years before starting; the most emotionally compelling output in the tool
•	Monthly Pension vs Contribution Change — bar chart across 7 scenarios: -15%, -10%, -5%, Current, +5%, +10%, +15%, with a dashed gold target pension line for instant visual calibration
•	Monthly Pension vs Retirement Age — bar chart showing pension at every 2-year retirement age from 12 years early to 10 years late, with the planned age highlighted in teal with a star

💡	Pension Definition Advisory in Module 2
A prominent advisory box distinguishes guaranteed pension (NPS annuity, EPF pension, FD interest) from supplementary market drawdown. The planning thumb-rule is stated explicitly: aim for 60-70% of monthly expenses covered through guaranteed income before retirement.

MODULE 3	Holistic Corpus Integrator  —  Complete Wealth Picture

NPS is rarely a subscriber's only savings instrument. Module 3 integrates all 10 asset classes into a single unified retirement picture — the first module of its kind in the NPS planning ecosystem. It makes the critical distinction between guaranteed income (annuity, EPF pension, FD interest) and market-linked drawdown (NPS lump sum, mutual funds, equity), which feeds directly into the proprietary PSI score.

Asset Class	Type	Default Return	Notes
NPS	Market-linked	10% p.a.	Step-up compounding; annuity portion computed separately
EPF / Gratuity	Guaranteed	8.25% p.a.	Flat monthly contribution assumed
PPF	Guaranteed	7.1% p.a.	Flat monthly contribution assumed
Mutual Funds	Market-linked	12% p.a.	User-editable; SIP modelled
Stocks / Equity	Market-linked	13% p.a.	User-editable; direct equity
Property	Market-linked	7% p.a.	Investable value or rental income
FD / Bonds	Guaranteed	7% p.a.	Interest treated as guaranteed income floor
Gold / Commodities	Market-linked	8% p.a.	User-editable
International / Crypto	Market-linked	12% p.a.	High risk; clearly flagged
Other Savings	Mixed	7% p.a.	User-defined return

Key Outputs and Charts
•	Growth Table — each asset's current balance, monthly contribution, return rate, projected retirement value, growth multiple, and % of total corpus
•	Growth Chart — multi-line time series showing how each asset compounds from today to retirement, with NPS/MF/equity applying the step-up rate
•	Allocation Shift — two side-by-side donut charts showing portfolio composition today vs at retirement, with auto-generated insight text explaining the shift
•	Crossover Point Alert — auto-detects and flags the age at which guaranteed income surpasses market-linked income, a significant milestone in retirement security planning
•	PSI Gauge — Pension Stability Index displayed on the Retirometer colour scale, computed from total multi-asset guaranteed income vs expenses

MODULE 4	Annuity Optimizer  —  Four Pension Strategies

At retirement, NPS subscribers face one of the most irreversible financial decisions of their lives: how to split the corpus between annuity purchase and lump-sum withdrawal. Module 4 makes this fully transparent by simultaneously modelling four distinct strategies across three time horizons.

Strategy	Structure	Year 1 Income	Key Trade-off
Pure Annuity	100% corpus to annuity	Highest guaranteed	No lump sum; fully illiquid
Balanced Split	User-defined % annuity + managed lump sum	Moderate guaranteed + market	Best of both; customisable split
Lump Sum Heavy	40% annuity + 60% lump sum drawdown	Lowest guaranteed	Maximum flexibility; corpus depletion risk
Phased Drawdown	Annuity base + systematic withdrawal	Moderate, declining	Sustains longer if markets cooperate

Key Outputs and Charts
•	Monthly income at Year 1, Year 10, and Year 20 for all four strategies on a single grouped bar chart — revealing long-run income divergence
•	Corpus Depletion curve — year-by-year balance of the lump-sum portion under each strategy, clearly marking when corpus reaches zero
•	Inflation Erosion chart — real purchasing power of a fixed annuity over 30 years; a Rs 50,000/month annuity at 6% inflation is worth only Rs 15,686/month in real terms after 20 years
•	All four annuity types with quantified payout adjustments: Life (baseline), Joint Life (~10% lower), Return of Premium (~8% lower), Increasing 3% p.a. (~15% lower starting)


MODULE 5	Retirement Risk Dashboard  —  Three Proprietary Scores

The analytical heart of Retirometer V. Three proprietary metrics deliver a multi-dimensional view of retirement security that no single corpus number can capture.

Score	Formula	What It Measures	Target
PSI Pension Stability Index	Guaranteed Income / Annual Expenses x 100	Percentage of expenses covered by income that cannot stop — annuity, EPF pension, FD interest — regardless of how markets perform	>=75%
RSR Retirement Sufficiency Ratio	Total Income (all sources) / Annual Expenses x 100	Whether combined guaranteed + market-linked income covers total retirement expenses. 100% = break-even; above 130% = comfortable surplus	>=130%
LCS Longevity Coverage Score	Years corpus stays positive: return -3%, inflation +2% vs inputs	How many years the corpus survives when returns disappoint and inflation exceeds expectations simultaneously — the true worst-case test	= Full horizon



Key Outputs and Charts
•	6-Dimension Retirement Health Radar — hexagonal chart scoring across Income Adequacy, Longevity Safety, Corpus Strength, Inflation Resilience, Sequence Risk, and Liquidity / Diversification
•	Market Shock Test — corpus trajectory under normal conditions vs a -40% crash in Year 1 of retirement, illustrating sequence-of-returns risk with specific corpus values at Age 80 and Age 85 under both scenarios
•	Inflation Erosion chart — real purchasing power of Rs 1 lakh fixed annual income plotted over 30 years at the user's inflation rate
•	Auto-generated personalised advice — text calibrated to the exact PSI / RSR / LCS shortfall, suggesting specific corrective actions rather than generic guidance

💡	Radar Trade-off Transparency
The tool explicitly educates users that Liquidity and Sequence Risk are inherent trade-offs — more market income improves flexibility but increases sequence-of-returns risk, and both cannot be maximised simultaneously. This nuance, rarely surfaced in consumer tools, is explained with a note below the radar.

MODULE 6	Scenario Lab  —  Side-by-Side Planning

Three fully independent scenarios — each with its own age, corpus, contribution, step-up, return rate, inflation, and retirement age — are computed simultaneously and compared side by side. The defaults are deliberately meaningful: Current Plan, Higher Contribution, and Early Start (age 25 vs 32), immediately demonstrating that starting 7 years earlier with a smaller SIP can outperform a larger contribution started later.

Key Outputs and Charts
•	Winner badge — automatically crowns the scenario with the highest projected corpus, with corpus and pension figures for all three
•	Parallel corpus growth chart — three coloured growth lines on a single axis for instant visual comparison across all scenarios
•	Key Metrics Comparison — grouped bar chart with corpus and pension side by side for all three scenarios
•	Real Pension Value Over Time — shows how each scenario's pension income erodes in real purchasing power terms post-retirement
•	Sequence-of-Returns Risk panel — unique to Module 6; two retirement trajectories for Scenario A with identical long-run average returns but different timing demonstrate that when returns arrive matters as much as their average

MODULE 7	NPS Fund Optimizer  +  Tax Calculator

Answers the question NPS subscribers ask most but rarely get a data-driven answer to: should I choose Active Choice or Auto Choice, and what is the right E/C/G split? Interactive sliders for Equity (E, capped at 75%), Corporate Bonds (C), and Government Securities (G) auto-balance to 100% in real time, with the blended return computed live as the weighted average.

Key Outputs and Charts
•	Full comparison table: Active Choice custom allocation vs LC-75, LC-50, and LC-25 Auto Choice — showing corpus, monthly pension, and performance gap vs the best option
•	NPS Tax Benefit Calculator: Section 80CCD(1) deduction against the Rs 1.5 lakh 80C ceiling, net of other 80C investments entered by the user, plus Section 80CCD(1B) exclusive Rs 50,000 additional deduction independent of the 80C limit
•	Cumulative Tax Savings chart — the compounding tax benefit visualised over the full contribution period; for a 30% slab taxpayer, combined deductions can save up to Rs 75,000 per year
•	Active Choice donut chart showing E/C/G allocation and the live blended return assumption

MODULE 8	Corpus Sustainability Simulator  —  Retirement Runway

Answers the question at the centre of every retiree's anxiety: will my money outlive me? Simulates year-by-year corpus drawdown under realistic dual-inflation conditions — the critical distinction from simpler tools. General inflation (default 6%) is modelled separately from medical inflation (default 12%), reflecting India's actual healthcare cost escalation trend.

Key Outputs and Charts
•	Primary result banner — states clearly whether the corpus survives to life expectancy, or the exact age it runs out if it does not
•	Sustainable withdrawal amount — the inflation-adjusted monthly drawdown that keeps the corpus alive for the full planning horizon, computed by reverse simulation
•	Year-by-year drawdown chart with corpus line, total expense overlay, and depletion point explicitly marked
•	Annual Expense Breakdown — stacked area chart separating general living expenses from medical expenses, each growing on its own inflation curve
•	3-Bucket Strategy — auto-allocates corpus into Bucket 1 Liquid (0-5 years), Bucket 2 Balanced (5-15 years), and Bucket 3 Growth (15+ years), a widely recommended approach to reduce sequence-of-returns risk in early retirement
•	Full scrollable Year-by-Year Retirement Runway table — corpus opening, annual expense, other income, corpus closing, and traffic-light status for every year from retirement to life expectancy

MODULE 9	Pre-Retirement Health Check  +  35X Rule

Steps back from accumulation arithmetic to ask a more fundamental question: before I optimise my returns, am I protected against the risks that could derail everything? Functions as a pre-retirement financial safety audit covering five critical dimensions.

Traffic Light Safety Net Check
•	Emergency Fund — checks whether current fund covers the 6-month expenses benchmark; flags the gap in rupees
•	Term Insurance — validates against the 10x annual income thumb-rule, quantifying any under-insurance
•	Health Insurance — checks against the recommended Rs 10 lakh minimum sum insured for urban India
•	Savings Rate — computes actual monthly savings as a percentage of take-home income and benchmarks against the 20% target

35X Corpus Rule
Industry consensus: a corpus of 35 times annual retirement expenses sustains a ~3% Safe Withdrawal Rate comfortably across a 30-year retirement. Module 9 computes the 35X target in nominal future rupees, current readiness as a percentage, the gap in rupees, and the monthly SIP required to close the gap from today.

Retirement Age Sensitivity Table
Shows required monthly savings across retirement ages from 50 to 68, letting subscribers see exactly what earlier retirement costs in contribution terms and whether each age is feasible relative to their current income — expressed as a percentage of take-home pay.

⚠️	PFRDA Early Exit Warning
When retirement age is below 60, Module 9 automatically surfaces: PFRDA Early Exit Rule — withdrawal before age 60 requires 80% of NPS corpus for annuity purchase versus the standard 40%. Plan accordingly. This regulatory detail is frequently overlooked in early retirement planning.
 
5. Unique Differentiators
The following are the unique capabilities of Retirometer V

Differentiator	Why It Matters
PSI — Pension Stability Index	First proprietary score separating guaranteed income from total income. Shows what % of expenses are covered even if all markets go to zero. No existing tool makes this distinction.
RSR — Retirement Sufficiency Ratio	Holistic sufficiency across all 10 income sources — not just NPS. Reveals real-world retirement security, not just corpus size.
LCS — Longevity Coverage Score	Worst-case stress test (return -3%, inflation +2%) showing precisely how many years the corpus survives under simultaneous adverse conditions.
Market Shock Test (-40% Year 1)	Quantifies sequence-of-returns risk with a before/after corpus comparison. Corpus values shown at Age 80 and 85 under both normal and shocked conditions.
3-Bucket Retirement Strategy	Auto-computed liquid/balanced/growth allocation. A sophisticated strategy recommended by CFPs but absent from free tools.
Medical Inflation Modelled Separately	India healthcare costs escalate at ~12% p.a., not 6%. Modelling separately gives an honest picture of late-retirement spending reality.
Crossover Age Analysis	Auto-detects and flags the age when guaranteed income surpasses market-linked income — a landmark insight in retirement income planning.
Cost of Delay Precisely Quantified	Not just warned about but computed in rupees. Shows the exact increase in required SIP for every year of delay at 2, 5, 8, and 10 years.
Contribution & Retirement Age Sensitivity	Two parallel bar charts show pension outcomes across 7 contribution levels and across retirement ages from 12 years early to 10 years late.
35X Rule + Sensitivity Table	The 35X corpus target is standard in financial planning but absent from NPS tools. The sensitivity table across retirement ages makes it immediately actionable.
PFRDA Rules Enforced at UI Level	40% annuity minimum is hard-coded into sliders — not just warned about. Users physically cannot model a regulatory violation.
Global Profile Sync	One change updates all 9 modules instantly. No inconsistent assumptions across calculators — the single biggest source of planning errors eliminated.
 
6. Competitive Comparison
Feature	Retirometer V	Typical NPS Tool	Financial Advisor
NPS accumulation with step-up SIP	Full FVGA formula	Basic flat SIP	Yes
Multi-asset holistic corpus (10 classes)	Yes	NPS only	Manual
Reverse goal calculator with full chain	Yes, chain shown	Partial	Yes
Four annuity strategy comparison	3 time points shown	No	Ad hoc
3 proprietary scores PSI / RSR / LCS	Yes	No	No
Sequence-of-returns shock test -40%	Full simulation	No	Rare
3-Bucket retirement strategy	Auto-computed	No	Rare
Medical inflation separate (12%)	Yes	No	Sometimes
35X rule + retirement age sensitivity	Full table	No	Ad hoc
PFRDA rules enforced at UI level	Hard-coded minimums	Warning only	Advisor discretion
Bilingual English and Hindi	187 strings instant toggle	Sometimes	Rarely
Cost of Delay quantified precisely	Interactive chart	No	No
Contribution + retirement age sensitivity	Two parallel charts	No	No
Personalised print-to-PDF report	One-click	Screenshot only	PDF export
Single file, 100% offline-capable	248 KB HTML	Requires server	Software needed
 
7. Technical Implementation
7.1 Technology Stack
Component	Technology	Rationale
Core Language	Vanilla JavaScript ES6+	Zero framework dependencies; instant load; offline-capable; no build pipeline
Charts	Chart.js 4.4.1 via CDN	Industry-standard; responsive canvas rendering; 27 chart instances across all modules
Typography	Plus Jakarta Sans, Playfair Display, JetBrains Mono, Noto Sans Devanagari	Premium UI stack; monospace for number alignment; Devanagari for Hindi rendering quality
Architecture	Single-file HTML (248 KB)	One file = one share = works everywhere; no server, no build step required
Data Layer	In-memory JavaScript objects	Fast; no localStorage; no privacy concerns; resets cleanly on page reload
Print / PDF	CSS @media print stylesheet	Leverages the browser's built-in PDF engine; no third-party library needed

7.2 Financial Formulae — Verified
Formula	Used In	Verification
FVGA — Future Value Growing Annuity (step-up SIP)	M1, M2, M3, M6, M7, M8, M9	Verified against manual year-by-year simulation; matches to within rounding
FVL — Lump-Sum Future Value (standard compound)	All corpus calculations	Standard formula; independently verified
PV Annuity — Finite-horizon (not perpetuity)	M2 Goal Finder, M3, M4	Correct for 30-year horizon; perpetuity over-states required corpus by 15-30%
reqPMT — Required Monthly Contribution	M2, M9	Reverse-derived via bisection search from the FVGA formula
WCR / LCS — Year-by-Year Corpus Sustainability	M1, M5, M8	Verified against manual spreadsheet with dual inflation curves





7.3 Edge Case Handling
•	Age equals Retirement Age (zero accumulation years) — returns zero corpus with a clear message rather than crashing
•	Life Expectancy at or below Retirement Age — red-border GPS field validation plus alert on Calculate button click
•	Monthly Contribution equals zero (lump-sum only) — FVGA returns zero correctly; FVL handles the lump sum
•	Inflation rate exceeds return rate (negative real return) — safeR = max(-0.99, r) prevents divide-by-zero and negative corpus
•	Zero corpus passed to risk or sustainability modules — alert and early return before any chart generation
•	Annuity rate zero with non-zero annuity allocation — validated on Calculate with a descriptive alert
 
8. Recommended Demo Flow (8–10 minutes)
The following eight steps cover the most impactful capabilities in a structured sequence that builds naturally.

1.	Fill the GPS Bar — Enter name, age 32, retire at 60, NPS Rs 5 lakh + Rs 15,000 per month contribution, expenses Rs 40,000 per month. Point out how all nine module tabs auto-populate immediately from these 10 fields.
2.	Module 1 — NPS Simulator — Click Calculate. Show the uncertainty band across three scenarios, nominal vs real corpus distinction, and the Retirometer Gauge landing in the moderate zone.
3.	Module 2 — Goal Finder — Set desired pension Rs 60,000 per month. Click Find My Goal. Show the full calculation chain, the Cost of Delay chart, and then the two new sensitivity charts — pension vs contribution change and pension vs retirement age.
4.	Module 3 — Corpus Integrator — Add EPF Rs 3 lakh, PPF Rs 1 lakh, Mutual Fund SIP Rs 3,000 per month. Click Analyse. Show Growth Table, Allocation Shift donuts, and PSI Gauge. Click Push to Risk Dashboard.
5.	Module 5 — Risk Dashboard — Click Analyse Risk. Show the three score cards (PSI / RSR / LCS), the 6-dimension radar chart, and the -40% Market Shock Test. This is the most visually striking module in the tool.
6.	Module 6 — Scenario Lab — Click Compare Scenarios. Show how Early Start at age 25 with Rs 8,000 per month beats Higher Contribution at Rs 15,000 starting at age 32. Point out the Winner badge.
7.	Module 8 — Sustainability — Pull corpus from Module 3. Click Simulate. Show the drawdown chart with medical inflation overlay, the 3-Bucket allocation breakdown, and the Year-by-Year Runway table.
8.	Print Report — Click the print button. Show the personalised header with the subscriber's name and date, and the clean multi-page PDF covering all nine modules.

🌐	Hindi Demo Tip
Click the Hindi button in the top-right corner at any point during the demo. All labels, gauge verdicts, chart titles, tab names, and card descriptions switch instantly — a powerful live demonstration of the bilingual architecture.
 
9. Known Limitations and Scope
The following are deliberate scope decisions declared transparently. They do not affect the core planning value of the tool for the vast majority of subscribers.

Limitation	Impact	Mitigation Within the Tool
Constant return in accumulation phase	Corpus may be over or under-stated if actual returns deviate significantly	Three-scenario range in M1; M5 stress test; M6 sequence-of-returns panel
Single-point life expectancy	Survivorship risk is binary rather than probabilistic	Default Plan-To Age set to 90 with explicit note that 50% of people outlive their expected lifespan
Annuity rates are illustrative	Actual monthly pension may differ from projection	Hint text instructs users to verify current rates with their annuity provider before deciding
Tax modelling is approximate	Post-tax corpus may be 10-20% lower than projected	Inline tax note in M1 results; 60% tax-free rule and slab rate taxation clearly explained
No EPF contribution cap enforcement	May overstate EPF corpus for very high earners	Users can manually adjust EPF return rates and monthly contributions in Module 3
Requires internet on first open	Fonts and Chart.js loaded from CDN on first use	Both resources are lightweight and cached by browsers; all subsequent opens are fully offline
 
10. Closing Statement
"From Retirement Corpus to Regular Pension"
Retirometer V does not ask you to trust a number.
It shows you every assumption, every formula, every trade-off — and lets you explore them.
Retirement planning isn’t just about reaching a number — it’s about creating lasting income, clarity, and confidence for the future.


