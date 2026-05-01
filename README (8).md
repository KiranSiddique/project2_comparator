# 📊 Hash Method Comparator

**Course:** Analysis of Algorithms  
**Student:** Kiran Siddique  
**Registration No:** 2023-BCS-052  
**University:** FJWU  

---

## 📌 Overview

A side-by-side comparison tool for all four major hash collision handling methods. Enter a seed number to generate your own personal dataset, then instantly compare how Separate Chaining, Linear Probing, Quadratic Probing, and Double Hashing perform on that data — with collision counts, average steps, and a visual bar chart.

---

## ✨ Features

- **Generates a personal dataset** from any seed number using the formula `(seed × i + i²) mod 997`
- **Compares all 4 methods simultaneously:**
  - Separate Chaining
  - Linear Probing
  - Quadratic Probing
  - Double Hashing
- **Both hash functions tested for each method:**
  - `H1: k mod m`
  - `H2: ⌊(k²/10)⌋ mod m`
- **Summary cards** — shows best collision count per method
- **Animated bar chart** — visual comparison of collision counts across all 8 combinations
- **Detailed comparison table** — collisions, average steps, load factor, and best/worst badges
- **Insight section** — explains results in plain English with real-world context

---

## 🚀 How to Run

No installation needed. Just open the file in any modern browser:

```
project2_comparator.html
```

Enter your seed, set the number of keys and table size, then click **Compare**.

---

## 🧠 Concepts Demonstrated

| Concept | Description |
|---|---|
| Separate Chaining | Uses linked lists at each slot; no limit on keys per slot |
| Linear Probing | Open addressing — probe `(h(k) + i) mod m` |
| Quadratic Probing | Open addressing — probe `(h(k) + i²) mod m` |
| Double Hashing | Probe step itself is a second hash: `R - (k mod R)` |
| Average Steps | Average number of comparisons per insertion |
| Load Factor α | `n / m` — key measure of table fullness |

---

## 📐 Algorithm Details

**Double Hashing formula used:**
```
pos = (h(k) + i × step) mod m
step = R - (k mod R),  where R = 37
```

**Key generation formula:**
```
keys[i] = (seed × i + i²) mod 997
```

---

## 🔧 Tech Stack

- HTML5
- CSS3 (grid layout, CSS variables, transitions)
- Vanilla JavaScript
- Google Fonts (DM Serif Display, DM Mono, DM Sans)
