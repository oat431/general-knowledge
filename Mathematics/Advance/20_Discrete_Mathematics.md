---
tags:
  - mathematics
  - advance
  - discrete-mathematics
  - graph-theory
  - combinatorics
  - ipst
source: "IPST (สสวท.) Mathematics Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ค303"]
---

# Discrete Mathematics — คณิตศาสตร์ discrete

> *"Discrete mathematics studies structures that are separate and distinct — the mathematics of computation."*

Discrete mathematics deals with countable, distinct structures rather than continuous quantities. This topic introduces graph theory, combinatorics, and recurrence relations — the mathematical foundations of computer science, algorithms, and network analysis.

---

## 1 | Course Coverage

### ม.6 (ค303)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Combinatorics review | Permutations, combinations; inclusion-exclusion; pigeonhole principle |
| **Semester 1** | Graph theory basics | Vertices, edges; degree; paths and circuits; connected graphs |
| **Semester 1** | Special graphs | Trees; complete graphs; bipartite graphs; planar graphs |
| **Semester 1** | Euler and Hamilton | Euler paths/circuits; Hamilton paths/cycles; applications |
| **Semester 1** | Recurrence relations | Linear recurrence; solving first-order; applications |
| **Semester 1** | Algorithms | Sorting; shortest path; spanning trees (intro) |

---

## 2 | Key Terminology

| Thai | English | Notes |
|---|---|---|
| ทฤษฎีกราฟ | Graph theory | $G = (V, E)$ |
| จุดยอด | Vertex | $v$ |
| เส้นเชื่อม | Edge | $e$ |
| ดีกรี | Degree | $\deg(v)$ |
| เส้นทาง | Path | Sequence of edges |
| วงจร | Circuit/cycle | Path returning to start |
| กราฟเชื่อมต่อ | Connected graph | Path exists between any two vertices |
| ต้นไม้ | Tree | Connected, acyclic graph |
| วงจรเออเลอร์ | Euler circuit | Uses every edge exactly once |
| วงจรแฮมิลตัน | Hamilton cycle | Visits every vertex exactly once |
| ความสัมพันธ์เวียนเกิด | Recurrence relation | $a_n = f(a_{n-1}, ...)$ |

---

## 3 | Key Concepts

### 3.1 Graph Basics

A **graph** $G = (V, E)$ consists of:
- **Vertices ($V$):** Set of points (nodes)
- **Edges ($E$):** Connections between vertices

**Degree of a vertex:** Number of edges incident to it.

**Handshaking Lemma:**
$$\sum_{v \in V} \deg(v) = 2|E|$$

The sum of all degrees is always even.

### 3.2 Paths and Circuits

- **Path:** Sequence of vertices connected by edges, no repetition
- **Trail:** Walk with no repeated edges
- **Circuit:** Closed trail (starts and ends at same vertex)

### 3.3 Euler Paths and Circuits

**Euler circuit:** Uses every edge exactly once and returns to start.

**Euler's Theorem:**
- A connected graph has an **Euler circuit** if and only if every vertex has **even degree**.
- A connected graph has an **Euler path** (not circuit) if and only if exactly **two vertices have odd degree**.

### 3.4 Hamilton Paths and Cycles

**Hamilton cycle:** Visits every vertex exactly once and returns to start.

Unlike Euler paths, there is no simple criterion for Hamilton cycles.

### 3.5 Trees

A **tree** is a connected graph with no cycles.

**Properties:**
- A tree with $n$ vertices has $n - 1$ edges
- Exactly one path between any two vertices
- Adding any edge creates a cycle
- Removing any edge disconnects the graph

**Spanning tree:** A subgraph that is a tree and includes all vertices.

### 3.6 Recurrence Relations

A **recurrence relation** defines a sequence recursively.

**First-order linear recurrence:**
$$a_n = r \cdot a_{n-1} + c$$

