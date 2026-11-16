# How to find information in this market

_Tested queries. Includes where search fails, so you do not waste a run on it._

The information we need does not sit on page one of Google. It sits in tender PDFs, in
central bank footnotes, in a Chinese company's own press release, and in the replies under
an official's post. These are the exact queries that reach it. Copy them, change the
country, run them again next week.

---

## 1. Where the money is: government contracts

Procurement is published, just not indexed well. Go at the portal directly, then use Google
to find the PDFs the portals bury.

```
site:gov.ke tenders filetype:pdf
site:*.go.ke "request for proposals" (digital OR software OR "trade facilitation")
site:tenders.go.ke (customs OR payments OR identity OR "data centre")
site:nipc.gov.ng OR site:bpp.gov.ng tender (software OR digital OR consultancy)
site:ppa.gov.gh tenders
site:umucyo.gov.rw (software OR system OR consultancy)
site:etenders.gov.za "request for bid" (software OR artificial intelligence)
site:nptab.org Guyana tender
site:gojep.gov.jm tender
intitle:"invitation to bid" (Kenya OR Ghana OR Rwanda) (system OR platform)
```

Rules that decide whether a foreign firm can even bid — always search these separately,
because they are written in the act, not the tender:

```
site:*.gov "local content" (technology OR services) (Nigeria OR Kenya OR Ghana)
"shall be incorporated in" (Nigeria OR Kenya) "to bid" technology
"CAMA" section 78 foreign company Nigeria
```

---

## 2. What the Chinese are actually doing (their own words first)

Company releases and government announcements beat any analyst piece.

```
site:huawei.com (Africa) (cloud OR "smart city" OR "safe city") press release
site:zte.com.cn Africa (smart city OR government network)
site:transsion.com OR site:tecno-mobile.com Africa strategy
site:alibabacloud.com Africa (customer OR case study)
(Chinese OR China) (AI OR "facial recognition" OR "smart city") (Kenya OR Nigeria OR Ghana OR Uganda) -site:wikipedia.org
"China" "Africa" ("digital silk road" OR "data centre") filetype:pdf
```

On X, the fastest route is the institution, not the keyword:

```
from:huaweienterprise (Africa OR Kenya OR Nigeria)
from:ChinaEmbKenya OR from:ChineseEmbNG (digital OR technology OR AI)
(Chinese OR China) (tender OR contract) (Africa) min_faves:2 filter:links
```

---

## 3. Who is actually shipping product into these markets

App-store charts and launch posts are the truth; press releases are not.

```
site:play.google.com/store/apps (Kenya OR Nigeria) fintech
"top free apps" (Kenya OR Nigeria OR Ghana) 2026
site:restofworld.org (Africa) (Chinese OR India) app
site:techcabal.com (Chinese OR Indian) (startup OR founder OR launches)
(launched OR shipping) ("built in" OR "made in") (Shenzhen OR Bangalore) (Lagos OR Nairobi OR Accra) min_faves:3
site:producthunt.com (Africa OR Nigeria OR Kenya OR Caribbean)
```

Four places to look that most people miss:
1. **App-store country charts** (free, in the browser) — what is actually being downloaded.
2. **Sensor Tower / Appfigures** press citations — downloads by country.
3. **The company's own careers page** — a Chinese firm hiring 20 engineers in Nairobi is a
   bigger signal than any announcement.
4. **Job boards** — `site:brightermonday.co.ke (Chinese OR Mandarin)`.

---

## 4. Payments, correspondent banks and settlement

Central banks publish the pain in their own words.

```
site:centralbank.go.ke ("correspondent" OR "de-risking" OR "payment system") filetype:pdf
site:cbtt.org OR site:centralbank.org.bb ("correspondent" OR "de-risking")
site:bis.org "correspondent banking" (Africa OR Caribbean)
site:imf.org "withdrawal of correspondent banking" country
site:afreximbank.com (PAPSS OR "payment and settlement")
"PAPSS" (volume OR transactions OR countries) 2026
"stablecoin" (Kenya OR Nigeria OR Ghana OR CARICOM) (regulation OR circular)
```

---

## 5. Reddit and X: complaints and vocabulary, never proof

**Tested on 16 Nov 2026 and it failed for discovery.** Three X live searches — government
tenders, correspondent banking, Chinese/Indian developers — returned 3, 6 and 6 results, and
the top hits were an ad for a design agency, a forfeiture notice, and a blog paragraph. X's
search does not index the supply side of this market. Do not send an agent there to find out
what Chinese firms are building; it will come back with noise and call it a finding.

Where X *does* work, and only there:
- **Replies under a known account.** Open the official's post, read the 50 replies. That is
  where the complaint lives.
- **`from:` pulls.** What a specific institution says, in its own words.
- **Announcement sweep.** `("signed an MoU" OR "we are pleased to announce") (Kenya OR Rwanda OR Guyana) min_faves:3`.

Use Reddit and X to learn how people describe the problem — the words they use are the words
that go in a script. Never as a source for a claim.

```
site:reddit.com/r/kenya ("customs" OR "KRA" OR "import") slow OR delay
site:reddit.com/r/Nigeria ("customs" OR "NAFDAC" OR "CBN") delay
site:reddit.com/r/Caribbean ("shipping" OR "freight" OR "bank")
```

**Where discovery actually happens, in order of yield:** procurement portals → company press
releases and case studies → app-store country charts → Rest of World / TechCabal / Semafor
Africa → LinkedIn company pages and job posts (a firm hiring ten engineers in Nairobi is a
louder signal than any announcement) → then Google with `site:` operators. X last.


---

## 6. The rule underneath all of it

Nothing enters the evidence base without a URL a machine can re-open and a quote that is
still there when it does. A search that returns a press-release feeling is worth nothing
until the primary document agrees.

Two things to check on every hit before believing it:
- **Who published it.** The ministry, the company, the central bank, or a journalist quoting
  one of them. Anything else is a lead, not a fact.
- **What year.** Africa analysis travels stale for years; a 2019 number about correspondent
  banking is not today's number. Pin the date and refuse anything undated.
