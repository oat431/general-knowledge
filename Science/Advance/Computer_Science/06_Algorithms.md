---
tags:
  - computer-science
  - advance
  - algorithms
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว332"]
---

# Algorithms — อัลกอริทึม

> *"An algorithm must be seen to be believed."* — Donald Knuth

An algorithm (อัลกอริทึม) is a finite, well-defined sequence of steps that solves a class of problems. The IPST curriculum in ม.5 (ว332) studies classic algorithms for searching (การค้นหา) and sorting (การเรียบลำดับ), and introduces algorithmic complexity (ความซับซ้อนของอัลกอริทึม) so students can reason about efficiency rather than guess.

Beyond memorising code, the goal is to understand *why* some algorithms are faster than others, how to express solutions in pseudocode and flowcharts, and how to make informed trade-offs between time and memory (การแลกเปลี่ยนเวลากับพื้นที่). This note ties together the computational thinking, data representation, and programming skills learned earlier.

---

## 1 | Course Coverage

### ม.5 (ว332)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Algorithm design process; pseudocode and flowcharts; linear and binary search; bubble, selection, insertion sort | Trace algorithms, implement searching & sorting |
| **Semester 2** | Introduction to merge sort; Big-O notation; time vs space trade-offs; selecting algorithms by context | Analyse complexity, choose appropriate algorithm |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| อัลกอริทึม | Algorithm | finite steps |
| รหัสเทียม | Pseudocode | informal description |
| ผังงาน | Flowchart | diagram |
| การค้นหาแบบลำดับ | Linear Search | O(n) |
| การค้นหาแบบทวิภาค | Binary Search | O(log n) |
| การเรียบลำดับแบบฟอง | Bubble Sort | O(n²) |
| การเรียบลำดับแบบเลือก | Selection Sort | O(n²) |
| การเรียบลำดับแบบแทรก | Insertion Sort | O(n²) |
| การเรียบลำดับแบบผสาน | Merge Sort | O(n log n) |
| ความซับซ้อนของเวลา | Time Complexity | Big-O |
| ความซับซ้อนของพื้นที่ | Space Complexity | memory |
| การแลกเปลี่ยน | Trade-off | time vs space |

---

## 3 | Key Concepts

### 3.1 Properties of an Algorithm

A valid algorithm is:

1. **Finite (จำกัด)** — terminates after a number of steps.
2. **Definite (แน่นอน)** — each step is unambiguous.
3. **Input** — zero or more inputs.
4. **Output** — at least one output.
5. **Effective (มีประสิทธิภาพ)** — each step is doable in finite time.

### 3.2 Linear Search (การค้นหาแบบลำดับ)

Check each element in turn until found or the list ends. Works on unsorted data.

```python
def linear_search(arr, target):
    for i, v in enumerate(arr):
        if v == target:
            return i
    return -1
```

Worst case: examine all $n$ elements → **$O(n)$**.

### 3.3 Binary Search (การค้นหาแบบทวิภาค)

Requires a **sorted** list. Repeatedly halve the search range.

```python
def binary_search(arr, target):
    lo, hi = 0, len(arr) - 1
    while lo <= hi:
        mid = (lo + hi) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            lo = mid + 1
        else:
            hi = mid - 1
    return -1
```

Each step halves the range → worst case **$O(\log n)$**.

### 3.4 Sorting Algorithms (การเรียบลำดับ)

**Bubble Sort (แบบฟอง)** — repeatedly swap adjacent out-of-order pairs; large values "bubble" to the end.

```python
def bubble_sort(arr):
    a = arr.copy()
    n = len(a)
    for i in range(n - 1):
        for j in range(n - 1 - i):
            if a[j] > a[j + 1]:
                a[j], a[j + 1] = a[j + 1], a[j]
    return a
```

**Selection Sort (แบบเลือก)** — repeatedly select the minimum and place it at the front.

