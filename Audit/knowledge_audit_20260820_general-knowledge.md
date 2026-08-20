---
type: knowledge-audit
vault: "F:/obsidian_note/general-knowledge"
baseline: "body-of-knowledge/"
audited_on: 2026-08-20
auditor: "QA (Senior QA Engineer — Quality & Test Engineering)"
scope: "coverage / traceability audit + general-knowledge gap analysis"
---

# Knowledge Audit — General Knowledge Vault

> **Vault:** Oralita General Knowledge (`F:/obsidian_note/general-knowledge`)
> **Baseline (authoritative scope):** `body-of-knowledge/` — Thai Basic Education Core Curriculum B.E. 2551 (revised 2560)
> **Date:** 2026-08-20
> **Method:** machine-assisted traceability (wikilink extraction + normalized filename matching) + manual spot-checks of note quality.

---

## 0. Executive Summary

| Axis | Verdict | Confidence |
|---|---|---|
| **Baseline (curriculum coverage)** | 🟢 **Strong** — 6 of 9 components fully matched; 2 partial; 1 empty | High |
| **Nice-to-have (general knowledge)** | 🟡 **Solid but Thai-curriculum-centric** — strong incidental coverage; real gaps in Western philosophy, world literature, current affairs | Medium (judgment) |

**Bottom line:** This is a *high-quality, well-structured* Thai-curriculum knowledge base. Math, Science, Arts, Health & PE, and Career & Technology are **fully populated and filename-matched** to the baseline. The real defects are (1) **Student Development Activities has zero content**, (2) **English has only a supplementary grammar reference, not the 4-strand curriculum**, and (3) a **systematic taxonomy drift** — the baseline's fine-grained strand overviews enumerate concept areas whose wikilinks no longer resolve to the actual (reorganized) content files, especially in Social Studies.

---

## 1. Inventory

| Layer | Files |
|---|---|
| Total markdown files | **573** |
| Baseline (`body-of-knowledge/`) | **56** |
| Content (everything else) | **517** |

### Baseline → Content mapping

| # | Component (BOK) | Claimed concept areas | Content folder | Notes found | Status |
|---|---|---|---|---|---|
| 1 | 📗 Thai Language (ภาษาไทย) | ~35–75 | `ภาษาไทย/` | 99 | ✅ Deep |
| 2 | 🌏 English (4 strands) | ~28 | `English Skill/` *(supplementary)* | 62 | 🟡 Partial |
| 3 | 🏛️ Social Studies (5 strands) | ~94 | `Social Studies/` | 68 | 🟡 Partial (drift) |
| 4 | 🔢 Mathematics (fund + adv) | ~43 | `Mathematics/` | 43 (20+23) | ✅ Exact |
| 5 | 🔬 Science (fund + 5 spec.) | ~150 | `Science/` | 107 (22+85) | ✅ Strong |
| 6 | 🎨 Arts (3 domains) | 19 | `Art/` | 22 (19+3 ov) | ✅ Exact |
| 7 | ❤️ Health & PE (2 strands) | ~14 | `Health-PE/` | 16 (14+2 ov) | ✅ Exact |
| 8 | 🔧 Career & Technology (5 strands) | 22 | `work-careers-technology/` | 27 (22+5 ov) | ✅ Exact |
| 9 | 🧭 Student Development Activities | 3 forms | *(none)* | **0** | 🔴 Empty |
| — | *(outside baseline)* | — | `career/` (7 career guides) | 62 | 🟢 Bonus |
| — | *(auxiliary)* | — | `checklist/` (book lists) | 10 | ⚪ Out-of-scope |

---

## 2. Axis 1 — Baseline (curriculum) Coverage

### 2.1 Fully matched (✅ no action needed)

