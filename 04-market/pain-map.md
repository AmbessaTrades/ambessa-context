# The five walls, with the numbers

_What actually blocks a cross-border deal between Africa, the Caribbean and the diaspora. Every figure here traces to a row in evidence/findings.csv._

Every figure here traces to a row in `evidence/findings.csv` (the current count lives there).

---

## 1. How to trust this

Every claim carries a source URL and a verbatim quote. `check.py` re-opens the source and
demands the quote be there; anything that fails is hidden by default. No X post, no Reddit
thread, no blog and no AI summary is treated as a pain. Research came from
U.S. State Department 2026 Investment Climate Statements (10 entries), World Bank trade and
connectivity work (5), Afreximbank, BusinessDay, the CARICOM Secretariat, central banks of
Barbados and Trinidad, ITC, IMF, ITA country guides.

One deliberate correction: **institutions do not post their pain.** Afreximbank, CARICOM,
Kagame, Mottley, Ruto — their timelines are summits and wins. Pain is in budgets, central
bank reports, audit findings and procurement records. X is where we speak, not where we learn.

---

## 2. The five walls. Every group hits the same five.

**Wall 1 — the payment rail is not ours**
- Caribbean banks have lost roughly **4 in 10** correspondent relationships in 15 years.
- Payments still route through US banks; there is no local-currency settlement between
  CARICOM and Africa. The replacement (CAPSS) covers Barbados, The Bahamas and the ECCB
  states, and linking to Africa is explicitly not in the pilot.
- Every African letter of credit must be confirmed by a bank **outside the region** before a
  foreign supplier will accept it.
- Africa runs **42 currencies**; PAPSS is projected to save firms up to **$5bn a year** if
  adopted — the fact a projection is still needed tells you the adoption is not there.

**Wall 2 — trade finance is missing, not expensive**
- Africa's trade finance gap: **$74bn** in 2025. West Africa alone **$14bn**, with **21%**
  of applications rejected; globally **45–67%** of rejections are collateral or applicant risk.
- Bank intermediation fell to **23%** of African merchandise trade (2020–24) from **40%**
  (2011–19), against roughly **80% globally**. Most African trade runs on open account with
  no credit insurance.
- Caribbean: US$1.5bn Afreximbank limit for the region, doubling to $3bn only once all member
  states join. 12 of 15 acceded, **only 9 ratified**.

**Wall 3 — the ocean and the port**
- The two regions are **1,600 miles apart with no direct transport link**.
- Caribbean countries spend **12–21% of the value of imported goods** on transport and insurance.
- Cargo sits roughly **three weeks** in African ports. Lagos runs **over 20 days** dwell.
  South African container terminals averaged **99-hour vessel waits**, with congestion surcharges.
- From port to a landlocked country, **75% of transit time is spent at the port**, not on the road.

**Wall 4 — the state is the counterparty**
- Kenya: **Sh511.75bn** in verified pending bills, up 5.1% year on year.
- Zambia and Ghana: late payment of vendors and VAT refunds "as a budgeting habit".
- Rwanda: a 30-day statutory VAT refund runs months to years in practice.
- Namibia: foreign arbitral awards **cannot be enforced** unless the investor holds a
  Certificate of Status Investment. Senegal: investors route disputes offshore because they
  do not trust local courts against the state.
- Procurement: Côte d'Ivoire is open on paper, opaque in practice; Botswana reserves tenders
  for citizen-owned firms; Nigeria's CAMA s.78 forces a separate local entity before any
  foreign firm can contract.

**Wall 5 — the gate nobody publishes**
- Caribbean SPS approval is the hidden veto on any African food supplier: **no published risk
  assessment** exists for most products, so the shipment simply does not move.
- CARICOM's Secretariat processed **192** Common External Tariff suspension requests — the
  tariff is negotiated one exemption at a time.
- Rum, the Caribbean's flagship branded export, faces an **88% tariff** in African markets.
- CARICOM MFN tariffs average **~13.2%**; bilateral trade between the regions has **never
  surpassed 6%**.

---

## 3. The reframe — and it changes what we sell

The verified pains say the deal does not die because the two sides distrust each other.
It dies because: **nobody will touch the payment, nobody will fund the gap, and nobody will
carry the goods.** Trust is fourth.

So "verified deal room" is right about the *form* — a private room holding one deal — but
too small about the *content*. What the buyer is actually short of is a desk that answers,
for one specific transaction:

1. **Who confirms this letter of credit, and what does it cost?**
2. **Who finances the gap between shipment and payment?**
3. **Who carries it, and what does clearance really take?**
4. **Who are these people, and what happens if it goes wrong?**

We do not build a bank and we do not buy a ship. We assemble the answers, we verify both
counterparties, and we hold the file. Software holds the room, the documents, the checks and
the status. Our network fills the four answers. That is a **per-live-deal** product:
$10–15k to open, $3–5k a month while the deal is live — and the verification dossier can be
sold alone at $10k to a buyer who is not ready for the room.

---

## 4. What we still do not know

1. Which real pair of firms sits in room #1 (a name on each side).
2. Whether the payment rail answer comes from a correspondent bank, a fintech, or PAPSS/CAPSS.
3. Whether a ministry pays per country, per deal, or per year.
4. Whether content sells the problem (my read) or the product.
5. Which single deal we can publish as proof in week one.

---

## 5. Files

- `intel/index.html` — the clickable page (56 verified, 13 hidden unless ticked)
- `intel/pains.db` — SQLite, one row per pain, with quote and source URL
- `intel/raw/*.json` — what each researcher wrote, untouched
- `intel/verified.json` — every entry with its verification note
- `intel/check.py` — the gate: fetch each source, demand the quote, cache the body
- `intel/x/following.json` — 141 accounts you follow
- `intel/x/posts*.jsonl` — 417 posts captured today with URLs
