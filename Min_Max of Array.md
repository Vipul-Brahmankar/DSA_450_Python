# Max/Min of array

## Approach 1:
- set max to -inf and min to +inf
- compare each elem and update max and min
- return final max/min
- Time Complexity: O(N)  - Auxiliary Space: O(1)

```
def getMinMax(arr):
	mini, maxi = float('inf'), float('+inf')
	for i in arr:
		if i < mini:
			mini = i
		if i > maxi:
			maxi = i
	return (mini, maxi)

if __name__ == "__main__":
	arr = [4, 9, 6, 5, 2, 3]
	print(getMinMax(arr))
```

## Approach 2:
- if n==1: min = max = arr[0]
- elif arr[0]<arr[1]: min, max = arr[0], arr[1]
- else: min, max = arr[1], arr[0]
- if n>2:
- Time complexity: O(n log n) - Auxilary Space: is O(1)

```
def getMinMax(arr):
	arr.sort()
	mini, maxi = arr[0], arr[-1]
	return (mini, maxi)
```


## Approach 2 [Sorting]:
- sort arr
- min, max = arr[0], arr[-1]
- Time complexity: O(n log n) - Auxilary Space: is O(1)

```
def getMinMax(arr):
	arr.sort()
	mini, maxi = arr[0], arr[-1]
	return (mini, maxi)
```

