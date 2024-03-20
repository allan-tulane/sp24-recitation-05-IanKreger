# CMPS 2200 Reciation 5
## Answers

**Name:**__Ian Kreger_______________________


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**

|      n |   qsort-fixed-pivot |   qsort-random-pivot |   tim_sort time |
|--------|---------------------|----------------------|-----------------|
|    100 |               0.030 |                0.445 |           0.006 |
|    200 |               0.097 |                0.876 |           0.004 |
|    500 |               0.112 |                1.078 |           0.006 |
|   1000 |               0.198 |                3.126 |           0.013 |
|   2000 |               0.394 |               25.128 |           0.028 |
|   5000 |               1.364 |               52.362 |           0.058 |
|  10000 |               2.142 |              103.155 |           0.128 |
|  20000 |               4.333 |              306.779 |           0.386 |
|  50000 |              68.392 |              537.397 |           0.813 |
| 100000 |              60.021 |             1381.626 |           1.339 |




The asymptotic upper bounds of selection sort is O(n^2) and for quicksort it is O(nlogn). This alligns with the runtimes provided. The data shows that quicksort generally performs better when it has fixed permutations over random permutations. This is shown by the data above. As the list sizes increase the difference becomes much larger. Quicksort with fixed permutations is much more efficient with larger list sizes proportionaly to quicksort with random permutations. Selection sort tends to remain relatively stable across different inputs but tends to run slower overall. In general the size of the list affects selection sort much more than quick sort. 

- **1c.**
- 
When looking at the fastest quicksort variant and Python's timsort function we can assume that timsort could beat quicksort in efficiency for both sorted lists and random permutations. Timsort has the advantage inherently because of its hybrid structure and the ability to merge the strategies of merge sort and insertion sort. This allows timsort to perform very well with data that would appear in real-world scenarios. This design allows Timsort to utilize any sequences that already exists in the data and enhancing its only sorting efficiency. This makes it expected that timsort would show to perform very well with sorted or random data types. This means that timsort is better than quicksort because it works efficiently with random and fixed data sets while our quicksort works very slow with random permutations. This information is supported in the data that is in part b.
