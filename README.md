# Algorithms in Computational Biology (INFO-F438)

This repository contains the solution notebooks for the assignments of the INFO-F438 Algorithms in Computational Biology course..

## Course Content

Overview of typical computational issues in biology and their algorithmic solutions, including problems on graphs, pattern matching, sequence alignment using dynamic programming, and NP-hard optimization problems.

## Objectives

Students will learn different algorithm design paradigms as they apply to computational biology and be able to apply them to efficiently solve a variety of problems. The course also includes a project where students will present a recent research article.

## Repository Structure

The work is divided into three main Jupyter Notebooks, each corresponding to a specific assignment.

### Assignment 1: Optimal Protein Folding in the HP Model
This assignment focuses on the hydrophobic-hydrophilic (HP) model for protein folding. The goal is to maximize the number of adjacent, non-covalent H-H pairs on a 2D square grid.

* **Core Tasks:** Implementation of `bestfold(S)`, a brute-force recursive function to find optimal foldings.
* **Optimization:** Implementation of `bestfold2(S)` using a branch-and-bound technique and greedy heuristics to prune the recursion tree.
* **Analysis:** Runtime plotting to determine the largest string length solvable within a minute.

### Assignment 2: Closest Duplicate
This notebook addresses string processing efficiency. The objective is to build a class structure capable of quickly identifying substring locations and finding the closest pair of duplicates within a large string.

* **Implementation:** A suffix tree-based approach (Class `ST`) designed to optimize the `locations` and `closest` methods.
* **Performance:** Detailed runtime analysis and plotting using `timeit` to demonstrate complexity relative to string size ($N$) and substring length ($k$).

### Assignment 3: Variations on the Longest Common Subsequence
This assignment explores sequence alignment through a variation called the Minimum Length Match LCS (MLMLCS). Unlike the standard LCS, this version filters "noise" by requiring that matches consist of substrings of at least length $k$.

* **Core Tasks:** Coding the `MLMLCS` function and visualizing how the resulting subsequence aligns with the source strings
* **Analysis:** Worst-case runtime and space usage analysis in terms of string lengths and the parameter $k$

## Requirements

To run the notebooks in this repository, you will need a standard Python environment with the following dependencies:

* Python 
* Jupyter Notebook
* Matplotlib (for runtime plots)
* Timeit (for performance measurement) 