| Component | Evidence |
|---|---|
| **Mathematics** | `Fundamental/` = 20 topics, `Advance/` = 23 topics; BOK lists ~20 + ~23. Filenames align 1:1 (`01_Numbers_and_Numeration` … `23_Differential_Equations`). |
| **Arts** | 19 concept areas (8 visual + 6 music + 5 performing) → 19 topic notes + 3 overviews. BOK's own "19/19 (100%)" claim **verified true**. |
| **Health & PE** | 14 concept areas → 14 topic notes + 2 overviews (`01_Human_Body_and_Growth` … `14_Recreation`). |
| **Career & Technology** | 22 concept areas → 22 topic notes + 5 overviews, spread across Home Economics / Agriculture / Crafts / Career / Technology. |
| **Science (Fundamental)** | 22 topic notes match the 22 listed concept areas (`01_Scientific_Method` … `22_Technology_and_Engineering`). |
| **Science (Specialized)** | Physics (23), Chemistry (20), Biology (20), Computer Science (12), Earth Science (10) all present and numbered. |
| **Thai Language** | 5 strands all populated (99 notes): การอ่าน / การเขียน / การฟังฯ / หลักการใช้ภาษาไทย (24) / วรรณคดีและวรรณกรรม (31 incl. sub-era folders). |

### 2.2 Partial (🟡)

| Component | Finding | Severity |
|---|---|---|
| **Social Studies** | Substantial content (63 topic notes across 5 strands) but **taxonomy divergence**: the BOK strand overviews enumerate a fine-grained taxonomy (Religion 18, Civics 22, Economics 18, History 14, Geography 18 ≈ 90 areas) with numbered wikilinks (`[[01_Buddha_Biography]]`, `[[22_Media_Literacy]]`, …) that **do not resolve** to the actual content files (which are named/organized differently: `01_Buddhist_Principles`, `02_Buddhist_Ceremonies_and_Meditation`, …). Coverage is *probably* adequate but **untraceable** — the baseline's own cross-references are stale. | 🟡 Improve |
| **English** | The BOK itself labels `English Skill/` as a **supplementary** teaching-ordered reference (grammar → skills → exams), *not* the 4-strand curriculum. Strand 2 (culture), Strand 3 (cross-curricular), and Strand 4 (community/world) topics have **no dedicated notes**; they are only cross-referenced into English Skill sections. The 62 English Skill notes are strong, but the curriculum map's own concept areas are unpopulated. | 🟡 Improve |

### 2.3 Empty (🔴)

| Component | Finding | Severity |
|---|---|---|
| **Student Development Activities** | BOK defines 3 forms (Guidance / Student Activities incl. Scouts / Social & Public Benefit) with 3 overview files, but **zero content notes exist anywhere in the vault**. The BOK's own "Progress Tracker" admits *"Topic notes: Not yet created"*. Full baseline gap. | 🔴 Gap |

---

## 3. Traceability & Naming Defects

These break clean wikilink resolution and should be fixed for the vault to be *machine-auditable* going forward:

