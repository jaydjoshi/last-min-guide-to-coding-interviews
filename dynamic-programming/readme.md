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

**Bottom up DP**
```
if(text1.charAt(i-1) == text2.charAt(j-1)){
    dp[i][j] = 1 + dp[i-1][j-1];
}else{
    dp[i][j] = Math.max(dp[i][j-1], dp[i-1][j]);
}
```

**Recursion / Top Down Memoization**
```
if(text1.charAt(m-1) == text2.charAt(n-1)){
    return 1 + lcs(text1, text2, m-1, n-1);
}else{
    return Math.max( lcs(text1, text2, m-1, n), lcs(text1, text2, m, n-1));
}
```
**Subsequence**
1. https://leetcode.com/problems/longest-common-subsequence/
2. https://www.geeksforgeeks.org/printing-longest-common-subsequence/
3. https://www.geeksforgeeks.org/minimum-number-deletions-insertions-transform-one-string-another/
4. https://www.geeksforgeeks.org/given-two-strings-find-first-string-subsequence-second/ ( DP is not optimal choice for this)
5. https://www.geeksforgeeks.org/find-length-longest-subsequence-one-string-substring-another-string/ (pending)
6. https://leetcode.com/discuss/general-discussion/1276555/find-number-of-times-a-string-occurs-as-a-subsequence-in-given-string (pending)
7. https://leetcode.com/problems/edit-distance/
8. https://leetcode.com/problems/distinct-subsequences/

**Substring**
1. https://leetcode.com/discuss/interview-question/1273766/longest-common-substring
https://www.geeksforgeeks.org/longest-common-substring-dp-29/
2. https://www.geeksforgeeks.org/print-longest-common-substring/

**Supersequence**
1. https://leetcode.com/problems/shortest-common-supersequence/
2. https://leetcode.com/problems/shortest-common-supersequence/discuss/1274116/printing-scs-shortest-common-supersequence

**Repeating sequence**
1. https://leetcode.com/discuss/general-discussion/1274765/longest-repeated-subsequence-lrs
   https://www.geeksforgeeks.org/longest-repeating-subsequence/

**Palindrome**
1. https://leetcode.com/problems/longest-palindromic-subsequence/
2. https://leetcode.com/problems/longest-palindromic-substring/
3. https://www.geeksforgeeks.org/count-palindrome-sub-strings-string/ (pending)
   https://leetcode.com/problems/count-different-palindromic-subsequences/ (pending)
4. https://www.geeksforgeeks.org/minimum-number-deletions-make-string-palindrome/
5. https://leetcode.com/problems/minimum-insertion-steps-to-make-a-string-palindrome/

**Increasing subsequence**
1. https://leetcode.com/problems/longest-increasing-subsequence/ 

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