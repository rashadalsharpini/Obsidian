![[ArcoLinux-2024-03-09-1710000227_screenshot_1920x1080 1.jpg]]![[ArcoLinux-2024-03-09-1710000259_screenshot_1920x1080 1.jpg]]

---


```c
quickSort(arr, low, high) 
	if low < high pivotIndex <- partition(arr, low, high)
	 quickSort(arr, low, pivotIndex - 1) // Sort left subarray 
	 quickSort(arr, pivotIndex + 1, high) // Sort right subarray 
	 partition(arr, low, high) 
		 pivot <- arr[high] 
		 i <- low - 1 
	for j in low to high-1 
		 if arr[j] <= pivot 
			 i <- i + 1 
			 swap(arr[i], arr[j])
	 swap(arr[i + 1], arr[high]) 
	 return i + 1 // Return the final position of the pivotelement
```
