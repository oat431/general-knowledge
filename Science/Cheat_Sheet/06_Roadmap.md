---
tags:
  - science
  - cheatsheet
  - roadmap
level: "Meta: the map of all layers"
sources: ["[[00_Index]]"]
created: 2026-10-07
---

# Science Roadmap: From Quarks to Computation

> *"The board on the box lid: five layers of reality, every piece, and the order you unlock them."*

This roadmap shows the whole journey as **one dependency map**: each node is a topic, each arrow means "learn this first", and each layer builds on the one below. Click any node to jump to its rulebook.

---

## The Full Map

```mermaid
flowchart TD
    subgraph L1["Layer 1: Physics — the laws everything obeys"]
        P1["Measurement and<br/>Scientific Method"] --> P2["Kinematics<br/>Motion"]
        P2 --> P3["Dynamics<br/>Newton's Laws"]
        P3 --> P4["Work, Energy<br/>and Power"]
        P3 --> P5["Momentum<br/>and Collisions"]
        P4 --> P6["Heat and<br/>Thermodynamics"]
        P2 --> P7["Waves, Sound<br/>and Light"]
        P3 --> P8["Electrostatics<br/>and Circuits"]
        P8 --> P9["Magnetism and<br/>EM Induction"]
        P7 --> P10["Modern Physics<br/>Quantum and Relativity"]
        P9 --> P10
        P10 --> P11["Nuclear Physics"]
    end

    subgraph L2["Layer 2: Chemistry — the rules of matter"]
        C1["Atomic Structure<br/>built on quantum rules"] --> C2["Periodic Table<br/>and Trends"]
        C2 --> C3["Chemical Bonding"]
        C3 --> C4["Intermolecular<br/>Forces"]
        C1 --> C5["Stoichiometry<br/>and the Mole"]
        C5 --> C6["Solutions and<br/>Gas Laws"]
        C4 --> C7["Acids, Bases<br/>and Equilibrium"]
        C6 --> C7
        C5 --> C8["Thermochemistry<br/>and Kinetics"]
        C3 --> C9["Organic Chemistry<br/>and Polymers"]
        C1 --> C10["Nuclear Chemistry"]
    end

    subgraph L3["Layer 3: Biology — the rules of the living"]
        B1["Cell Biology<br/>chemistry in a bag"] --> B2["Biomolecules"]
        B2 --> B3["Cell Energy<br/>ATP, photosynthesis, respiration"]
        B2 --> B4["Molecular Biology<br/>DNA and Central Dogma"]
        B4 --> B5["Cell Division"]
        B5 --> B6["Genetics<br/>and Inheritance"]
        B6 --> B7["Evolution<br/>and Diversity"]
        B3 --> B8["Human Body<br/>Systems"]
        B7 --> B9["Ecology<br/>energy flow and cycles"]
    end

    subgraph L4["Layer 4: Earth Science — the rules of our planet"]
        E1["Minerals and Rocks"] --> E2["Plate Tectonics"]
        E2 --> E3["Earthquakes<br/>and Volcanoes"]
        E1 --> E4["Weathering<br/>and Erosion"]
        E2 --> E5["Earth History<br/>Deep Time"]
        E6["Weather and<br/>Climate"] --> E7["Water Cycle and<br/>Hydrology"]
        E6 --> E8["Climate Change<br/>carbon cycle"]
        E9["Solar System<br/>and Astronomy"]
    end

    subgraph L5["Layer 5: Computer Science — the rules we invented"]
        S1["Computational<br/>Thinking"] --> S2["Data Representation<br/>binary and information"]
        S1 --> S3["Boolean Logic<br/>and Gates"]
        S3 --> S4["Programming<br/>Fundamentals"]
        S4 --> S5["Functions and<br/>Modularity"]
        S5 --> S6["Algorithms<br/>and Big-O"]
        S5 --> S7["Data Structures"]
        S6 --> S8["Computer Systems<br/>and Networks"]
        S8 --> S9["Databases"]
        S6 --> S10["Artificial<br/>Intelligence"]
        S9 --> S11["Digital Citizenship<br/>and Security"]
    end

    P10 ==>|quantum rules| C1
    P11 ==>|nuclear physics| C10
    P4 ==>|energy conservation| C8
    P6 ==>|thermodynamics| C8
    C3 ==>|bonding makes molecules| B2
    C4 ==>|intermolecular forces| B1
    C7 ==>|pH and buffers| B8
    C9 ==>|organic chemistry| B2
    B3 ==>|life shapes atmosphere| E8
    B9 ==>|ecosystems and climate| E8
    P3 ==>|gravity drives orbits| E9
    P6 ==>|heat drives weather| E6
    E1 ==>|geology shapes habitats| B7
    S2 ==>|bits are physical| P10
    S8 ==>|networks are physics| P9

    style L1 fill:#19362D,color:#CDD3D1,stroke:#1FB854
    style L2 fill:#19362D,color:#CDD3D1,stroke:#1EB88E
    style L3 fill:#19362D,color:#CDD3D1,stroke:#1FB8AB
    style L4 fill:#19362D,color:#CDD3D1,stroke:#1FB854
    style L5 fill:#19362D,color:#CDD3D1,stroke:#1EB88E
```

