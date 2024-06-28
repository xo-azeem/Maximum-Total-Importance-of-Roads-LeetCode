# Maximum Total Importance of Roads

LeetCode Q # 2285.

You are given an integer n denoting the number of cities in a country. The cities are numbered from 0 to n - 1.

You are also given a 2D integer array roads where roads[i] = [ai, bi] denotes that there exists a bidirectional road connecting cities ai and bi.

You need to assign each city with an integer value from 1 to n, where each value can only be used once. The importance of a road is then defined as the sum of the values of the two cities it connects.

Return the maximum total importance of all roads possible after assigning the values optimally.

Example 1:

<div align = "center">

  ![image](https://github.com/xo-azeem/Maximum-Total-Importance-of-Roads-LeetCode/assets/171427226/5a6411fd-6981-4249-bbb2-694d73a3bc96)
  
</div>

Input: n = 5, roads = [[0,1],[1,2],[2,3],[0,2],[1,3],[2,4]]</br>
Output: 43</br>
Explanation: The figure above shows the country and the assigned values of [2,4,5,3,1].</br>
- The road (0,1) has an importance of 2 + 4 = 6.</br>
- The road (1,2) has an importance of 4 + 5 = 9.</br>
- The road (2,3) has an importance of 5 + 3 = 8.</br>
- The road (0,2) has an importance of 2 + 5 = 7.</br>
- The road (1,3) has an importance of 4 + 3 = 7.</br>
- The road (2,4) has an importance of 5 + 1 = 6.</br>
The total importance of all roads is 6 + 9 + 8 + 7 + 7 + 6 = 43.</br>
It can be shown that we cannot obtain a greater total importance than 43.</br>

Example 2:

<div align = "center">

![image](https://github.com/xo-azeem/Maximum-Total-Importance-of-Roads-LeetCode/assets/171427226/2a1b2751-3486-42f2-b507-f95915ad543b)

</div>

Input: n = 5, roads = [[0,3],[2,4],[1,3]]</br>
Output: 20</br>
Explanation: The figure above shows the country and the assigned values of [4,3,2,5,1].</br>
- The road (0,3) has an importance of 4 + 5 = 9.</br>
- The road (2,4) has an importance of 2 + 1 = 3.</br>
- The road (1,3) has an importance of 3 + 5 = 8.</br>
The total importance of all roads is 9 + 3 + 8 = 20.</br>
It can be shown that we cannot obtain a greater total importance than 20.</br>

My Solution Analysis:

<div align = "center">

  ![image](https://github.com/xo-azeem/Maximum-Total-Importance-of-Roads-LeetCode/assets/171427226/f0bb5862-7ec6-4a8c-aad4-8241680e5f19)

  Time complexity: O(n log n).</br>Space complexity: O(n log n).
</div>