**Solution (if $r \neq 1$):**
$$a_n = r^n \cdot a_0 + c \cdot \frac{r^n - 1}{r - 1}$$

**Example:** Fibonacci sequence
$$F_n = F_{n-1} + F_{n-2}, \quad F_0 = 0, \; F_1 = 1$$

### 3.7 Pigeonhole Principle

If $n$ items are placed into $m$ containers and $n > m$, then at least one container contains more than one item.

**Example:** In a group of 367 people, at least two share a birthday (366 possible days).

### 3.8 Inclusion-Exclusion Principle

For two sets:
$$|A \cup B| = |A| + |B| - |A \cap B|$$

For three sets:
$$|A \cup B \cup C| = |A| + |B| + |C| - |A \cap B| - |A \cap C| - |B \cap C| + |A \cap B \cap C|$$

### 3.9 Complete Graphs and Bipartite Graphs

| Graph type | Description | Edges |
|---|---|---|
| **Complete graph $K_n$** | Every pair of vertices connected | $\frac{n(n-1)}{2}$ |
| **Bipartite graph** | Vertices split into two groups; edges only between groups | At most $mn$ for groups of $m$ and $n$ |
| **Cycle graph $C_n$** | Vertices arranged in a single cycle | $n$ |
| **Path graph $P_n$** | Vertices in a single path | $n-1$ |

### 3.10 Planar Graphs and Euler's Formula

A graph is **planar** if it can be drawn without any edges crossing.

**Euler's Formula** for connected planar graphs:
$$V - E + F = 2$$

where $V$ = vertices, $E$ = edges, $F$ = faces (including the outer face).

**Example:** A cube graph has $V = 8$, $E = 12$, $F = 6$. Check: $8 - 12 + 6 = 2$ ✓

### 3.11 Kruskal's Algorithm (Minimum Spanning Tree)

To find a minimum spanning tree:
1. List all edges in order of increasing weight
2. Add the smallest edge that does not create a cycle
3. Repeat until all vertices are connected ($n-1$ edges for $n$ vertices)

---

## 4 | Common Problem Types

### Type 1: Graph Degree
> A graph has 5 vertices with degrees 2, 3, 4, 3, 4. How many edges?

**Solution:** Sum of degrees = 16. By Handshaking Lemma: $|E| = 16/2 = 8$.

### Type 2: Euler Circuit
> Does a graph with vertex degrees 2, 2, 3, 3 have an Euler circuit?

**Solution:** No. Not all degrees are even (two vertices have degree 3). But it has an Euler path (exactly two odd vertices).

### Type 3: Tree Properties
> A tree has 12 vertices. How many edges?

**Solution:** $n - 1 = 11$ edges.

### Type 4: Recurrence Relation
> Solve $a_n = 2a_{n-1} + 1$ with $a_0 = 0$.

**Solution:** $r = 2$, $c = 1$.
$a_n = 2^n(0) + 1 \cdot \frac{2^n - 1}{2 - 1} = 2^n - 1$

### Type 5: Pigeonhole Principle
> Show that among any 5 points in an equilateral triangle of side 1, at least two are within distance $1/2$.

**Solution:** Divide triangle into 4 smaller equilateral triangles of side $1/2$. By pigeonhole, at least 2 of 5 points fall in the same small triangle, so their distance is at most $1/2$.

### Type 6: Counting with Inclusion-Exclusion
> How many integers from 1 to 100 are divisible by 2 or 3?

**Solution:**
$|A| = 50$ (divisible by 2), $|B| = 33$ (divisible by 3), $|A \cap B| = 16$ (divisible by 6)
$|A \cup B| = 50 + 33 - 16 = 67$

---

## 5 | Cross-Links

- [[01_Sets_and_Logic]] — Set operations, logic
- [[17_Probability]] — Counting principles
- [[08_Sequences_and_Series]] — Recurrence relations
- [[05_Computer Science - Overview]] — Algorithms, data structures
