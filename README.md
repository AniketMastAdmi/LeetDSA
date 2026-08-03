# LeetCode Solutions

Total Solved: 7
Easy: 4
Medium: 3
Hard: 0

Languages
1class Solution:
2    def search(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low,high = 0, n - 1
5        
6
7        while low <= high:
8            mid = (low + high) // 2 
9            if nums[mid] == target:
10                return mid 
11            if nums[mid] <= nums[high]:
12                if nums[mid] <= target <= nums[high]:
13                    low = mid + 1
14                else:
15                    high = mid - 1
16
17            else:
18                if nums[low] <= target <= nums[mid]:
19                    high = mid - 1
20                else:
21                    low = mid + 1 
22        return -1
23
24
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
for(int i = 0; i<nums.size(); i++)
    {
        if(nums[i] == target)
            return 1;
    }
    return 0;

Last Updated
2026-08-03 06:32


## Solved Problems

| # | Title | Difficulty | Language | Synced At |
|---|---|---|---|---|
| 81 | [Search in Rotated Sorted Array II](https://github.com/AniketMastAdmi/LeetDSA/blob/main/LeetCode/Medium/0081_Search_in_Rotated_Sorted_Array_II/solution.txt) | Medium | for(int i = 0; i<nums.size(); i++)
    {
        if(nums[i] == target)
            return 1;
    }
    return 0; | 2026-08-03 |
| 33 | [Search in Rotated Sorted Array](https://github.com/AniketMastAdmi/LeetDSA/tree/main/LeetCode/Medium/0033_Search_in_Rotated_Sorted_Array) | Medium | 1class Solution:
2    def search(self, nums: List[int], target: int) -> int:
3        n = len(nums)
4        low,high = 0, n - 1
5        
6
7        while low <= high:
8            mid = (low + high) // 2 
9            if nums[mid] == target:
10                return mid 
11            if nums[mid] <= nums[high]:
12                if nums[mid] <= target <= nums[high]:
13                    low = mid + 1
14                else:
15                    high = mid - 1
16
17            else:
18                if nums[low] <= target <= nums[mid]:
19                    high = mid - 1
20                else:
21                    low = mid + 1 
22        return -1
23
24 | 2026-08-01 |
| 75 | [Sort Colors](https://github.com/AniketMastAdmi/LeetDSA/tree/main/LeetCode/Medium/0075_Sort_Colors) | Medium | [0]
[2,0]
[0,0,0,1,1,1,2,2,2]
[2,2,2,0,0,0,1,1,1]
[2,2,1,1,0,0,0]
[2,1,2,2,2,2,0,0,0]
[2,2,2,2,2,1,0,0,1,1,0]
[2,2,2,1,1,0,0,1,0,1,0,2,1,0,2,1,0,2,1,1] | 2026-07-24 |
| 21 | [Merge Two Sorted Lists](https://github.com/AniketMastAdmi/LeetDSA/blob/main/LeetCode/Easy/0021_Merge_Two_Sorted_Lists/solution.py) | Easy | Python | 2026-07-24 |
| 1 | [Two Sum](https://github.com/AniketMastAdmi/LeetDSA/tree/main/LeetCode/Easy/0001_Two_Sum) | Easy | Python | 2026-07-24 |
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
