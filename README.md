# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

1) Constant factors and Lower Order Terms: asymptotic analysis ignores constant factores and lower order terms which can dominate performance for smaller input sizes.  For example, an algorithm with O(n) complexity might perform worse than an O(n^2) algorithm for certain input sizes due to larfe constrants or inefficient operations
2) Harware and System Overheads: Practical performance is influenced by factors like CPU chaching, memory latency, and I/O bottlenecks.  An algorithm that appears efficient asumptotically might suffer in practice due to poor cache locality or high memory access times.
3) Input Specific Behavior: asymptotic complexity assumes the worst case, average case, or best case without considering specific input characteristics.  For example a binary search tree may not be balanced, leading to worse than expected performance.

The asymptotic complexity of searching in a binary search tree is O(log n).  For 1000 elements this corresponds to apporoximatley log(base 2)1000 which equals about 10 levels, and for 10,000 elements, log(base2)10,000 equals about 14 levels.  Assuming the time scales proportionally the search time for 10,000 elements would be roughly 5 * (14/10) = 7 seconds.

The reasons that there might be discrepancy between predicted and measured time:
1) Unbalanced Tree Structure: if the binary search tree is not balance, the depth of the tree could approach O(n) instead of O(log n) leading to significantly higher search times.
2) System Resource Constraints: With a Larger tree, increased memory usage could lead to cache misses or higher memory access times degrading performance.  If the treee no longer fits the CPU cache, the search could be slowed by frequent memory fetches.
3) Implementation Overheads: Practical factors such as inefficient implementation, recursive function overhead, or additional operations during traversal could add signigicant time beyond the theoretical O(log n) expectation.

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."