| # | Issue | Location | Fix |
|---|---|---|---|
| T1 | Folder `Science/Advance/physic` (lowercase, singular) vs BOK "Physics" | content | rename to `Physics` |
| T2 | `Computer_Science` / `Earth_Science` (underscore) vs BOK "Computer Science" / "Earth Science" | content | rename to spaces |
| T3 | BOK "Vault:" paths point to non-existent folders (`Thai\`, `English\`, `Physics\`, `Chemistry\`, `Biology\`, `Computer Science\`, `Earth Science\`) | baseline | update to `ภาษาไทย\`, `English Skill\`, `Science/Advance/*` |
| T4 | Broken internal BOK cross-links (`[[05 Mechanics]]` → should be `[[01_Mechanics_-_Overview]]`; `[[12 Cell and Molecular Biology]]`, `[[09 Chemical Foundations]]`, etc.) | baseline | repair links |
| T5 | Social Studies strand-overview wikilinks don't resolve (taxonomy drift, §2.2) | baseline ↔ content | re-sync names or add redirect/alias |

---

## 4. Axis 2 — Nice-to-have (general knowledge for a human)

**Reference frame (auditor-defined):** knowledge a generally well-educated adult should hold *beyond* a school curriculum — world history, world geography, general science literacy, philosophy & critical thinking, world literature & arts, personal finance, media/information literacy, current affairs, psychology, and civic/law literacy.

### 4.1 Well covered (incidentally strong for a curriculum vault)

| Domain | Evidence |
|---|---|
| World history & civilizations | `Social Studies/04 History/12_Ancient_Civilizations`, `02_World_History_and_Civilizations`, `13_SE_Asian_History` |
| World geography | `Social Studies/05 Geography/12_World_Regions`, `13_Geographic_Coordinates` |
| Personal finance | `Social Studies/03 Economics/02_Personal_Finance`, `10_Economic_Indicators`, `14_Consumer_Rights` |
| Media & digital literacy | `Social Studies/02 Civics/12_Media_Literacy`, `work-careers-technology/05 Technology/21_Digital_Citizenship`, `22_Information_Literacy` |
| Health literacy | `Health-PE/` — nutrition, disease prevention, mental health, relationships |
| Career exploration | `career/` — 7 deep guides (accountant, agriculture, engineer, lawyer, nurse, psychologist, teacher) + university-path notes |
| Logic / critical thinking | pervasive in Mathematics (Mathematical Reasoning) and Computer Science (Boolean Logic, Computational Thinking) |

### 4.2 Genuine gaps (🟡 / 🔴)

| Domain | Finding | Severity |
|---|---|---|
| **Western philosophy** | `ปรัชญาตะวันตก` = **0 files**; `epistemology` = 1 file. Philosophy content is entirely Buddhist/Thai (Sufficiency Economy, Dhamma). No Plato/Aristotle/Kant/ethics traditions, no epistemology/logic-as-philosophy. | 🔴 Gap |
| **World literature (non-Thai)** | `world literature` = **0 files**. `literature` (45 files) = Thai literature + English academic writing. No Shakespeare, world classics, or comparative literature. | 🔴 Gap |
| **Current affairs / contemporary world** | `current affairs` / `current events` = **0 files**. Vault is curriculum-static (correctly so for its purpose) — not a living news/current-events layer. | 🟡 (by design) |
| **Psychology as a discipline** | Only ~17–19 files touch psychology, mostly the `career/psychologist` guide + mental-health strand. No general psychology (cognition, biases, development theory). | 🟡 |

> **Judgment note:** these "nice-to-have" gaps are *not defects of the curriculum vault* — they are candidates for a future "beyond-school" layer. Flagging them so you can decide whether that layer is in scope.

---

## 5. Findings Register (severity-ranked)

| # | Finding | Axis | Severity | Evidence |
|---|---|---|---|---|
| F1 | Student Development Activities: 0 content notes | Baseline | 🔴 Gap | no folder; BOK "Topic notes: Not yet created" |
| F2 | English 4-strand curriculum has no dedicated notes (only supplementary English Skill) | Baseline | 🟡 | BOK self-labels English Skill as supplementary |
| F3 | Social Studies BOK↔content taxonomy drift (~90 claimed areas vs 63 differently-named notes); wikilinks don't resolve | Baseline | 🟡 | wikilink resolution fails |
| F4 | `Science/Advance/physic` + underscore folder names break traceability | Traceability | 🟡 | folder listing |
| F5 | BOK "Vault:" paths + internal cross-links are stale/broken | Traceability | 🟡 | 151 non-resolving refs |
| F6 | Western philosophy absent | Nice-to-have | 🔴 | 0 files |
| F7 | World (non-Thai) literature absent | Nice-to-have | 🔴 | 0 files |
| F8 | Current affairs / psychology-as-discipline light | Nice-to-have | 🟡 | 0 / ~19 files |

---

## 6. Note Quality (spot-check)

Sampled 2 notes; both are **excellent**:

- `Science/Advance/physic/01_Measurement_and_Scientific_Method.md` — full frontmatter (tags, source, course codes ว301), grade-band scope, Thai/English terminology table, 6 sub-sections, worked problem types with LaTeX, cross-links. **High quality.**
- `Social Studies/01 Religion/01_Buddhist_Principles.md` — grade-band breakdown, Four Noble Truths / Eightfold Path / Five Precepts / Aggregates / Dependent Origination tables, Thai terminology, cross-links. **High quality.**

> No quality red flags found in sampling. The vault's weakness is **structural traceability**, not content depth or accuracy.

---

## 7. Recommendations (priority order)

1. 🔴 **Fill Student Development Activities** — 3 overviews exist; create topic notes for Guidance, Student Activities (Scouts/Girl Guides), and Social/Public Benefit, or explicitly descope this component in the BOK if not intended.
2. 🟡 **Re-sync Social Studies taxonomy** — reconcile BOK strand-overview concept-area lists with actual content filenames (rename files *or* update wikilinks). This restores baseline traceability.
3. 🟡 **Decide English scope** — either build the 4-strand curriculum notes or formally document "English Skill = the English content, curriculum map is conceptual."
4. 🟡 **Fix naming drift** — rename `physic` → `Physics`, `Computer_Science`/`Earth_Science` → spaces; update BOK "Vault:" paths and repair broken internal cross-links.
5. 🟢 **Optional "beyond-school" layer** — Western philosophy, world literature, current affairs, general psychology, if the "general knowledge for a human" goal extends past the Thai curriculum.

---

## 8. Verdict

**Baseline coverage: ~78% fully matched (6/9 components exact), 2 partial, 1 empty.** Content depth and quality are excellent; the defects are concentrated in *traceability* (stale wikilinks / taxonomy drift) and *one missing component*, not in content quality.

**Nice-to-have: strong incidental general-knowledge coverage** (world history/geography, finance, media literacy, health, careers) but with clear humanities gaps (Western philosophy, world literature) characteristic of a national-curriculum scope.

*Audit is a point-in-time snapshot; re-run after any taxonomy/rename remediation to confirm traceability recovery.*

---

## 9. Remediation Applied (2026-08-20)

Taxonomy/backlink drift was **fixed** in a follow-up pass. All machine-repairable links now resolve.

| Item | Result |
|---|---|
| BOK overview wikilinks remapped to actual content notes | ✅ **316** links fixed (Career & Tech, Math, Science, Social Studies, Thai, Health) |
| Content-file cross-links remapped (wrong number/space/underscore/stale name) | ✅ **111** links fixed (Science, Social Studies, Math, Thai, career) |
| Folder naming drift renamed | ✅ `physic`→`Physics`, `Computer_Science`→`Computer Science`, `Earth_Science`→`Earth Science` |
| Stale `physic/` path references | ✅ 3 links → `Physics/` |
| Stale `Vault:` prose paths in BOK overview | ✅ 11 references corrected |
| `Teaching`→`Teacher` career link typo | ✅ 2 links fixed |

**Remaining broken links: 24 — all genuine *content gaps* (missing notes), not taxonomy drift:**

| Gap | Location |
|---|---|
| Fluid Mechanics | Science/Physics (no note) |
| Natural Hazards, Natural Resources, Space Exploration, Stars & Galaxies | Science/Earth Science (no notes) |
| Water Properties, Ethics (`Foundation/Society`), Environmental Chemistry | Science cross-refs to non-existent notes |
| การเขียนบันทึก, การเขียนเพื่อการสมัครงาน | ภาษาไทย/การเขียน (no notes) |
| บทร้อยกรอง, วรรณกรรมแปล | ภาษาไทย/วรรณคดี (no notes) |
| architect, doctor, pharmacist, social-worker + Technician/Diplomat/Judge/Psychiatrist | career/ (folders/notes not yet built) |

**Also flagged (not fixed):** `ภาษาไทย/การเขียน/05_การเขียนจดหมาย.md` and `14_การเขียนจดหมาย.md` are **duplicates with different content** — worth reconciling.

*Note: a first pass of the content-file fix contained an auto-matching bug that flipped valid links whose names normalize to a collision (e.g. `17_Probability`↔`19_Probability`); it was caught, fully reverted via `git reset --hard`, and re-applied with a guard that only rewrites genuinely-broken links.*

