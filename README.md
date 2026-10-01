# BFS Implementation & Python Concepts

This repository contains a Jupyter Notebook (`BFS IMPLEMENTATION.ipynb`) demonstrating foundational Python programming concepts alongside a step-by-step Breadth-First Search (BFS) tree traversal implementation[cite: 1].

---

## Table of Contents

- [Overview](#overview)[cite: 1]
- [Notebook Breakdown](#notebook-breakdown)[cite: 1]
  - [Part 1: Function with List](#part-1-function-with-list)[cite: 1]
  - [Part 2: Lambda Function with List Comprehension](#part-2-lambda-function-with-list-comprehension)[cite: 1]
  - [Part 3: Object-Oriented Programming (OOP)](#part-3-object-oriented-programming-oop)[cite: 1]
  - [Part 4: Breadth-First Search (BFS) Algorithm](#part-4-breadth-first-search-bfs-algorithm)[cite: 1]
  - [Part 5: BFS Algorithm Dry Run](#part-5-bfs-algorithm-dry-run)[cite: 1]
- [Requirements](#requirements)[cite: 1]

---

## Overview

The notebook covers functional programming constructs in Python, basic Object-Oriented Programming, and data structure traversals using queues[cite: 1].

---

## Notebook Breakdown

### Part 1: Function with List
* Uses the `map()` higher-order function combined with a `lambda` expression to transform a list[cite: 1].
* Takes an input list (e.g., `[1, 2, 3, 4, 5]`) and returns a new list with each element squared (`[1, 4, 9, 16, 25]`)[cite: 1].

### Part 2: Lambda Function with List Comprehension
* Combines `lambda` functions with list comprehension to filter elements[cite: 1].
* Filters an array to return only even numbers (e.g., extracting `[2, 4]` from `[1, 2, 3, 4, 5]`)[cite: 1].

### Part 3: Object-Oriented Programming (OOP)
* Implements a `student` class to demonstrate object-oriented design principles[cite: 1].
* Initializes attributes: `name`, `roll_no`, and `semester`[cite: 1].
* Features a `display_information()` method to print formatted student details[cite: 1].

### Part 4: Breadth-First Search (BFS) Algorithm
* Defines a custom `treenode` class representing nodes with child references[cite: 1].
* Utilizes `collections.deque` for efficient queue operations (`popleft()`)[cite: 1].
* Performs level-order traversal on a constructed tree structure (Root node `A` through `L`), outputting the state of the queue at each step[cite: 1].
* Final output sequence: `['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L']`[cite: 1].

### Part 5: BFS Algorithm Dry Run
A complete trace of the BFS algorithm execution across 12 steps[cite: 1]:

| Step | Current Node | Queue After Popping | Children Added | Queue Now |
| :--- | :--- | :--- | :--- | :--- |
| **1** | A | [] | B, C, D | [B, C, D] |
| **2** | B | [C, D] | E, F | [C, D, E, F] |
| **3** | C | [D, E, F] | G, H, I | [D, E, F, G, H, I] |
| **4** | D | [E, F, G, H, I] | J | [E, F, G, H, I, J] |
| **5** | E | [F, G, H, I, J] | (None) | [F, G, H, I, J] |
| **6** | F | [G, H, I, J] | (None) | [G, H, I, J] |
| **7** | G | [H, I, J] | K, L | [H, I, J, K, L] |
| **8** | H | [I, J, K, L] | (None) | [I, J, K, L] |
| **9** | I | [J, K, L] | (None) | [J, K, L] |
| **10** | J | [K, L] | (None) | [K, L] |
| **11** | K | [L] | (None) | [L] |
| **12** | L | [] | (None) | [] |

---

## Requirements

* Python 3.x[cite: 1]
* Jupyter Notebook / JupyterLab[cite: 1]