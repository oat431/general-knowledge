---
type: topic-proposal
vault: "F:/obsidian_note/general-knowledge"
drafted_on: 2026-09-05
author: "Edu (Educator) with user decisions via /grill-me"
scope: "beyond-curriculum general knowledge layer (humanities core) + baseline debt closure"
status: draft-for-review
---

# More Topics Proposal — General Knowledge Vault (2026-09-05)

> **What this is:** The curriculum baseline (8 learning areas + Learner Development Activities) is complete and machine-auditable. This proposal defines what comes *next*: a beyond-curriculum "general knowledge for an educated adult" layer, plus closure of the small baseline debts found by the link checker on 2026-09-05.
> **How it was made:** structured grill-me interview (10 decisions locked with the user), vault-wide wikilink scan (3,668 links checked), and review of the 2026-08-20 + 2026-08-28 audits.

---

## 1. Locked Decisions (grill synthesis)

| # | Question | Decision |
|---|---|---|
| 1 | Audience and purpose | Adult / family lifelong reference: exam-free, what an educated adult should know |
| 2 | Domain scope | **Humanities core only**: philosophy, world literature, world religions and mythology |
| 3 | Language | **Per topic, decided by the user** (suggestions pre-filled in §5-7, editable) |
| 4 | Depth | Adult general knowledge: readable, concepts + context + sources, no exam framing |
| 5 | Placement | Both: a new root **and** deepening existing subjects where natural |
| 6 | Root structure | `General Knowledge/` umbrella with numbered folders: 01 Philosophy, 02 World Literature, 03 World Religions and Mythology (room for future clusters) |
| 7 | Sequencing | One domain at a time: Philosophy first (audit's #1 🔴 gap), then World Literature, then Religions and Mythology |
| 8 | Book pipeline | Full pipeline: book checklists into `checklist/`, summaries into `Book/` by the book-summarizer profile, notes informed by them |
| 9 | Baseline debts | **Phase 0 of this proposal**: close missing notes + broken links + duplicates + N1 before new topics |
| 10 | BOK integration | Amended 2026-09-05: BOK drafts now live in `body-of-knowledge/General Knowledge/` (index + 3 domain overviews); the curriculum BOK subjects stay untouched |

---

## 2. Why These Topics

- The 2026-08-20 audit flagged the beyond-curriculum axis: **Western philosophy 🔴 (0 files), world literature 🔴 (0 files)**, psychology 🟡, current affairs 🟡. Humanities core closes the two red gaps plus the religions/mythology neighbor the Religion strand already gestures at.
- `Book/Sapiens` already points this direction: the vault's only non-curriculum book summary.
- Curriculum coverage is *finished*; growth must come from outside the 2551/2560 baseline without polluting its machine-auditability.

---

## 3. Phase 0 — Baseline Hygiene (do first)

Evidence: vault-wide wikilink scan, 2026-09-05: 3,668 links, 119 broken targets.

### 3.1 Genuinely missing notes: 20 (create)

| # | Area | Missing note | Evidence |
|---|---|---|---|
| 1 | Science/Physics | Fluid Mechanics | BOK `02_Thermodynamics_and_Waves_-_Overview` links it |
| 2 | Science/Earth Science | Natural Hazards | BOK `02_Astronomy_and_Environment_-_Overview` |
| 3 | Science/Earth Science | Natural Resources | same |
| 4 | Science/Earth Science | Space Exploration | same |
| 5 | Science/Earth Science | Stars and Galaxies | same |
| 6 | Science/Chemistry | Environmental Chemistry | linked from Earth Science `10_Climate_Change_and_Environment` |
| 7 | Science/Biology | Water Properties | linked from Chemistry `04_Intermolecular_Forces` |
| 8 | Science (CS cross-ref) | Ethics (society and technology) | linked from CS `12_Digital_Citizenship` |
| 9 | ภาษาไทย/การเขียน | การเขียนบันทึก | BOK การเขียน overview |
| 10 | ภาษาไทย/การเขียน | การเขียนเพื่อการสมัครงาน | BOK การเขียน overview |
| 11 | ภาษาไทย/วรรณคดี | บทร้อยกรอง | BOK วรรณคดี overview |
| 12 | ภาษาไทย/วรรณคดี | วรรณกรรมแปล | BOK วรรณคดี overview (doubles as the World Literature bridge, §9) |
| 13 | career/ | architect | linked from career/engineer |
| 14 | career/ | doctor | linked from career/nurse |
| 15 | career/ | pharmacist | linked from career/nurse |
| 16 | career/ | social worker | linked from career/psychologist |
| 17 | career/ | technician | linked from career/engineer |
| 18 | career/ | diplomat | linked from career/lawyer |
| 19 | career/ | judge / prosecutor | linked from career/lawyer |
| 20 | career/ | psychiatrist | linked from career/psychologist |

**Fix:** create notes following each area's existing pattern (career guides reuse the 7 existing guide templates).

### 3.2 Broken links: ~92 (rewrite targets, no new content)

All targets' basenames exist elsewhere in the vault; the path part is stale. Classes:

| Class | Count | Pattern | Fix |
|---|---|---|---|
| `Fundamental/` stale paths | ~34 | `[[Fundamental/NN_Topic]]` from Mathematics/Advance, BOK Science overview, Physics notes (leftover from the Fundamental/Advance reorganization) | bare basename `[[NN_Topic]]` (unique) or correct relative path |
| Strand-folder-prefixed overview links | ~21 | `[[01 Religion/00_overview]]`, `[[02 Civics/06_Government_Structure]]`, etc. written from sibling strand folders | correct relative path `[[../01 Religion/00_overview]]` |
| BOK cross-overview links from Student Development | ~4 | `[[../../Arts/Arts - Overview]]` etc. | correct path or bare filename |
| BOK Science overview links from Career and Technology | ~3 | `[[Science/03_Biology - Overview]]` | `[[../Science/03_Biology - Overview]]` or bare |
| career → BOK links | ~2 | `[[body-of-knowledge/Science/04_Human_Body_Systems]]` | link to content note `[[04_Human_Body_Systems]]` |
| Thai path links | ~27 | `[[หลักการใช้ภาษาไทย/01_อักษรไทย]]` from วรรณคดี folders, `[[การอ่าน/00_ภาพรวม]]` (wrong target name), `[[สมัยอยุธยา/00_overview]]`, etc. | correct relative path or correct filename |

**Fix:** scripted rewrite with the guard used in the 2026-08-20 remediation (only rewrite genuinely broken links; verify with the link checker). The exact per-link list is reproducible from the checker output.

### 3.3 Other baseline items

| Item | Action |
|---|---|
| Duplicate `ภาษาไทย/การเขียน/05_การเขียนจดหมาย.md` vs `14_การเขียนจดหมาย.md` (different content) | reconcile into one note |
| Finding N1 (audit 2026-08-28): 15 Progress-Tracker paths in the 3 Student Development BOK sub-overviews + main overview are inline-code paths, not wikilinks | convert to wikilinks |

### 3.4 Phase 0 acceptance criteria

- Link checker reports **0 broken targets outside `Audit/`** (7 audit-doc links are evidence quotes, expected to stay broken).
- All 20 missing notes exist with content.
- Duplicate pair reconciled; N1 converted.

---

## 4. New Layer Structure

```
General Knowledge/                        ← new top-level root
├── 00_Overview.md                        ← index: 3 domains, reading paths, cross-link map
├── 01 Philosophy/
│   ├── 00_overview.md                    ← roadmap + progress tracker (01-20)
│   ├── 01_What_Is_Philosophy.md
│   └── ... (20 notes)
├── 02 World Literature/
│   ├── 00_overview.md
│   └── ... (20 notes)
└── 03 World Religions and Mythology/
    ├── 00_overview.md
    └── ... (20 notes: 11 religions + 9 mythology)
```

### Note template (adult general knowledge, 8-15 KB)

```yaml
---
tags: [general-knowledge, philosophy]   # domain tag per folder
source: "primary books + references"
created: YYYY-MM-DD
---
```

Body: What is this + why it matters → core concepts (tables) → timeline (Mermaid) → key ideas per thinker/tradition → Thai terminology table → "Why it matters today" (adult relevance, 2-3 examples) → further reading → cross-links. Colons, not em-dashes. Mermaid over ASCII. English narrative with Thai terms in parentheses unless the user marks the topic as Thai.

### BOK policy

`body-of-knowledge/General Knowledge/` holds this layer's BOK: the `General Knowledge - Overview.md` index plus one domain overview per folder (Philosophy, World Literature, World Religions and Mythology), created 2026-09-05. The curriculum BOK subjects themselves stay untouched, so future audits keep the curriculum baseline clean. The content root `General Knowledge/` gets `00_overview.md` progress trackers as content notes are built.

---

## 5. Domain 01 — Philosophy (~20 notes)

Build order = table order (chronological). **Language column = suggestion; user overrides per topic.**

| # | File | Covers | Language | Key books | Cross-links |
|---|---|---|---|---|---|
| 01 | What Is Philosophy | branches: metaphysics, epistemology, ethics, logic, aesthetics, political philosophy | EN + TH | Warburton: A Little History of Philosophy | [[Mathematical_Reasoning]] if present; CS [[12_Digital_Citizenship]] |
| 02 | Pre-Socratic Philosophers | Thales, Heraclitus, Parmenides, atomists | EN + TH | Durant: Story of Philosophy | Science [[01_Scientific_Method]] |
| 03 | Socrates and the Socratic Method | questioning, examined life, trial | EN + TH | Plato: Apology | หลักการใช้ภาษาไทย การโต้แย้ง; English Skill debate notes |
| 04 | Plato | Theory of Forms, The Republic, cave | EN + TH | The Republic (trans.) | Civics [[06_Government_Structure]] |
| 05 | Aristotle | logic, virtue ethics, politics, science legacy | EN + TH | Nicomachean Ethics | Science [[01_Scientific_Method]] |
| 06 | Hellenistic Philosophy | Stoicism, Epicureanism, Skepticism | EN + TH | Marcus Aurelius: Meditations | Economics Sufficiency Economy ↔ Stoic parallels |
| 07 | Medieval Philosophy | Augustine, Aquinas, scholasticism | EN + TH | Kenny or Copleston excerpts | Religion strand [[01_Buddhist_Principles]] (comparative) |
| 08 | Islamic and Jewish Philosophy | Al-Farabi, Avicenna, Averroes, Maimonides | EN + TH | Fakhry: History of Islamic Philosophy | Religion strand other-religions notes |
| 09 | Renaissance and Humanism | Machiavelli, Erasmus, Montaigne | EN + TH | The Prince | History strand world civilizations |
| 10 | Rationalism | Descartes, Spinoza, Leibniz | EN + TH | Descartes: Meditations | Mathematics logic notes |
| 11 | Empiricism | Locke, Berkeley, Hume | EN + TH | Hume excerpts | Science [[01_Scientific_Method]] |
| 12 | Enlightenment and Social Contract | Hobbes, Locke, Rousseau, Voltaire, Montesquieu | EN + TH | Rousseau: Social Contract | Civics democracy notes |
| 13 | Kant and German Idealism | Critique of Pure Reason, categorical imperative, Hegel | EN + TH | Warburton chapters | Ethics theme across Religion strand |
| 14 | Utilitarianism and Ethical Theories | Bentham, Mill; deontology vs consequentialism vs virtue | EN + TH | Mill: On Liberty | Religion strand moral reasoning |
| 15 | Existentialism | Kierkegaard, Nietzsche, Sartre, Camus, Beauvoir | EN + TH | Sartre: Existentialism Is a Humanism | World Literature [[The Stranger]] note |
| 16 | Pragmatism | Peirce, James, Dewey | EN + TH | James excerpts | CS computational thinking |
| 17 | Analytic Philosophy | Frege, Russell, Wittgenstein, Popper | EN + TH | Russell: Problems of Philosophy | CS [[07_Data_Structures]] logic context |
| 18 | Political Philosophy and Justice | Marx, Rawls, Nozick, Berlin | EN + TH | Rawls excerpts | Economics [[10_Economic_Indicators]] |
| 19 | Philosophy of Science | induction, falsification, Kuhn paradigms | EN + TH | Popper excerpts | Science [[01_Scientific_Method]] |
| 20 | Eastern Philosophy Beyond Thailand | Confucianism, Daoism, Zen, Vedanta, Indian logic | EN + TH | Tao Te Ching, Confucius: Analects | Religion strand Buddhism notes (contrast) |
| 21* | Philosophy of Mind and AI | consciousness, Turing, Chinese Room | EN + TH | Hofstadter excerpts | CS AI notes |
| 22* | Applied Ethics Today | bioethics, tech ethics, climate ethics, Stoic revival | EN + TH | Sandel: Justice | Health-PE, work-careers-technology technology strand |

`*` = optional; trim if the build feels long.

---

## 6. Domain 02 — World Literature (~20 notes)

| # | File | Covers | Language | Key books | Cross-links |
|---|---|---|---|---|---|
| 01 | How to Read Literature | plot, character, theme, style; why stories matter | EN + TH | Bauer: The Well-Educated Mind | ภาษาไทย การวิเคราะห์วรรณคดี notes |
| 02 | Ancient Epics | Gilgamesh, Iliad, Odyssey | EN + TH | translations | ภาษาไทย วรรณคดี comparisons |
| 03 | Greek Drama | Sophocles Oedipus Rex, Euripides, Aristophanes | EN + TH | translations | Performing Arts notes (Art folder) |
| 04 | Roman Literature | Virgil Aeneid, Ovid Metamorphoses | EN + TH | translations | Greek mythology notes (§7) |
| 05 | Dante and the Medieval World | Divine Comedy, Chaucer | EN + TH | translations | World Religions (medieval Christian world) |
| 06 | Shakespeare | Hamlet, Macbeth, sonnets | EN + TH | plays | English Skill reading notes |
| 07 | Cervantes and the Early Novel | Don Quixote | EN + TH | translation | |
| 08 | Enlightenment Literature | Voltaire Candide, Swift, Defoe | EN + TH | translations | Philosophy 12 Enlightenment |
| 09 | Goethe and German Literature | Faust, Werther | EN + TH | translations | Philosophy 13 (Goethe's era) |
| 10 | Russian Literature | Tolstoy, Dostoevsky, Chekhov | EN + TH | translations | |
| 11 | French 19th Century | Hugo Les Misérables, Balzac, Flaubert | EN + TH | translations | musical/ song notes already in oralita_md (Les Mis) |
| 12 | English 19th Century | Austen, Dickens, Brontës | EN + TH | translations | English Skill |
| 13 | American Classics | Melville, Twain, Poe; Fitzgerald, Hemingway, Steinbeck | EN + TH | translations | |
| 14 | Modernism | Kafka, Joyce, Woolf, Eliot | EN + TH | translations | |
| 15 | Dystopian Fiction | Orwell 1984, Huxley, Bradbury, Golding | EN + TH | translations | Civics [[12_Media_Literacy]] |
| 16 | Magical Realism and Latin America | García Márquez, Borges, Allende | EN + TH | translations | |
| 17 | Asian Literature | Murakami, Kawabata, Tagore, Mo Yan, Bashō haiku | EN + TH | translations | ภาษาไทย วรรณกรรมไทย (neighbor) |
| 18 | African and Middle Eastern Literature | Achebe, Mahfouz, Adichie, Gibran | EN + TH | translations | |
| 19 | Poetry of the World | Rumi, Neruda, Whitman, Dickinson, Baudelaire | EN + TH | anthologies | ภาษาไทย ฉันทลักษณ์ (poetic forms contrast) |
| 20 | Children's Classics and Folk Tales | Aesop, Grimm, Andersen, Arabian Nights | EN + TH | collections | ภาษาไทย นิทานและตำนาน |
| 21* | ASEAN and Southeast Asian Literature | neighbors beyond Thailand | EN + TH | anthologies | History strand SE Asian history |
| 22* | Literary Movements Overview | Romanticism → Realism → Modernism → Postmodernism | EN + TH | Sutherland: A Little History of Literature | (could be the 00_overview roadmap instead) |

---

## 7. Domain 03 — World Religions and Mythology (20 notes: 11 religions + 9 mythology)

| # | File | Covers | Language | Key books | Cross-links |
|---|---|---|---|---|---|
| 01 | What Is Religion | comparative frame: belief, ritual, ethics, community, texts | EN + TH | Smith: The World's Religions | Religion strand [[01_Buddhist_Principles]] |
| 02 | Christianity | history, denominations, Bible, core beliefs | EN + TH | Smith | Religion strand other-religions |
| 03 | Islam | history, Five Pillars, Quran, Sunni/Shia | EN + TH | Smith | Religion strand other-religions |
| 04 | Judaism | Torah, history, traditions | EN + TH | Smith | History strand |
| 05 | Hinduism | Vedas, deities, karma/dharma/moksha | EN + TH | Smith | Mythology 17 (Ramayana) |
| 06 | Sikhism | gurus, scripture, practices | EN + TH | Smith | |
| 07 | Chinese Religious Traditions | Confucianism as tradition, Daoism, folk religion | EN + TH | Smith | Philosophy 20 |
| 08 | Shinto and Japanese Traditions | kami, shrines, festivals | EN + TH | Smith | |
| 09 | Zoroastrianism | first monotheism, influence | EN + TH | Smith | History strand ancient civilizations |
| 10 | Indigenous and Animist Traditions | world overview | EN + TH | Armstrong | Thai spirit-house / folk belief notes |
| 11 | Comparative Themes | creation, afterlife, golden rule, pilgrimage, fasting | EN + TH | Smith | Religion strand ceremonies |
| 12 | What Is Mythology | myth vs legend vs folktale; hero's journey | EN + TH | Campbell: Hero with a Thousand Faces | ภาษาไทย นิทานและตำนาน |
| 13 | Greek Mythology | Olympians, heroes, Trojan War | EN + TH | Hamilton: Mythology | World Literature 02-03 |
| 14 | Norse Mythology | gods, Ragnarok | EN + TH | Gaiman: Norse Mythology | |
| 15 | Egyptian Mythology | gods, afterlife, Book of the Dead | EN + TH | Hamilton excerpts | |
| 16 | Mesopotamian Mythology | Enuma Elish, Gilgamesh | EN + TH | translations | History strand ancient civilizations |
| 17 | Hindu Mythology | Ramayana, Mahabharata | EN + TH | Bhagavad Gita | **รามเกียรติ์ ↔ Ramayana** (gold cross-link to ภาษาไทย วรรณคดี) |
| 18 | East Asian Mythology | Journey to the West, Kojiki | EN + TH | translations | World Literature 17 |
| 19 | Universal Mythic Archetypes | flood myths, tricksters, underworld journeys | EN + TH | Campbell | |
| 20 | Mythology in Modern Culture | retellings, films, games | EN + TH | Fry: Mythos | Art folder, CS games notes |

---

## 8. Book Pipeline

Follows the vault's established multi-profile flow.

**Step 1 (educator):** create `checklist/` files following the existing pattern (priority tiers, status checkboxes, Why column, Thai translation availability):
- `checklist/Philosophy - Books.md`
- `checklist/World Literature - Books.md`
- `checklist/World Religions and Mythology - Books.md`

**Step 2 (book-summarizer profile):** summarize from checklists into `Book/<Title>/` (pattern already used for `Book/Sapiens`).

**Step 3 (educator):** enrich topic notes with summarized book content; tick checklist statuses.

Starter recommendations (tiers):

| Domain | 🔴 Essential | 🟡 Recommended | 🟢 Deep dive |
|---|---|---|---|
| Philosophy | Sophie's World (Gaarder): best first book, philosophy as story; A Little History of Philosophy (Warburton); The Story of Philosophy (Durant) | Meditations (Aurelius), The Republic (Plato), On Liberty (Mill), Tao Te Ching, Existentialism Is a Humanism (Sartre) | A History of Western Philosophy (Russell, reference), Think (Blackburn) |
| World Literature | the works themselves in translation (Thai editions exist for major classics) | A Little History of Literature (Sutherland), The Well-Educated Mind (Bauer) | How to Read a Book (Adler) |
| Religions/Mythology | The World's Religions (Smith), Mythology (Hamilton), Norse Mythology (Gaiman) | A History of God (Armstrong), Hero with a Thousand Faces (Campbell), Bhagavad Gita | A History of Religious Ideas (Eliade) |

Note: Sophie's World bridges Philosophy AND World Literature (novel form) AND the existing `Book/Sapiens` shelf-mate: summarize it first.

---

## 9. Cross-Link Plan (the "deepen existing" half)

Bidirectional links between the new root and existing content. Highlight relationships:

| New note | Existing note(s) | Why |
|---|---|---|
| Hellenistic Philosophy (06) | Social Studies Economics: Sufficiency Economy | Stoicism ↔ พอเพียง: same core insight, different cultures |
| What Is Religion / Comparative Themes | Social Studies 01 Religion: Buddhism notes | Buddhism as one tradition among many, not the only lens |
| Hindu Mythology (17) | ภาษาไทย วรรณคดี: รามเกียรติ์ | Same epic, two traditions: the vault's single best bridge note |
| Children's Classics and Folk Tales | ภาษาไทย นิทานและตำนาน | Aesop ↔ Thai fables |
| Poetry of the World | ภาษาไทย หลักการใช้ภาษาไทย: ฉันทลักษณ์ | Meter and rhyme systems compared |
| How to Read Literature | ภาษาไทย การวิเคราะห์วรรณคดี | Shared analytical toolkit |
| Philosophy of Science (19) | Science Fundamental: 01_Scientific_Method | The curriculum note's philosophical foundation |
| Political Philosophy (18) | Social Studies 02 Civics: Democracy | Social contract ↔ Thai constitutional civics |
| Greek Mythology (13) | Art 03 Performing Arts | Greek tragedy ↔ theatre history |
| Mythology in Modern Culture (20) | Art folder + CS games notes | Where myths live today |
| Dystopian Fiction (15) | Civics 12_Media_Literacy | Surveillance and information control |
| Applied Ethics Today (22*) | Health-PE + work-careers-technology | Bioethics, tech ethics |

Direction: new notes link to existing via short wikilinks; existing notes gain links back only where the topic genuinely touches them (no forced edits across 580 files).

---

## 10. Build Phases

| Phase | Work | Owner | Done when |
|---|---|---|---|
| 0 | Baseline hygiene: 20 missing notes, ~92 link fixes, duplicate pair, N1 | educator (this profile) | checker: 0 broken outside `Audit/` |
| 1 | Scaffolding: BOK layer ✅ done 2026-09-05 (`body-of-knowledge/General Knowledge/`); book checklists in `checklist/` ⬜; content-root `00_overview.md` trackers created with each domain build | educator (this profile) | user approves template + checklists |
| 2 | Philosophy build: 20-22 notes | educator; book-summarizer runs Sophie's World etc. in parallel | progress tracker 100% |
| 3 | World Literature build: 20-22 notes | same | tracker 100% |
| 4 | Religions and Mythology build: 20 notes | same | tracker 100% |
| 5 | Re-audit: new audit doc in `Audit/` (knowledge_audit_2026MMDD_general-knowledge-layer.md), link checker clean, tracker claims vs disk | QA profile | verified |

---

## 11. Open Items / User TODO

1. **Language per topic**: edit the Language column in §5-7 (suggestions are EN + TH everywhere; the user said they will decide per topic).
2. **Book list approval**: confirm or edit the starter recommendations in §8 (especially Thai translation availability).
3. **Mythology placement**: keep mythology inside folder 03, or split into its own folder 04? (Proposal keeps them together.)
4. **Optional notes**: mark the `*` notes in §5-6 keep/trim.
5. **Template**: approve the §4 note template before Phase 2 starts.

---

## 12. Change Request

Edit this file directly, or tell Edu what to change: scope, order, names, counts. The locked decisions (§1) are the contract; anything else is adjustable.
