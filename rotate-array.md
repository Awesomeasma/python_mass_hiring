## The following code rotates arr[] by d elements. 
```
def rotate(arr,d): 
    # Store the first d elements in a temp array
    # Shift rest of the arr[]
    # Store back the d elements
    n = len(arr)
    i=arr.index(d)
    new_array=[]
    new_array=arr[i+1:]+arr[0:i+1]
    return new_array
   
d = 2
# d = index of element by which we should rotate.

print(rotate([1,2,3,4,5,6,7],d))
```
## Output:

4 5 6 7 1 2 3
### Time Complexity: O(n)
### Auxiliary Space: O(n)