**Reading the map:**
- Thin arrows `-->` = learn this first (within a layer)
- Thick arrows `==>` = cross-layer dependencies (why the stack is real)

---

## The Unlock Order

| Stage | Rulebook | Why it comes here |
|---|---|---|
| 1 | [[01_Physics_Motion_and_Energy]] | The substrate: matter, energy, forces. Nothing above works without it |
| 2 | [[02_Chemistry_Matter_and_Reactions]] | Physics applied to atoms: quantum rules + EM force = bonding behavior |
| 3 | [[03_Biology_Life_and_Evolution]] | Chemistry that self-replicates: molecules → cells → organisms → evolution |
| 4 | [[04_Earth_Science_Systems_and_Cycles]] | All three lower layers running on one planet for 4.6 billion years |
| 5 | [[05_Computer_Science_Logic_and_Information]] | The layer we built: logic made physical with electrons from Layer 1 |

---

## Three Rules That Cross Every Layer

The deepest patterns repeat at every scale — these are the "meta-rules" of the world:

### Conservation (การอนุรักษ์)
- **Physics:** energy, momentum, charge are conserved
- **Chemistry:** mass is conserved in reactions (Lavoisier)
- **Biology:** energy flows through ecosystems, never created or destroyed
- **Earth:** the rock cycle recycles matter; plate tectonics conserves surface area
- **CS:** information is conserved in reversible computation; bits can't be copied perfectly (no-cloning in quantum)

### Cycles (วัฏจักร)
- **Physics:** oscillations, waves, orbits
- **Chemistry:** equilibrium, reaction cycles (Calvin, Krebs)
- **Biology:** cell cycle, biogeochemical cycles, life cycles
- **Earth:** rock cycle, water cycle, carbon cycle
- **CS:** the fetch-decode-execute loop, event loops

### Emergence (การอุบัติใหม่)
- **Physics:** thermodynamics emerges from particle statistics
- **Chemistry:** wetness, color, reactivity emerge from electron arrangements
- **Biology:** life emerges from non-living chemistry; consciousness from neurons
- **Earth:** climate emerges from atmosphere-ocean-land interactions
- **CS:** intelligence emerges from simple gates; the internet emerges from protocols

> 💡 **Deeper why:** The reason the same three patterns appear at every layer is that each layer is a *complex system* built from the one below. Conservation comes from symmetries in the laws (Noether), cycles come from feedback (restoring forces), and emergence comes from many interacting parts producing behavior no single part has.

---

## Suggested Reading Paths

**Exam sprint (ม.6):** Read each rulebook's Section 1–2 only, plus the `When to use` lines. Two hours total.

**Deep understanding:** Read 01 → 05 in order, stopping at every `💡 Deeper why` callout. One week.

**Curiosity path:** Start at [[03_Biology_Life_and_Evolution]] (evolution patterns), then [[04_Earth_Science_Systems_and_Cycles]] (deep time), then work down to [[01_Physics_Motion_and_Energy]] to find the foundations.

---

## Chain Navigation

⬅ [[05_Computer_Science_Logic_and_Information]] · 🏠 [[00_Index]] · ➡ *(end of chain)*
