## The following code outputs the first non repeating element in an array .
```
def firstNonRepeatingELement(nums):
  n = len(nums)
  for i in range(n):
    j = i
    while(j < n):
      if(nums[i] == nums[j] and i != j):
        break
      j += 1
    if(j == n):
      return nums[i]
# Driver code
nums = [9, 4, 9, 6, 7, 4]
print(firstNonRepeatingElement(nums))
```
## Output:

6
### Time Complexity: O(n*n)
### Auxiliary Space: O(1)
