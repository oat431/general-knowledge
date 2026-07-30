---
tags:
  - computer-science
  - advance
  - data-structures
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว332"]
---

# Data Structures — โครงสร้างข้อมูล

> *"The choice of data structure is at least as important as the choice of algorithm."* — Niklaus Wirth

Data structures (โครงสร้างข้อมูล) are organized ways of storing, managing, and accessing data so that operations can be performed efficiently. They are the containers that algorithms manipulate; choosing the right structure determines whether a program runs in milliseconds or hours. In Python, the built-in collections — lists, tuples, dictionaries, and sets — cover most everyday needs.

This note covers the core data structures required by the IPST curriculum (ว332): arrays/lists, stacks, queues, hash maps, tuples, sets, trees, and graphs. For each, we examine the core operations (เพิ่ม/ลด/ค้นหา — insert/delete/search), their time complexity, and when to choose one over another.

---

## 1 | Course Coverage

### ม.5 (ว332)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Linear structures: lists, stacks, queues, tuples | Implement push/pop, enqueue/dequeue, slicing |
| **Semester 2** | Mappings and hierarchies: dictionaries, sets, trees, graphs | Build adjacency lists, traverse trees, select structures |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| โครงสร้างข้อมูล | Data structure | Container for organized data |
| อาร์เรย์ / ลิสต์ | Array / List | Indexed, contiguous storage |
| สแต็ก | Stack | LIFO (Last-In-First-Out) |
| คิว | Queue | FIFO (First-In-First-Out) |
| พจนานุกรม / แฮชแมป | Dictionary / Hash map | Key → value, $O(1)$ lookup |
| ทูเพิล | Tuple | Immutable sequence |
| เซต | Set | Unique, unordered elements |
| ต้นไม้ | Tree | Hierarchical, root → leaves |
| กราฟ | Graph | Nodes (vertices) + edges |
| โหนด / จุดยอด | Node / Vertex | A single data element |
| การแวะผ่าน | Traversal | Visiting every node |

---

## 3 | Key Concepts

### 3.1 Lists / Arrays (ลิสต์ / อาร์เรย์)

A list (ลิสต์) is an ordered, mutable, zero-indexed sequence. Python lists are dynamic arrays — they grow and shrink automatically.

```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])      # "apple"  (zero-indexed)
print(fruits[-1])     # "cherry" (negative = from end)
print(fruits[1:3])    # ["banana","cherry"] (slicing, exclusive end)

fruits.append("date")      # add to end    O(1) amortized
fruits.insert(1, "avocado")# insert at idx O(n)
fruits.remove("banana")    # remove by val  O(n)
len(fruits)                # 4
```

### 3.2 Stacks (สแต็ก) — LIFO

A stack (สแต็ก) follows **Last-In-First-Out**: the last element added is the first removed. Think of a stack of plates.

```python
stack = []
stack.append(10)   # push
stack.append(20)
stack.append(30)
top = stack.pop()  # 30  (pop removes + returns last)
peek = stack[-1]   # 20  (peek without removing)
```

Use cases: undo/redo, function call stack (call stack), expression evaluation, backtracking.

### 3.3 Queues (คิว) — FIFO

A queue (คิว) follows **First-In-First-Out**: the first element added is the first removed — like a line at a ticket counter.

```python
from collections import deque   # efficient O(1) both ends
q = deque()
q.append("A")      # enqueue
q.append("B")
q.append("C")
first = q.popleft()  # "A"  (dequeue)
```

Use cases: print spooler, BFS (breadth-first search), task scheduling.

### 3.4 Dictionaries / Hash Maps (พจนานุกรม)

A dictionary (พจนานุกรม) maps **keys** to **values** with average $O(1)$ lookup using a hash function (ฟังก์ชันแฮช).

```python
scores = {"Alice": 90, "Bob": 85}
scores["Charlie"] = 78      # add
scores["Alice"] = 95        # update
del scores["Bob"]           # delete
for name, score in scores.items():
    print(name, score)
```

