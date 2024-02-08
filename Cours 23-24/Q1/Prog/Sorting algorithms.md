
# Bubble

```python
def bubblesort(arr):
	n = len(arr)
	swapped = False
	for i in range(n-1):
	
		for j in range(0, n-i-1):
			if arr[j] > arr[j+1]:
				swapped = True
				arr[j], arr[j+1] = arr[j+1], arr[j]
				
		if not swapped:
			return

arr = [64,34,25,12,22,11,90]
bubblesort(arr)

print("sorted array is:")
for i in range(len(arr)):
	print("% d" % arr[i], end=" ")

```

# Tri par insertion

```python
def insertionSort:
	n = len(arr)

	if n <= 1:
		return

	for i in range(1,n):
		key = arr[i]
		j = i-1
		while j >= 0 and key < arr[j]:
			arr[j+1] = arr[j]
			j -= 1
		arr[j+1] = key

arr = [12,11,13,5,6]
insertionSort(arr)
print(arr)

```


# Tri par fusion

```python
def merge(arr, l, m, r)
	n1 = m-l+1
	n2 = r-m

	# L pour left et R pour right du sub-array

	# Temporary arrays:
	L = [0]*(n1)
	R = [0]*(n2)
	# Data to temp arrays:
	for i in range(0, n1):
		L[i] = arr[l+i]
	for j in range(0, n2):
		R[j] = arr[m+1+j]

	# Merge back
	i = 0
	j = 0
	k = l 

	while i < n1:
		arr[k] = L[i]
		i += 1
		k += 1

	while j < n2:
		arr[k] = R[j]
		j += 1
		k += 1
		

def fusion(arr, l, r):
	if l < r:
		m = l+(r-l)//2
		
		fusion(arr, l, m)
		fusion(arr, m+1, r)
		merge(arr, l, m, r)

arr = [10,11,13,5,6,7]
n = len(arr)

print("Given array is: ")
for i in range(n):
	print("%d" % arr[i],end=" ")

fusion(arr, 0, n-1)
print("\nSorted array is: ")
for i in range(n):
	print("%d" % arr[i], end=" ")
```


