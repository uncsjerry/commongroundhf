# Site Update Brief — June 12, 2026

**Purpose:** Working instructions for the next terminal session updating commongroundhousingtrust.org. Source material: Fran Esposito's (BPHI CSO) emails of May 26, May 29, June 1–4, and June 12, 2026, plus City of Fort Lauderdale Commission Agenda Memo CAM #26-0409 (June 16, 2026 Conference Meeting). Site last updated April 13, 2026 (commit 8bd4083).

**Internal working document — do not publish or commit to the public repo without review.**

---

## Update 1 — Heritage Crossing / USPS site: appraised value is now $13.5M (filed fact)

The City completed an appraisal of 400 NW 7 Avenue in May 2026: **$13.5 million** (≈ $102/SF on 131,679 SF). This supersedes the site's current figure of "$10M+ ($75–$100/SF), Bob Wojcik, CRA Housing Mgr, Feb 2026."

Source: CAM #26-0409, p. 2 (public record — citable).

**Files / locations to edit:**
- `index.html:1041–1043` — Fair Market Value row in the Heritage Crossing data table → replace with $13.5M, source "City of Fort Lauderdale appraisal, May 2026 (CAM #26-0409)"
- `index.html:1189` — capital stack table, land acquisition note ("$10M+ value contributed")
- `index.html:1281` — CRA/City Contributions row ("Land value ($10M+)")
- `index.html:1368–1369` — "$10M+ in contributed land" headline + subtitle
- `index.html:1381` — return card stat "$10M+"
- `index.html:1389` — pipeline narrative ("$10M+ contributed land asset")
- `index.html:1393` — Year-10 land value projection (re-baseline 3–4% appreciation on $13.5M → ~$18–$20M; verify programmatically)
- `index.html:2241` — competitive comparison table ("$0 land conveyance ($10M+ contributed value)")
- `print.html` and `report.html` — grep for `$10M+` and `Wojcik` and mirror the changes

## Update 2 — Heritage Crossing: City Commission is actively considering the site's future (new section material)

The City Commission takes up the future use of the Alridge Post Office site at its **June 16, 2026 Conference Meeting (CAM #26-0409, District 2)**. New filed facts from the memo:

- USPS notified the City on **October 2, 2025** that it will not renew the lease expiring **December 11, 2027** (confirms existing site date).
- Site is **3.02 acres / 131,679 SF**, zoned NWRAC-MUe.
- CDBG history now documented: ~$1.8M HUD-approved CDBG acquisition (Aug 11, 1994) + ~$1.85M City-funded construction; rental income is CDBG Program Income. Sale proceeds may be treated as CDBG Program Income — HUD inquiry pending.
- Options before the Commission: (a) retain for City use; (b) **convey to a governmental entity such as the CRA or the Housing Authority for affordable housing at or below 80% AMI** (Charter §8.02); (c) declare surplus and sell at ≥75% of appraised value, with 15% of proceeds to the Affordable Housing Trust Fund (§8.04); (d) competitive solicitation/RFP under **F.S. §255.065** (§8.09).

**Files / locations to edit:**
- `index.html` Heritage Crossing data table (~line 1030–1060) — add rows: "City Commission consideration: June 16, 2026 (CAM #26-0409)"; "CDBG Program Income status: HUD inquiry pending"
- `index.html:1389` — pipeline narrative: the conveyance-to-CRA pathway is now explicitly on the Commission's published options list; F.S. 255.065 solicitation is the competitive alternative. Frame as "Key Insight" callout in site voice.
- Note the alignment: the site's CLT/affordable model fits both the CDBG national objective (low/mod-income benefit) and the §8.02 conveyance pathway — this is the strategic argument; label as analysis, not filed fact.
- Asset to add: `assets/` — Commission Agenda Memo 26-0409.pdf and Exhibit 1 - USPS Site Presentation.pdf (both attached to Fran's 6/12 email; save into assets/ before linking)

## Update 3 — Aspire 1650: timeline has moved — Q3 2026 closing is stale

Because of Broward County permitting delays (drainage, building), on **May 18, 2026** a Petition for Waiver of Rule 67-48.002(96) and the 2024 QAP was filed to move the 2025 Housing Tax Credit award into **2027**. The 10% compliance test date of 7/31/26 could not be met. FHFC staff suggested revisions (all positive); response filed by June 3 deadline; item goes to the **FHFC Board on June 26, 2026 on the Consent Agenda with a positive staff recommendation**. Fee to effectuate: ~$200K (paid by Green Mills). Petitioner: Aspire 1650, Ltd.

Also: all building and civil permits have been submitted (KEITH processing); Pirtle will hold the master building permit.

Source: Fran's emails 5/26, 5/29, 6/1–6/4/2026 (FHFC filing 2025-362CSA is public record).

**Files / locations to edit (hold until after the June 26 FHFC board vote, then update in one pass):**
- `index.html:677` — section subtitle ("Financial closing and groundbreaking targeted Q3 2026")
- `index.html:710–713` — milestone table (GC Bids / Financial Closing Q3 2026 / CO Q4 2027) → re-baseline to the 2027 credit year once FHFC confirms
- `index.html:733` — pro forma subtitle ("Construction targeted Q3 2026")
- `index.html:816` — source/disclaimer paragraph — add the waiver petition and FHFC board action date
- `index.html:2319` — precedent table row ("FHFC pipeline — construction Q3 2026")
- `report.html` / `print.html` — mirror

## Update 4 — State budget FY2026/27 (supporting facts, smaller edits)

- **Sadowski funds fully funded** — Aspire 1650's state capital stack layer is intact. (Positive proof point for the "state" layer of the capital stack section.)
- **$38M+ in Special Member Projects** general revenue — precedent: Chip LaMarca's $250K for the 7 on 7th workforce lab (2023). BPHI considering a member-project ask in the FY27/28 session (3/2/27–4/30/27). Forward-pipeline talking point.
- Property tax reform (special session 6/1–6/3) could bar local property-tax funding of affordable housing unless classified as "infrastructure" — watch item; veto power runs to 6/30/26.

Source: Fran's 5/29 email + Florida Housing Coalition final budget deck (attached to that email).

**Files / locations:** capital stack section of `index.html` (state layer) — one or two sentence update; optionally a "Legislative watch" callout. Label projections vs. fact.

---

## Terminal session checklist

1. `git pull`, branch `update/june-2026-fran`
2. Make Update 1 + 2 edits (public record now — citable immediately)
3. Hold Update 3 until 6/26 FHFC board action, or publish with "pending FHFC board approval 6/26/26" labeling — Jerry to decide
4. Verify all recomputed dollar figures programmatically (no eye math)
5. Cross-check `index.html`, `print.html`, `report.html`, `six-pillars-alignment.html` for every instance of `$10M+`, `Q3 2026`, `Wojcik`
6. Commit, deploy, document

One inconsistency to resolve while in there: the hero (line ~109) says Heritage Crossing "~300 units" while the precedent table (line 2319 area) and the April commit say **353 units** — standardize on 353.
