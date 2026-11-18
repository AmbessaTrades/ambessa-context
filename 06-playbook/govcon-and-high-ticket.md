# Government money and high-ticket selling — what we studied and what we took

Read this after `05-offers/hypotheses.md`. It records two operators we studied in November 2026 and
the model we built from them. **Nothing here is a decision.** The three business shapes at the end are
hypotheses; Ambi decides which one is real.

## Why this file exists

We needed an answer to one question: how does somebody actually get paid by governments and by
seven-figure companies, in public, without an ad budget? Two operators answered it from opposite ends
— one sells a process for winning public contracts, one sells a $28,000 private plan — and the
pattern between them is what we kept.

## Operator one — Rick Howard (GovClose)

Retired US Air Force lieutenant colonel, twenty years as an acquisitions officer, reports managing
$82 billion in contracts, 700+ CEOs trained. He teaches a four-step method, not proposal writing.

**His five load-bearing ideas**

1. **The office, not the agency.** The unit is a named buying office with a budget line — not "the
   Department of Defense".
2. **Obligated, not announced.** Start from money already paid (award records) and work backwards.
   The published tender is the crowded end of the funnel.
3. **Median, not average.** In his own October 2026 sample of 84 AI-related awards: average $3.76M,
   **median $642.7K**, small-business median $464K.
4. **Count the bidders.** Offers-received is the probability field. His table prints Defense at
   **1.80 offers (5/8 records reported)**; Commerce at 7.33. A niche with two bidders is a market.
5. **Arrive before the RFP.** The market-research phase is legal access; after the solicitation
   publishes, contact becomes protest grounds.

**Also worth keeping:** 47 of those awards were full-and-open against 10 small-business set-asides —
certification is not the door. And every one of his numbers carries a denominator and a confession
when the figure is a proxy ("landscaping used as the tree-care proxy", "estimate, still to be
verified"). That discipline is the whole difference between this and a $297 course.

## Operator two — Andrew Henderson (Nomad Capitalist)

A boutique consulting firm selling a "Holistic Plan" to entrepreneurs and investors. His funnel is
published, so it can be read exactly.

| Stage | What it is |
|---|---|
| Content | policy and tax videos with a threat or a number in the title |
| Free proof | **eight proprietary indexes** — Passport, Tax Map, Citizenship Map, Country Intelligence, Beach, Freedom, Lifestyle, Real Estate |
| Capture | one action, "GET STARTED", in the header of every page |
| Qualify | a five-step application, 6–7 minutes |
| Intro call | 45 minutes |
| The gap | plan creation, **8–12 weeks** |
| The close | **a two-hour plan presentation** — "we create Plans, not options" |
| After | implementation as general contractor, plus ongoing support |

**The price is public and the quote is refused: services start at US$28,000, flat fee.** The
qualifier is US$500,000 annual income or US$1M net worth. 1,500+ clients from 100+ countries.

**The five steps, as questions**

1. Personal — name, contact details, preferred contact channel, time zone.
2. Eligibility — nationality, country of residence, age band, criminal record.
3. Goals and financial — what you want, what success means, how you feel about living abroad,
   interests, **your current structure and complexity (trusts, foundations, entities)**, then the
   gate: income US$500K+ / net worth US$1M+ / both / neither, then a net-worth band up to US$30M+.
4. Readiness — how long you have been thinking about it, what has stopped you, which stage you are at.
5. Confirmation — "I'm ready to proceed / later / do not wish", referral code, accuracy confirmation.

**The mechanics worth copying**

- It never asks for a budget. It asks for a **band and a structure**, which is what lets them price
  the deal without capping it.
- The eight-week gap *is* the product: a long diagnostic turns a service into a deliverable, and the
  two-hour presentation is a handover rather than a pitch.
- The free layer is evidence, not a teaser: eight working tools that rank, prove expertise and give a
  reason to come back.
- Scarcity is a headcount, not a countdown: "I can only personally help four people a month".

**The arithmetic that matters:** 1,500 clients × $28,000 = $42M+ against 1.14M subscribers — roughly
**0.13% of the audience paying $28,000.** Reach is not the machine. Arrival is.

## The model we built from them

**A Ledger row** is one buying office × one recurring need: spend, records observed, offers-received
with its denominator, median award, incumbent, recompete date, window (forecast / sources-sought /
live / award-only), fiscal year end, evidence links, and a confidence label of verified, proxy or
estimate. **A row with no evidence link is deleted, not scored.**

**Five passes per country:** the procurement law (thresholds, methods, publication duties) → the
portals and award registers (including what is missing) → 12–24 months of awards grouped by office →
competition (offers, or distinct winners) → the pre-tender window (procurement plans, budgets, donor
pipelines).

**A country pack** is the repeatable unit: law, portals, awards, offices, calendar, triggers, score —
seven files, one checklist, so the second country costs a fraction of the first.

**Sale Odds, 0–100:** money 20 · bidder thinness 20 · window 20 · access 15 · buyer density 15 ·
readiness 10. Gates: no source and date, no score; under three records, ceiling 60 and labelled thin.

**The law of the score: buy the trigger, not the budget.** A policy change, a new register, a
threshold move or a project closing date opens a market. A big budget alone does not.

## What the Caribbean data actually looks like

- **Jamaica** — Public Procurement Act 2015; GOJEP 2.0 publishes tenders *and* contract award
  notices; ≥J$1.5M must run on-platform; a **small-business set-aside is entering force in 2026**.
  The best machine-readable market in the region.
- **Trinidad and Tobago** — the Act requires a public Contract Awards Register; the register currently
  reads "No Contract Awards Published". The vacuum is the product.
- **Guyana** — NPTAB publishes awards, tender-opening minutes, bidder registrations and a
  barred-contractor list; the portal was dismantled for four years and restored in 2021, so history
  has to be rebuilt by hand. Oil money and local-content rules make it the largest spend.

## The three shapes — none chosen

| Shape | Who pays | Price | What must be true |
|---|---|---|---|
| A. Procurement intelligence | firms chasing public money | $50–300/mo | data vacuum, thin competition, a trigger |
| B. Pan-African economics suite | anyone, self-serve | $200–300 up front + ~$50/mo | one irresistible calculation runnable in two minutes |
| C. High-ticket engagement | one firm at a time | $10–15K | we can produce a plan nobody else can |

Chooser: buyer density · pain severity · ability to pay · proof we can produce today · days to first
dollar. Never how impressive it sounds.

## Images

The captures that go with this file are library items 72–86 in `09-assets/library/`:

- `72`–`76` — the five application steps, captured from the live form with mock data, never submitted
- `77`–`80` — the home page, the plan process, the research indexes, the live event
- `81`–`86` — GovClose's field guide, agencies table, set-aside table, average-vs-median, spend chart
  and pipeline diagram

Raw base: `https://raw.githubusercontent.com/AmbessaTrades/ambessa-context/main/09-assets/library/`

## What is verified and what is not

**Verified:** the US$28,000 floor and the five-step question set (walked on the live site); the 84
awards / $316M obligated / $642.7K median / 1.80 Defense offers figures (read from his own screens);
Jamaica's GOJEP obligations; Trinidad's empty register; Guyana's portal history.

**Not verified:** Caribbean spend totals, the count of $5M+ firms per sector, and every price above
except Nomad's own. Treat them as working numbers in a test.
