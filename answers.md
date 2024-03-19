# CMPS 2200 Reciation 5
## Answers

**Name:**__Ian Kreger_______________________


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**
|        |      n |   qsort-fixed-pivot |   qsort-random-pivot |
|--------|--------|---------------------|----------------------|
|    100 |  0.067 |               0.438 |                0.006 |
|    200 |  0.082 |               0.479 |                0.004 |
|    500 |  0.149 |               1.410 |                0.007 |
|   1000 |  0.202 |               4.065 |                0.029 |
|   2000 |  0.931 |              64.753 |                0.028 |
|   5000 |  0.968 |              25.959 |                0.054 |
|  10000 |  2.001 |             167.691 |                0.169 |
|  20000 |  9.418 |             303.918 |                0.884 |
|  50000 | 18.360 |             707.959 |               52.316 |
| 100000 | 34.963 |            1463.445 |                2.135 |


The asymptotic upper bounds of selection sort is O(n^2) and for quicksort it is O(nlogn). This alligns with the runtimes provided. The data shows that quicksort generally performs better when it has random permutations over fixed permutations. This is shown by the data above. As the list sizes increase the difference becomes much larger. Quicksort with random permutations is much more efficient with larger list sizes proportionaly to quicksort with fixed permutations. Selection sort tends to remain relatively stable across different inputs but tends to run slower overall. In general the size of the list affects selection sort much more than quick sort. 

- **1c.**
When looking at the fastest quicksort variant and Python's timsort function we can assume that timsort could beat quicksort in efficienty for both sorted lists and random permutations. Timsort has the advantage inherently because of its hybrid structure and the ability to merge the strategies of merge sort and insertion sort. This allows timsort to perform very well with data that would appear in real-world scenarios. This design allows Timsort to utilize any sequences that already exists in the data and enhancing its only sorting efficiency. This makes it expected that timsort would show to perform very well with sorted or random data types. This means that timsort is better than quicksort because it works efficiently with random and fixed data sets while our quicksort works very slow with fixed permutations. 
