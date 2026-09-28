# Q3 Final Conclusion

The given student scores are:

78, 92, 65, 88, 95, 72, 84, 90

Both Max Heap and Linear Search find the highest score as **95**.

The Max Heap stores the highest score at the root. Therefore, the maximum can be obtained in O(1) time after the heap has been maintained. Insertion into the heap takes O(log n) in the worst case.

Linear Search checks the scores one by one. For 8 scores, it requires 7 comparisons to find the maximum, giving O(n) time.

Therefore, when student scores are continuously inserted and the highest score needs to be maintained and accessed repeatedly, the Max Heap representation is suitable because the current maximum is always available at the root.
