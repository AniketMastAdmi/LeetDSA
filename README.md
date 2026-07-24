# LeetCode Solutions

Total Solved: 5
Easy: 4
Medium: 1
Hard: 0

Languages
1class Solution:
2    def searchInsert(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low, high = 0, n-1 
5        lb = n 
6
7        while low <= high:
8            mid = (low + high) // 2
9            # lb = mid 
10            if nums[mid] >= target:
11                lb = mid
12                high = mid - 1
13            else:
14                low = mid + 1
15
16        return lb
17
Python
[0]
[2,0]
[0,0,0,1,1,1,2,2,2]
[2,2,2,0,0,0,1,1,1]
[2,2,1,1,0,0,0]
[2,1,2,2,2,2,0,0,0]
[2,2,2,2,2,1,0,0,1,1,0]
[2,2,2,1,1,0,0,1,0,1,0,2,1,0,2,1,0,2,1,1]

Last Updated
2026-07-24 18:20


## Solved Problems

| # | Title | Difficulty | Language | Synced At |
|---|---|---|---|---|
| 75 | [Sort Colors](https://github.com/AniketMastAdmi/LeetDSA/blob/main/LeetCode/Medium/0075_Sort_Colors/solution.txt) | Medium | [0]
[2,0]
[0,0,0,1,1,1,2,2,2]
[2,2,2,0,0,0,1,1,1]
[2,2,1,1,0,0,0]
[2,1,2,2,2,2,0,0,0]
[2,2,2,2,2,1,0,0,1,1,0]
[2,2,2,1,1,0,0,1,0,1,0,2,1,0,2,1,0,2,1,1] | 2026-07-24 |
| 21 | [Merge Two Sorted Lists](https://github.com/AniketMastAdmi/LeetDSA/blob/main/LeetCode/Easy/0021_Merge_Two_Sorted_Lists/solution.py) | Easy | Python | 2026-07-24 |
| 1 | [Two Sum](https://github.com/AniketMastAdmi/LeetDSA/blob/main/LeetCode/Easy/0001_Two_Sum/solution.py) | Easy | Python | 2026-07-24 |
| 13 | [Roman to Integer](https://github.com/AniketMastAdmi/LeetDSA/tree/main/LeetCode/Easy/0013_Roman_to_Integer) | Easy | Python | 2026-07-24 |
| 35 | [Search Insert Position](https://github.com/AniketMastAdmi/LeetDSA/tree/main/LeetCode/Easy/0035_Search_Insert_Position) | Easy | 1class Solution:
2    def searchInsert(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low, high = 0, n-1 
5        lb = n 
6
7        while low <= high:
8            mid = (low + high) // 2
9            # lb = mid 
10            if nums[mid] >= target:
11                lb = mid
12                high = mid - 1
13            else:
14                low = mid + 1
15
16        return lb
17 | 2026-07-24 |
