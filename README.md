## Explanation

- **Read(arr):** Reads the array that needs to be sorted.
- **FOR i FROM 1 TO arr.length-1 STEP 1 DO:** Starts the loop from the second element of the array.
- **key := arr[i]:** Stores the current element in `key`.
- **j := i - 1:** Initializes `j` to point to the element before the current element.
- **WHILE (j >= 0 AND arr[j] > key) DO:** Checks if the previous element is greater than `key` and shifts it one position to the right.
- **arr[j + 1] := key:** Places `key` in its correct position.
- **Write(arr):** Outputs the sorted array.

## Example

Consider an array: [5, 2, 4, 6, 1, 3]

Steps:

1. Start with the second element (2). Compare with 5 and shift 5 to the right. Insert 2 in the first position.
   - Array: [2, 5, 4, 6, 1, 3]
2. Move to the third element (4). Compare with 5 and shift 5 to the right. Insert 4 in the second position.
   - Array: [2, 4, 5, 6, 1, 3]
3. Move to the fourth element (6). It is in the correct position.
   - Array: [2, 4, 5, 6, 1, 3]
4. Move to the fifth element (1). Compare with 6, 5, 4, and 2, shifting each to the right. Insert 1 in the first position.
   - Array: [1, 2, 4, 5, 6, 3]
5. Move to the sixth element (3). Compare with 6, 5, and 4, shifting each to the right. Insert 3 in the third position.
   - Array: [1, 2, 3, 4, 5, 6]

The sorted array is [1, 2, 3, 4, 5, 6].

## Advantages

- Simple to implement.
- Efficient for small datasets.
- Stable sort (maintains the relative order of equal elements).

## Disadvantages

- Not suitable for large datasets as its average and worst-case time complexity is O(n^2).

## Usage

Insertion sort is typically used for small datasets or as a part of more complex algorithms like Shell sort. It is also useful when the array is almost sorted since it can efficiently handle such cases.

<!-- or

# Insertion Sort Algorithm

## Description
Insertion Sort is a simple and efficient comparison-based sorting algorithm. It works similarly to sorting playing cards in your hands. The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.

## Algorithm
1. Iterate from the second element to the last element of the array.
2. For each element, compare it with the elements before it in the array.
3. Shift all the elements greater than the current element one position to the right.
4. Insert the current element into its correct position. -->

s
git branch -M main
