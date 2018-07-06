# C-Plus-Plus-Basic-DS-Problems

## Table of contents
* [Algorithms](#algo)
* [Time complexity](#time-complexity)
   * [Big O](#big-o)

## <a name="algo"></a> Algorithms

- [Insertion sort](/algo/insertion_sort.h)

## <a name="time-complexity"></a> Time complexity
Time complexity is a way of measuring how long an algorithm takes to run.

It's important to consider how long an algorithm takes to run. A poorly written algorithm could take tens of thousands of times longer to finish than a well written algorithm.

But measuring the running time of an algorithm can be tricky.

We can't measure an algorithm absolutely (i.e. in milliseconds), because the amount of time it takes will vary between hardware and between runs. An algorithm could take 1200ms to complete on my machine, and 4000ms on a slow computer.

Instead, we measure the *relative* running time.

To do this, we count the number of operations performed in the algorithm.

The most common way to express time complexity is with big O notation.

### <a name="big-o"></a> Big O notation

Big O notation measures the relative time an algorithm takes to run given the worst case.

Big O only cares about the big operations.

Generally we only care about the rough running time, so constant actions aren't included in the calculation.

Here's a table to use as a reference when looking through the algorithms in this project:

Big-O | Name | Description
------| ---- | -----------
**O(1)** | constant | **This is the best.**
**O(log n)** | logarithmic | **Pretty great.**
**O(n)** | linear | **Good performance.**
**O(n log n)** | "linearithmic" | **Decent performance.**
**O(n^2)** | quadratic | **Kinda slow.**
**O(n^3)** | cubic | **Poor performance.**
**O(2^n)** | exponential | **Very poor performance.**
**O(n!)** | factorial | **Intolerably slow.**