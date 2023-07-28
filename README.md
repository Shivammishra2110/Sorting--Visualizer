# Sorting_Visualizer

A web application showcasing the inner workings of sorting algorithms.

Implemented algorithms:
1) Bubble sort
2) Selection sort
3) Insertion sort
4) Merge sort
5) Quick sort
6) Heap sort

Features:
1) Colored representation of step being executed.
  1.1) Blue: Default
  1.2) Yellow: Being compared
  1.3) Red: Identified as in incorrect position and to be moved
  1.4) Green: Incorrect position
2) 3 Controls for visualizations
  2.1) Speed of visualization (5-speed levels)
  2.2) Data size ()
  2.3) Generation of new data (Randomly generate new data).
4) Time and Space complexity of the algorithm being visualized.

Theory
**1) Bubble Sort:**

Bubble Sort is a simple sorting algorithm that repeatedly steps through the list to be sorted, compares adjacent elements, and swaps them if they are in the wrong order. The pass-through of the list is repeated until the entire list is sorted. The algorithm gets its name because more minor elements "bubble" to the top of the list while larger elements "sink" to the bottom.

- **Algorithm Steps:**
  1. Start from the first element and compare it with the next element.
  2. If the current element is greater than the next element, swap them.
  3. Move to the next pair of elements and repeat the above steps until the end of the list.
  4. Continue these steps for multiple passes until the list is fully sorted.

- **Time Complexity:**
  - Best Case: O(n) (when the list is already sorted)
  - Average Case: O(n^2)
  - Worst Case: O(n^2)

**2) Selection Sort:**

Selection Sort is another simple sorting algorithm that divides the input list into two parts: the sorted part and the unsorted part. It repeatedly selects the smallest (or largest, depending on the sorting order) element from the unsorted part and places it at the end of the sorted part until the entire list is sorted.

- **Algorithm Steps:**
  1. Find the minimum (or maximum) element in the unsorted part of the list.
  2. Swap the found element with the first element of the unsorted part.
  3. Move the boundary between the sorted and unsorted parts of one element to the right.
  4. Repeat the above steps until the entire list is sorted.

- **Time Complexity:**
  - Best Case: O(n^2)
  - Average Case: O(n^2)
  - Worst Case: O(n^2)

**3) Insertion Sort:**

Insertion Sort is a simple sorting algorithm that builds the final sorted list one element at a time. It starts by considering the first element as a sorted part and repeatedly inserts the next element from the unsorted part into its correct position in the sorted part until all elements are included in the sorted list.

- **Algorithm Steps:**
  1. Start with the second element (index 1) and compare it with the previous elements in the sorted part.
  2. If the current element is smaller (or larger, depending on the sorting order) than the compared element, move the compared element one position to the right.
  3. Repeat the above step until a proper position for the current element is found in the sorted part.
  4. Move the boundary between the sorted and unsorted parts of one element to the right.
  5. Repeat the above steps until the entire list is sorted.

- **Time Complexity:**
  - Best Case: O(n) (when the list is already sorted)
  - Average Case: O(n^2)
  - Worst Case: O(n^2)

**4) Merge Sort:**

Merge Sort is a divide-and-conquer sorting algorithm that divides the input list into smaller halves, sorts them recursively, and then merges them back together in the correct order to obtain the sorted list.

- **Algorithm Steps:**
  1. Divide the unsorted list into two halves.
  2. Recursively sort each half.
  3. Merge the two sorted halves by comparing elements from both halves and placing them in the correct order.
  4. Repeat the above steps until the entire list is sorted.

- **Time Complexity:**
  - Best Case: O(n log n)
  - Average Case: O(n log n)
  - Worst Case: O(n log n)

**5) Quick Sort:**

Quick Sort is also a divide-and-conquer sorting algorithm that selects a "pivot" element from the list and partitions the other elements into two sub-lists: components less than the pivot and features greater than the pivot. It then recursively sorts these sub-lists.

- **Algorithm Steps:**
  1. Choose a pivot element from the list.
  2. Partition the list into two sub-lists: elements less than the pivot and elements greater than the pivot.
  3. Recursively apply Quick Sort to the sub-lists.
  4. Concatenate the sorted sub-lists with the pivot to get the final list.

- **Time Complexity:**
  - Best Case: O(n log n)
  - Average Case: O(n log n)
  - Worst Case: O(n^2) (when the pivot selection is not optimal)

**6) Heap Sort:**

Heap Sort is a comparison-based sorting algorithm that uses a binary heap data structure to sort elements. It first converts the input list into a max-heap (for ascending order) or min-heap (for descending order), and then repeatedly extracts the root element from the heap to get the sorted list.

- **Algorithm Steps:**
  1. Build a max-heap (or min-heap) from the input list.
  2. Extract the root element (which is the maximum in the case of max-heap) and place it at the end of the sorted list.
  3. Re-heapify the remaining elements to maintain the heap property.
  4. Repeat the above steps until all elements are extracted and the list is sorted.

- **Time Complexity:**
  - Best Case: O(n log n)
  - Average Case: O(n log n)
  - Worst Case: O(n log n)

Heap Sort's time complexity is consistent across all cases due to its nature as a comparison-based sorting algorithm, and its primary performance bottleneck lies in building the initial heap, which takes O(n) time. However, it is important to note that the constant factors involved in the time complexity of Heap Sort are typically higher than other efficient sorting algorithms like Merge Sort or Quick Sort, which might make it slower in practice for smaller input sizes compared to those algorithms. Nonetheless, Heap Sort is still widely used in certain scenarios, especially when a stable sorting algorithm with guaranteed O(n log n) time complexity is required.
