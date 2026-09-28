# Q3 Execution Details

## Input

```text
78 92 65 88 95 72 84 90
```

## Max Heap insertion

The scores are inserted one at a time. After each insertion, the new value is moved upward whenever it is greater than its parent.

Final Max Heap:

```text
95 92 84 90 88 65 72 78
```

## Maximum using Max Heap

The root contains the maximum value:

```text
95
```

## Maximum using Linear Search

The program scans the scores from left to right and updates the current maximum whenever a larger score is found.

Final maximum:

```text
95
```

Number of Linear Search comparisons:

```text
7
```