### 3.5 Tuples and Sets (ทูเพิลและเซต)

- **Tuple (ทูเพิล):** immutable sequence — once created, cannot change. Faster and hashable.
  ```python
  point = (3, 4)
  x, y = point     # unpacking
  ```
- **Set (เซต):** unordered collection of **unique** elements. Supports union, intersection, difference.
  ```python
  a = {1, 2, 3}
  b = {3, 4, 5}
  a | b   # {1,2,3,4,5}  union
  a & b   # {3}          intersection
  a - b   # {1,2}        difference
  ```

### 3.6 Trees (ต้นไม้)

A tree (ต้นไม้) is a hierarchical structure with a **root** node; each node has zero or more **children**. A **binary tree** (ต้นไม้ทวิภาค) has at most two children per node.

```python
class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

# Build:       1
#            /   \
#           2     3
root = Node(1)
root.left = Node(2)
root.right = Node(3)

def inorder(node):
    if node:
        inorder(node.left)
        print(node.value, end=" ")
        inorder(node.right)

inorder(root)   # 2 1 3  (left, root, right)
```

Traversals: **in-order** (left→root→right), **pre-order** (root→left→right), **post-order** (left→right→root), and **level-order** (BFS).

### 3.7 Graphs (กราฟ)

A graph (กราฟ) consists of **vertices** (จุดยอด) connected by **edges** (เส้นเชื่อม). An **adjacency list** (รายชื่อ adjacency) is the most common representation.

```python
graph = {
    "A": ["B", "C"],
    "B": ["A", "D"],
    "C": ["A"],
    "D": ["B"]
}
# A -- B -- D
#  \
#   C
```

Graphs model social networks, maps/routing, and dependencies.

### 3.8 Choosing the Right Structure

| Need | Best structure | Why |
|---|---|---|
| Ordered, indexable | list | $O(1)$ random access |
| Key→value lookup | dict | $O(1)$ average search |
| Unique elements | set | dedup + set operations |
| Undo / backtracking | stack | LIFO matches last action |
| Fair processing order | queue | FIFO matches arrival |
| Hierarchical data | tree | parent-child relationships |
| Networked relations | graph | many-to-many connections |

---

## 4 | Common Problem Types

### Type 1: Reverse a String Using a Stack

> Push every character of a string onto a stack, then pop them all — the reversed order emerges naturally from LIFO.

**Solution:**
```python
def reverse_string(s):
    stack = []
    for ch in s:
        stack.append(ch)
    reversed_s = ""
    while stack:
        reversed_s += stack.pop()
    return reversed_s

print(reverse_string("hello"))  # "olleh"
```

### Type 2: Balanced Parentheses Checker

> Determine whether a string of `()[]{}` has matching, correctly nested brackets.

**Solution:**
```python
def is_balanced(expr):
    pairs = {")": "(", "]": "[", "}": "{"}
    stack = []
    for ch in expr:
        if ch in "([{":
            stack.append(ch)
        elif ch in ")]}":
            if not stack or stack.pop() != pairs[ch]:
                return False
    return len(stack) == 0

print(is_balanced("({[]})"))   # True
print(is_balanced("({[)]}"))   # False
```

### Type 3: Word Frequency Counter (Dictionary)

> Count how many times each word appears in a sentence.

**Solution:**
```python
def word_freq(text):
    freq = {}
    for word in text.split():
        word = word.lower().strip(".,!?")
        freq[word] = freq.get(word, 0) + 1
    return freq

print(word_freq("the cat and the dog and the bird"))
# {'the': 3, 'cat': 1, 'and': 2, 'dog': 1, 'bird': 1}
```

---

## 5 | Cross-Links

- [[06_Algorithms]] — prerequisite: algorithms operate on data structures
- [[08_Object_Oriented_Programming]] — implement structures as classes
- [[10_Databases]] — tables are a structured data form
- [[../../Fundamental/17_Sets|Mathematics: Sets]] — set operations in math and code
