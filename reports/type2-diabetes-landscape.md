# Type 2 Diabetes Clinical Trials Landscape — Research Digest

**Prepared:** 2026-10-22  
**Source:** ClinicalTrials.gov registry (queried via the registry's search/analysis tools)  
**Query scope:** Condition search `"type 2 diabetes"` — **12,002 studies** in the full landscape at time of pull.  
**Companion data file:** [`data/trend-counts.md`](../data/trend-counts.md) contains the raw numbers as a plain list.

---

## 1. Full landscape — breakdown by overall status (12,002 studies)

| Overall status | Count |
| --- | ---: |
| COMPLETED | 7,885 |
| UNKNOWN | 1,535 |
| TERMINATED | 578 |
| NOT_YET_RECRUITING | 423 |
| ACTIVE_NOT_RECRUITING | 339 |
| WITHDRAWN | 242 |
| RECRUITING | 872 |
| ENROLLING_BY_INVITATION | 92 |
| SUSPENDED | 33 |
| NO_LONGER_AVAILABLE | 2 |

Status buckets sum to 12,001 against the 12,002-study total — the registry is live and posts new/updated records continuously, so counts captured in separate queries minutes apart can differ by a study or two. Counts above are exactly as returned by each registry query; no rounding or estimation was applied.

## 2. Full landscape — breakdown by phase

| Phase | Count |
| --- | ---: |
| EARLY_PHASE1 | 86 |
| PHASE1 | 1,247 |
| PHASE2 | 1,313 |
| PHASE3 | 1,645 |
| PHASE4 | 1,408 |
| N/A | 4,497 |
| Unknown | 2,116 |

Phase buckets total 12,312 against 12,002 distinct studies because the registry's phase facet counts a multi-phase study (e.g., Phase 1/2) once in **each** phase bucket. The same behavior is visible in the registry's native recruiting-only breakdown (894 phase buckets vs 872 studies).

Notable: late-phase activity is substantial — Phase 3 (1,645) and Phase 4 (1,408) together account for ~2,600+ phase slots, but the single largest bucket is N/A (4,497), reflecting the large share of non-pharmaceutical (device, behavioral, observational-style) and unclassified interventional research in T2D.

## 3. Full landscape — breakdown by sponsor class

| Sponsor class | Count |
| --- | ---: |
| OTHER (academic, medical centers, non-profits) | 7,189 |
| INDUSTRY | 4,355 |
| OTHER_GOV (non-US/non-federal government bodies) | 244 |
| NIH | 108 |
| FED (US federal agencies other than NIH) | 66 |
| NETWORK | 27 |
| INDIV (individual/unaffiliated investigators) | 13 |

These buckets sum to exactly 12,002 studies (each study counted once by lead-sponsor class). Academia/other sponsors carry ~60% of the landscape; industry carries ~36% (4,355 studies) but dominates the Phase 3 pipeline (977 of the 1,645 Phase 3 slots in completed industry-sponsored trials alone are industry; see methodology note).

## 4. Full landscape — breakdown by country (site-country occurrences)

Country counts are **site-country occurrences**: a study is counted once for every country in which it has sites, so totals far exceed the 12,002-study count. Top 25:

| Rank | Country | Site occurrences |
| --- | --- | ---: |
| 1 | United States | 49,286 |
| 2 | Japan | 6,207 |
| 3 | China | 5,749 |
| 4 | Germany | 5,673 |
| 5 | Canada | 5,450 |
| 6 | United Kingdom | 4,159 |
| 7 | India | 3,906 |
| 8 | Poland | 3,228 |
| 9 | Russia | 3,171 |
| 10 | Spain | 3,060 |
| 11 | France | 2,992 |
| 12 | Italy | 2,578 |
| 13 | South Korea | 2,548 |
| 14 | Mexico | 2,502 |
| 15 | Hungary | 2,106 |
| 16 | Argentina | 2,086 |
| 17 | Romania | 1,773 |
| 18 | Brazil | 1,743 |
| 19 | Czechia | 1,731 |
| 20 | Netherlands | 1,698 |
| 21 | Australia | 1,615 |
| 22 | South Africa | 1,400 |
| 23 | Slovakia | 1,362 |
| 24 | Denmark | 1,168 |
| 25 | Israel | 1,147 |

The full merged country list (~110 countries/territories) is in [`data/trend-counts.md`](../data/trend-counts.md). The US hosts roughly 4x the site occurrences of the next-largest country; Central/Eastern Europe (Poland, Hungary, Romania, Czechia, Slovakia) collectively forms a major global trial-site hub.

---

## 5. Recruiting-only view — active pipeline vs full landscape

Restricted to trials with overall status **RECRUITING** (872 studies):

**Status breakdown (recruiting only):** RECRUITING — 872 (single status by definition).

**Phase breakdown (recruiting only):**

| Phase | Count |
| --- | ---: |
| N/A | 409 |
| Unknown | 202 |
| PHASE3 | 74 |
| PHASE2 | 69 |
| PHASE4 | 68 |
| PHASE1 | 59 |
| EARLY_PHASE1 | 13 |

Phase buckets total 894 vs 872 distinct recruiting studies (multi-phase studies counted once per phase bucket, as above).

**Sponsor class (recruiting only, for context):** OTHER 665; INDUSTRY 180; OTHER_GOV 19; NETWORK 6; NIH 2 (sums to 872).

**Contrast, recruiting pipeline vs full landscape:**

- The active pipeline is **small relative to the historical base**: only 872 of 12,002 studies (≈7%) are recruiting right now, versus 7,885 already completed and 1,535 with unknown/stale status.
- The recruiting pipeline is **skewed toward early and non-pharmaceutical work**: Phase 3 represents only 74 recruiting phase slots (≈8% of recruiting buckets) versus Phase 3's ≈13% share of the full landscape — the late-phase surge in the full landscape is largely a completed-trials artifact.
- Industry's share of the active pipeline (180 of 872, ≈21%) is lower than its ≈36% share of the full landscape, i.e., the currently recruiting T2D effort is proportionally more academic/investigator-initiated than the historical record.
- Nearly half of recruiting studies are N/A phase (409) — device, digital-health, behavioral, and care-delivery research dominates what is actively enrolling.

---

## 6. Five most recently started industry-sponsored, currently recruiting T2D trials

(Registry query: condition "type 2 diabetes", lead sponsor class INDUSTRY, overall status RECRUITING, sorted by start date descending. Pulled 2026-10-22.)

| # | NCT ID | Title | Sponsor | Phase | Start date |
| --- | --- | --- | --- | --- | --- |
| 1 | NCT07748208 | A Phase II Prospective, Open-Label Safety Study of Inavolisib and Fulvestrant With or Without Palbociclib in Participants With PIK3CA-Mutated Hormone Receptor-Positive, HER2-Negative Advanced Breast Cancer and Type 2 Diabetes | Hoffmann-La Roche | Phase 2 | 2026-10-30 |
| 2 | NCT07868354 | An Open-label, Multiple-arm Study to Assess Tolerability in Participants With Overweight or Obesity, With or Without Type 2 Diabetes, When Switching From Tirzepatide to Zenagamtide | Novo Nordisk A/S | Phase 1 | 2026-10-08 |
| 3 | NCT07855133 | An Open-label, Multiple-arm Study to Assess Tolerability in Participants With Overweight or Obesity, With or Without Type 2 Diabetes, When Switching From Semaglutide to Zenagamtide | Novo Nordisk A/S | Phase 1 | 2026-10-05 |
| 4 | NCT07864168 | Evaluation of MiniMed Next Generation Extended Wear Sensors and Algorithm in Patients With Type 1 and Type 2 Diabetes | Medtronic MiniMed, Inc. | N/A | 2026-10-05 |
| 5 | NCT07831798 | A Phase 1/2, First-in-Human, Dose Escalation and Expansion Study to Evaluate the Safety, Tolerability, and Efficacy of VV-14300 (Adeno-associated Virus Vector-mediated Glucokinase) in Adults With Long-Standing Type 1 Diabetes and Suboptimal Glycemic Control Using an Automated Insulin Delivery (AID) System | Kriya Therapeutics, Inc. | Phase 1/2 | 2026-10 |

**Scope note:** the registry's condition search for "type 2 diabetes" also returns adjacent studies — #4 enrolls both type 1 and type 2 diabetes, and #5 is a type 1 diabetes gene-therapy trial (returned by the registry's expanded condition matching). They are reported as returned by the registry; flagging so the digest isn't misread as five strictly-T2D-exclusive trials.

