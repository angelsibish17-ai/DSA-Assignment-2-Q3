# Assignment 2 – Question 3
## Max Heap and Linear Search for Student Scores

### Given data
78, 92, 65, 88, 95, 72, 84, 90

## 1. Max Heap
A Max Heap keeps the largest element at the root. The given scores were inserted one by one and the heap was adjusted upward whenever a newly inserted score was greater than its parent.

Final heap:
95, 92, 84, 90, 88, 65, 72, 78

Maximum score = 95.

## 2. Linear Search
Linear Search examines the scores from left to right and maintains the largest value found so far.

Comparisons for 8 scores = 7.
Maximum score = 95.

## 3. Execution comparison

| Operation | Max Heap | Linear Search |
|---|---|---|
| Find maximum | O(1), maximum is at root | O(n) |
| Insert a new score | O(log n) | O(1) if simply appended to an unsorted list |
| Maintain highest score continuously | Efficient because root stores maximum | Requires scanning all scores to find maximum |
| Extra structure | Heap array | No special structure |
| Space | O(n) | O(n) for the stored data |

For the given 8 scores, Max Heap identifies 95 from the root, while Linear Search performs 7 comparisons.

## 4. Effect of increasing number of students
As the number of students increases, Linear Search needs to examine the scores to find the maximum, so its maximum-finding time grows linearly, O(n). A Max Heap keeps the maximum at the root, so finding the maximum is O(1). Insertion into the Max Heap takes O(log n) in the worst case because the new element may move upward through the heap.

## 5. Conclusion
For a system that continuously maintains student scores and frequently needs the highest score, a Max Heap is suitable because the highest score is always available at the root and new scores can be inserted in O(log n) time.

For a one-time maximum search on an existing unsorted list, Linear Search is simpler and requires no heap construction.

## 6. Files included
- max_heap_linear_search.c – C source code
- input.txt – given input
- output.txt – execution output
- trace_table.md – insertion and search traces
- analysis.md – complexity and comparison
