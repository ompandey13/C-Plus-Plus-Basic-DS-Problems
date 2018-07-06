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
**O(1)** | constant | **This is the best.** The algorithm always takes the same amount of time, regardless of how much data there is. Example: looking up an element of an array by its index.
**O(log n)** | logarithmic | **Pretty great.** These kinds of algorithms halve the amount of data with each iteration. If you have 100 items, it takes about 7 steps to find the answer. With 1,000 items, it takes 10 steps. And 1,000,000 items only take 20 steps. This is super fast even for large amounts of data. Example: binary search.
**O(n)** | linear | **Good performance.** If you have 100 items, this does 100 units of work. Doubling the number of items makes the algorithm take exactly twice as long (200 units of work). Example: sequential search.
**O(n log n)** | "linearithmic" | **Decent performance.** This is slightly worse than linear but not too bad. Example: the fastest general-purpose sorting algorithms.
**O(n^2)** | quadratic | **Kinda slow.** If you have 100 items, this does 100^2 = 10,000 units of work. Doubling the number of items makes it four times slower (because 2 squared equals 4). Example: algorithms using nested loops, such as insertion sort.
**O(n^3)** | cubic | **Poor performance.** If you have 100 items, this does 100^3 = 1,000,000 units of work. Doubling the input size makes it eight times slower. Example: matrix multiplication.
**O(2^n)** | exponential | **Very poor performance.** You want to avoid these kinds of algorithms, but sometimes you have no choice. Adding just one bit to the input doubles the running time. Example: traveling salesperson problem.
**O(n!)** | factorial | **Intolerably slow.** It literally takes a million years to do anything.