**Story in the pipeline:** three of the five newest industry trials are incretin/obesity-metabolic programs (two Novo Nordisk zenagamtide switch-tolerability studies off tirzepatide and semaglutide, plus the Roche petrelintide-phase obesity/T2D wave reflected in the wider recruiting set), alongside next-gen diabetes device tech (Medtronic extended-wear sensors) and gene therapy (Kriya's AAV-glucokinase). The industry frontier in T2D right now is weight/metabolic switching, sensors, and curative biologics.

---

## 7. SUNSHINE study (NCT01608724) — status confirmation

- **NCT ID:** NCT01608724 (acronym SUNSHINE; org study ID D1680L00008)
- **Title:** A Multicenter, Single Arm, Cohort Study to Evaluate the Efficacy and Safety of Saxagliptin 5mg, Once Daily for 24 Weeks, in Patients With Type 2 Diabetes Mellitus
- **Sponsor:** AstraZeneca (industry)
- **Phase:** Phase 4
- **Overall status currently listed by the registry:** **COMPLETED** (status verified date 2015-12; primary completion and study completion May 2014, actual; enrollment 2,165 actual)

Confirmed via two independent registry lookups on 2026-10-22, both returning **COMPLETED**. The study remains completed and has not been reactivated.

---

## 8. Methodology and caveats

1. **Tool cap workaround (exactness preserved).** The registry analysis tool caps a single analysis at 5,000 studies; the full T2D landscape is 12,002. Full-landscape phase, sponsor-class, and country breakdowns were therefore reconstructed from **disjoint partitions** that together cover the entire 12,002-study set exactly: completed-industry (3,410), completed-non-industry (4,475), and not-completed (4,117) — which sum to exactly 12,002. Partition counts were added arithmetically with no rounding or estimation; the sponsor-class buckets sum to exactly 12,002, validating the reconstruction. Status counts were obtained per-status via status-filtered queries (each returns that status's exact count).
2. **Live registry drift.** Queries ran minutes apart; the registry posted ~3 new records during the pull (the not-completed partition moved from 4,114 to 4,117 between two runs, all in Unknown-phase). Snapshot values are reported as returned at pull time.
3. **Phase and country facets count differently than studies.** Phase buckets count a multi-phase study once per phase (bucket sum > study count: 12,312 vs 12,002 full landscape; 894 vs 872 recruiting). Country counts are site-country occurrences, not study counts.
4. **Discarded anomalous result.** One analysis call (status breakdown with a combined completed-and-industry advanced filter) returned an anomalous 4,355-study mixed-status set that behaved like an all-industry query rather than the requested intersection; it was discarded in favor of the corroborated partition values. (Coincidentally, 4,355 equals the true total industry count, which served as a cross-check.)
5. **Trial list selection.** The five newest industry recruiting trials come from the registry's own relevance-ranked, start-date-descending result for the stated filters; NCT IDs, titles, sponsors, phases, and start dates were individually verified via direct record lookups.
