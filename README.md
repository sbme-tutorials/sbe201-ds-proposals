# \[SBE201\] Final Project Proposals

Groups that didn't yet decide an idea for their final project are suggested one of the ideas in this file.

* Each proposed idea can be selected by two groups at most.
* For some proposals, after selection, you may need to ask the TA for further information.
* Cheating and copying external codes is the easiest way to guarantee zero grade for the project, for the whole team.
* You are encouraged to use *CMake* script to define your project structure and let it carry out building your programs.

| Project | Group(s) |
|----------|----------|
| Pattern Matching | |
| Huffman Coding | |
| Bloxorz Hacking | |
| Sequence Alignments | |


## P1. Patterns Matching in Linear Space and Query Time

Make a survey over these algorithms and report their time and space complexity:

* Trie,
* Suffix Tree,
* Suffix Array,
* and Burrows-Wheeler-Transform (BWT)

Implement the most efficient algorithm in your project.

### Resources

* [Finding Mutations in DNA and Proteins (Bioinformatics VI) \| Coursera](https://www.coursera.org/learn/dna-mutations).
* [Fast String Searching With Suffix Trees](http://marknelson.us/1996/08/01/suffix-trees/)
* Some related materials are available from with the TA.

## P2. Huffman Compression Algorithm

In this project, you are required to implement a Huffman compression algorithm. You need to compile to programs: one for compressing an input file, and another one to decompress an input compressed file.

What you will learn:

* Gain more intuition on how compression programs work.
* Huffman as a binary tree data structure.
* Greedy Algorithms.
* Probability and Entropy.
* Reading and writing to files in C++.

### Resources

* [Huffman Code \| Brilliant](https://brilliant.org/wiki/huffman-encoding/)
* [Huffman Coding - Greedy Algorithm](https://www.youtube.com/watch?v=dM6us854Jk0)
* [Huffman Algorithm \(1/3\) \[كود مصري\]](https://www.youtube.com/watch?v=eP3FzXc1K3g)
* [Huffman Algorithm \(2/3\) \[كود مصري\]](https://www.youtube.com/watch?v=LplgowaCY4c)
* [Huffman Algorithm \(3/3\) \[كود مصري\]](https://www.youtube.com/watch?v=Y5SWDAIZ0sQ)

## P3. Solve Bloxorz Game

> This task is inspired by [Scala Specialization \| Coursera](https://www.coursera.org/specializations/scala)

In this project, you are required to hack [Bloxorz Game](http://www.coolmath-games.com/0-bloxorz). Take your time playing this game (e.g until level 10) to have an intuition how you can implement an algorithm that solves this game. Your goal in each level is to navigate your rectangular block to the target hole by using four movements: left, right, up, and down. You are also scored higher when you get the solution with fewer steps.

Your program are given a simplified version of some levels (without orange tiles, circles, or crosses), then you need to output the sequence of steps (i.e movements) that will obtain the correct solution.

### State-space Exploration

* We start at some initial state *S*, and we are trying to reach an end state *T*.
* From every state, there are possible transitions to other states, some of which are out of bounds.
* We explore the states, starting from *S*. by exploring its neighbors and following the chain, until we reach *T*. There are different ways of exploring the state space. On the two ends of the spectrum are the following techniques:
    
    * **depth-first search** : when we see a new state, we immediately explore its direct neighbors, and we do this all the way down, until we reach a roadblock. Then we backtrack until the first non-explored neighbor, and continue in the same vein.
    * **breadth-first search** : here, we proceed more cautiously. When we find the neighbors of our current state, we explore each of them for each step. The respective neighbors of these states are then stored to be explored at a later time.

What you will learn:

* How to transform game problem into tree search problem.
* Using queues (ADT) during **breadth-first** search.
* Using sets (ADT) to avoid visiting the same state.

## P4. DNA Sequence Alignment

In this project, you are required to implement an algorithm that finds the optimal alignment between two DNA sequences.


What you will learn:

* Dynamic Programming Algorithms.
* Directed Acyclic Graphs.
* Files Input/Output in C++.

### Resources

* [Comparing Genes, Proteins, and Genomes (Bioinformatics III) \| Coursera](https://www.coursera.org/learn/comparing-genomes), week 1 \& week 2.