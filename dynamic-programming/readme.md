Dynamic Programming patterns
============================

Fibonacci numbers (1D)
-----------------
1. https://leetcode.com/problems/climbing-stairs/
2. https://leetcode.com/problems/min-cost-climbing-stairs/
3. https://leetcode.com/problems/house-robber/
4. https://leetcode.com/problems/house-robber-ii/

0/1 Knapsack problems (2D)
---------------------

**Hint to identify problem** : we either pick the item or dont pick the item.
- if item is greater than given sum, we cant pick the item.
- If item is equal to or less than the given sum, we can either pick the item or dont pick the item.

**Return number of ways/ Check if subset is present in arrays which sums up to given sum/ difference equal to given diff**
1. Subset sum
2. Count number of subset sums 
3. Count the number of subset with given difference
4. https://leetcode.com/problems/target-sum/

**Partition an array to 2 partitions and get 0 (equal partitions) / min difference,** 
5. https://leetcode.com/problems/partition-equal-subset-sum/
6. Minimum subset sum difference


Unbounded Knapsack problems (2D)
---------------------------
1. https://leetcode.com/problems/coin-change/
2. https://leetcode.com/problems/coin-change-2/
3. https://leetcode.com/problems/minimum-cost-for-tickets/

Longest Common subsequence (2D)
--------------------------
1. https://leetcode.com/problems/longest-common-subsequence/
2. https://leetcode.com/problems/longest-increasing-subsequence/
3. https://leetcode.com/problems/edit-distance/
4. https://leetcode.com/problems/distinct-subsequences/

Palindrome
----------
Trick - expand palindrome for O(1) time
1. https://leetcode.com/problems/longest-palindromic-substring/
2. https://leetcode.com/problems/palindromic-substrings/
3. https://leetcode.com/problems/longest-palindromic-subsequence/


**Note :** 
For 2D patterns, and bottom up approach, top left corner is the target.

For all DP problems follow below sequence,
1. First come up with recursion by identifying base condition and main condition using choise tree.
2. Memoize the recursion approach and come up with top down approach.
3. Convert memoization to bottom uo DP.