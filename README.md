# TDTU_ITProject_Final
This is IT Project Code Repository by student Yamin Thiri Wai(522k0046), Thant Thiri Maung(522k0050). This repository include implementation of HUOPM, HUOMIL and HUOPM-Improved (Dictionary-Join &amp; Adaptive Pruning).

---
## Problem Definition

High Utility Occupancy Pattern Mining (HUOPM) aims to discover itemsets that are not only frequent but also contribute a significant proportion of utility within the transactions in which they appear.

Given:
- A transactional quantitative database D = {T1, T2, ..., Tn}, where each transaction contains items with associated quantities.
- A profit table (PT) that assigns a unit utility (profit) value to each item.
- A user-defined minimum support threshold (alpha).
- A user-defined minimum utility occupancy threshold (beta).

The objective of HUOPM is to identify all itemsets X ⊆ I such that:
- Support condition:  
  sup(X) ≥ alpha × |D|
- Utility occupancy condition:  
  uo(X) ≥ beta

An itemset that satisfies both conditions is called a **High Utility Occupancy Pattern (HUOP)**.  
These patterns highlight item combinations that are both commonly occurring and economically significant relative to the transactions in which they appear.

### Input

The **HUOPM (High Utility Occupancy Pattern Mining)** problem takes the following inputs:

- **Transactional quantitative database**  
  D = {T1, T2, ..., Tn}, where each transaction contains items with associated quantities.

- **Profit table (PT)**  
  A table that assigns a unit utility (profit) value to each item in the item set I.

- **Minimum support threshold (alpha)**  
  A user-defined threshold specifying the minimum frequency requirement for an itemset.

- **Minimum utility occupancy threshold (beta)**  
  A user-defined threshold specifying the minimum relative utility contribution required for an itemset.


### Output

The output of the HUOPM process is a complete set:

H = { X | X ⊆ I, sup(X) ≥ alpha × |D|, uo(X) ≥ beta }

This set consists of all **High Utility Occupancy Patterns (HUOPs)** that satisfy both the support and utility occupancy constraints.

Each discovered pattern X ∈ H is accompanied by:

- **Support value**: sup(X)
- **Utility occupancy value**: uo(X)


---


## Repository Structure

### [`datasets/`](datasets)
Contains all transactional datasets used in experiments.

➡️ Dataset details and statistics:  
📄 [`datasets/README.md`](datasets/README.md)

---

### [`source/`](source)
Contains algorithm implementations, analysis, and evaluation notebooks.

➡️ Source code details:  
📄 [`source/README.md`](source/README.md)

---

## Experimental Evaluation

The algorithms are evaluated using:
- Runtime performance
- Memory consumption
- Dataset characteristics (dense vs sparse)

Experiments are conducted on multiple real-world benchmark datasets.

---

## Academic Note
This repository is intended for **research and educational purposes only**.  
The original algorithm ideas belong to their respective authors.
