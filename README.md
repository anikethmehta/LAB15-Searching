### ***Title*** : LAB12
### ***Aim*** :

(1) Linear search

(2) Binary search

### ***Algorithm*** :

Linear Search Algorithm:

Input: An array arr of size n and a target element target.

Output: The index of the target element in the array if found, or -1 if not found.

Start at the first element of the array (index 0).

Repeat the following steps for each element in the array, starting from index 0 and moving to the end of the array.

a. Check if the current element is equal to the target element.

b. If the current element is equal to the target, return the index of the current element.

If the loop completes without finding the target, return -1 to indicate that the target element is not in the array.

Binary Search Algorithm:

Input: A sorted array arr of size n and a target element target.

Output: The index of the target element in the array if found, or -1 if not found.

Initialize two pointers, left and right, to the first and last indices of the array, respectively.

While left is less than or equal to right, do the following:

a. Calculate the middle index mid as (left + right) / 2.

b. If the element at mid is equal to the target, return mid.

c. If the element at mid is less than the target, update left to mid + 1 to search the right half.

d. If the element at mid is greater than the target, update right to mid - 1 to search the left half.

If the loop completes without finding the target, return -1 to indicate that the target element is not in the array.

These algorithms provide two different methods for searching for an element in an array. Linear search is straightforward but less efficient, especially for large arrays. Binary search, on the other hand, is highly efficient for sorted arrays, as it reduces the search space by half at each step, making it much faster for large datasets.

### ***Explanation*** :

Linear search explanation:

The linearSearch function takes an array arr, its size size, and a target element target as arguments.

It iterates through the array using a for loop, checking each element to see if it matches the target.

If it finds the target element, it returns the index at which it was found. If the target element is not found, it returns -1.

In the main function, we call linearSearch to search for the target element in the array and print the result.

Binary search explanation:

The binarySearch function takes a sorted array arr, its size size, and a target element target as arguments.

It maintains two pointers, left and right, which define the search interval.

The function repeatedly calculates the mid index and checks if the element at mid matches the target.

If the element is found, it returns the index. If not, it adjusts the left and right pointers to search the appropriate half of the array.

The search continues until the target is found or the interval is empty, in which case it returns -1.

### ***Output Screenshot*** :

Code:

https://github.com/anikethmehta/LAB12/blob/main/code1.png

https://github.com/anikethmehta/LAB12/blob/main/code2.png

https://github.com/anikethmehta/LAB12/blob/main/code1_Bin.png