```python
def selection_sort(arr):
    a = arr.copy()
    for i in range(len(a)):
        m = i
        for j in range(i + 1, len(a)):
            if a[j] < a[m]:
                m = j
        a[i], a[m] = a[m], a[i]
    return a
```

**Insertion Sort (แบบแทรก)** — build a sorted portion, inserting each next element into its place.

```python
def insertion_sort(arr):
    a = arr.copy()
    for i in range(1, len(a)):
        key = a[i]
        j = i - 1
        while j >= 0 and a[j] > key:
            a[j + 1] = a[j]
            j -= 1
        a[j + 1] = key
    return a
```

**Merge Sort (แบบผสาน)** — divide-and-conquer: split in half, sort each half, merge sorted halves.

```python
def merge_sort(arr):
    if len(arr) <= 1:
        return arr
    mid = len(arr) // 2
    left  = merge_sort(arr[:mid])
    right = merge_sort(arr[mid:])
    return merge(left, right)

def merge(L, R):
    result, i, j = [], 0, 0
    while i < len(L) and j < len(R):
        if L[i] <= R[j]:
            result.append(L[i]); i += 1
        else:
            result.append(R[j]); j += 1
    result.extend(L[i:]); result.extend(R[j:])
    return result
```

### 3.5 Big-O Notation (ความซับซ้อนของเวลา)

Big-O describes how runtime grows with input size $n$, ignoring constants.

| Complexity | Name | Example |
|---|---|---|
| $O(1)$ | Constant | array index |
| $O(\log n)$ | Logarithmic | binary search |
| $O(n)$ | Linear | linear search |
| $O(n \log n)$ | Linearithmic | merge sort |
| $O(n^2)$ | Quadratic | bubble / selection / insertion sort |

Growth rate order (slowest → fastest):

$$O(1) < O(\log n) < O(n) < O(n \log n) < O(n^2) < O(2^n)$$

### 3.6 Time vs Space Trade-off (การแลกเปลี่ยนเวลากับพื้นที่)

Often a faster algorithm uses more memory. Merge sort runs in $O(n \log n)$ time but needs $O(n)$ extra space; bubble sort is $O(n^2)$ but sorts in place ($O(1)$ extra). Choosing the right algorithm depends on the constraints of the problem.

---

## 4 | Common Problem Types

### Type 1: Trace a Search
> Given `arr = [3, 7, 11, 15, 22]` and `target = 15`, trace binary search.

**Solution:** `lo=0,hi=4 → mid=2 (11) → lo=3 → mid=3 (15) → found at index 3`. Two comparisons instead of four for linear search.

### Type 2: Sort by Hand, Then Code
> Sort `[5, 2, 9, 1]` using bubble sort, showing each pass.

**Solution:**

```
Pass 1: [5,2,9,1] → [2,5,9,1] → [2,5,9,1] → [2,5,1,9]
Pass 2: [2,5,1,9] → [2,5,1,9] → [2,1,5,9]
Pass 3: [1,2,5,9]
```

```python
print(bubble_sort([5, 2, 9, 1]))   # [1, 2, 5, 9]
```

### Type 3: Compare Complexity
> Which is faster for $n = 1\,000\,000$: linear search or binary search?

**Solution:** Linear ≈ $10^6$ operations; binary ≈ $\log_2 10^6 \approx 20$ operations. Binary search is roughly 50 000× faster — but it requires the data to be sorted first.

### Type 4: Count Operations
> How many comparisons does selection sort make for a list of $n$ elements?

**Solution:**

$$(n-1) + (n-2) + \dots + 1 = \frac{n(n-1)}{2} = O(n^2)$$

---

## 5 | Cross-Links

- [[01_Computational_Thinking]] — algorithm design is a pillar of CT
- [[04_Programming_Fundamentals]] — loops and conditionals implement algorithms
- [[05_Functions_and_Modularity]] — recursion enables merge sort and binary search
- [[../../Advance/Mathematics/Fundamental/01_Logarithms|Mathematics: Logarithms]] — basis of $O(\log n)$ analysis
