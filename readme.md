Array
=======

Two pointer
--------------
1. https://leetcode.com/problems/merge-sorted-array
2. https://leetcode.com/problems/product-of-two-run-length-encoded-arrays

Prefix Sum
--------------
1. https://leetcode.com/problems/buildings-with-an-ocean-view

Prefix Sum with Hashmap
--------------------------
1. https://leetcode.com/problems/subarray-sum-equals-k
2. https://leetcode.com/problems/continuous-subarray-sum/

Hashmap
----------
1. https://leetcode.com/problems/kth-missing-positive-number

Random Index
------------
Use 
```
Random random = new Random();
int randomIndex = ramdom.nextInt(list.size());
```
1. https://leetcode.com/problems/random-pick-index
2. https://leetcode.com/problems/random-pick-with-weight ( calculate prefx sum and apply Random on it and search using binary search)

Heap
----
1. https://leetcode.com/problems/k-closest-points-to-origin

Sliding window
--------------
1. https://leetcode.com/problems/max-consecutive-ones-iii

Next Permutation
----------------
Algo:
- Traverse from right to left and get first pivot where nums[i] < nums[i+1]. If not pivot exist return -1.
- If pivot != -1
  - Treverse right to left and get index of first greater element than pivot. (This will always exists)
  - Swap pivot and first greater element
- reverse array from pivot + 1 to end.
1. https://leetcode.com/problems/next-permutation

Binary Search
-------------
1. https://leetcode.com/problems/kth-missing-positive-number
