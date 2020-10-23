# Sorting Algorithms

This folder contains various sorting algorithms used in programming for sorting and arranging data.
Understanding and learning to implement these algo's is an important skill to have for a programmer.

All these sorting algorithm are written in such a way that they are east to 
grasp and understand for a beginner level programmer

## Files

<!---------------------------------------------------------------------------------------------->
<!-- Insertion Sorting -->
<!---------------------------------------------------------------------------------------------->
<details>
<summary>1.<a href="https://github.com/aswnss-m/python_projects/blob/master/Sorting/insertion_sort.py">Insertion Sorting</a>
<br>
<b>Insertion Sort</b> is a simple sorting algorithm that works similar to the way you sort playing cards in your hands.</summary>
<br>The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.
Algorithm

To sort an array of size n in ascending order:
<ol>
  <ul> Iterate from arr[1] to arr[n] over the array. </ul>
  <ul> Compare the current element (key) to its predecessor.</ul>
<ul> If the key element is smaller than its predecessor, compare it to the elements before. Move the greater elements one position up to make space for the swapped element.</ul>
  </ol><br>

<img src="https://upload.wikimedia.org/wikipedia/commons/4/42/Insertion_sort.gif">

</details>
<!---------------------------------------------------------------------------------------------->
<!-- Selection Sorting -->
<!---------------------------------------------------------------------------------------------->
<details>
<summary>2.<a href="https://github.com/aswnss-m/python_projects/blob/master/Sorting/selection_sort.py">Selection Sorting</a>
<br>
<b>Selection Sort</b> is noted for its simplicity and has performance advantages over more complicated algorithms in certain situations, particularly where auxiliary memory is limited.</summary> <br>
The algorithm divides the input list into two parts: a sorted sublist of items which is built up from left to right at the front (left) of the list and a sublist of the remaining unsorted items that occupy the rest of the list. Initially, the sorted sublist is empty and the unsorted sublist is the entire input list. The algorithm proceeds by finding the smallest (or largest, depending on sorting order) element in the unsorted sublist, exchanging (swapping) it with the leftmost unsorted element (putting it in sorted order), and moving the sublist boundaries one element to the right.
  
Algorithm
<blockquote>
arr[] = 64 25 12 22 11

// Find the minimum element in arr[0...4]
// and place it at beginning
11 25 12 22 64

// Find the minimum element in arr[1...4]
// and place it at beginning of arr[1...4]
11 12 25 22 64

// Find the minimum element in arr[2...4]
// and place it at beginning of arr[2...4]
11 12 22 25 64

// Find the minimum element in arr[3...4]
// and place it at beginning of arr[3...4]
11 12 22 25 64 
</blockquote>
<br>
<img src= "https://upload.wikimedia.org/wikipedia/commons/9/94/Selection-Sort-Animation.gif" style="transform:rotate(-90deg)">
</details>
<details>
	<summary>
		3. <a href="https://github.com/aswnss-m/python_projects/blob/master/Sorting/bubble_sort.py">Bubble Sort</a>
		<br><b>Bubble Sort</b> is a simple sorting algorithm. This sorting algorithm is comparison-based algorithm in which each pair of adjacent elements is compared and the elements are swapped if they are not in order.
	</summary> <br>
	Bubble sort should be avoided in the case of large collections. It will not be efficient in the case of a reverse-ordered collection. 


<blockquote><br>
	
### Step-by-step example

Take an array of numbers " 5 1 4 2 8", and sort the array from lowest number to greatest number using bubble sort. In each step, elements written in bold are being compared. Three passes will be required;

First Pass 	
    ( 5 1 4 2 8 ) → ( 1 5 4 2 8 ), Here, algorithm compares the first two elements, and swaps since 5 > 1. <br>
    ( 1 5 4 2 8 ) → ( 1 4 5 2 8 ), Swap since 5 > 4 <br>
    ( 1 4 5 2 8 ) → ( 1 4 2 5 8 ), Swap since 5 > 2<br>
    ( 1 4 2 5 8 ) → ( 1 4 2 5 8 ), Now, since these elements are already in order (8 > 5), algorithm does not swap them.<br>
Second Pass<br>
    ( 1 4 2 5 8 ) → ( 1 4 2 5 8 )<br>
    ( 1 4 2 5 8 ) → ( 1 2 4 5 8 ), Swap since 4 > 2<br>
    ( 1 2 4 5 8 ) → ( 1 2 4 5 8 )<br>
    ( 1 2 4 5 8 ) → ( 1 2 4 5 8 )<br>

Now, the array is already sorted, but the algorithm does not know if it is completed. The algorithm needs one whole pass without any swap to know it is sorted.<br>

Third Pass<br>
    ( 1 2 4 5 8 ) → ( 1 2 4 5 8 )<br>
    ( 1 2 4 5 8 ) → ( 1 2 4 5 8 )<br>
    ( 1 2 4 5 8 ) → ( 1 2 4 5 8 )<br>
    ( 1 2 4 5 8 ) → ( 1 2 4 5 8 )<br>
</blockquote>
	<img src="https://upload.wikimedia.org/wikipedia/commons/c/c8/Bubble-sort-example-300px.gif">
</details>

<!---------------------------------------------------------------------------------------------->
<!-- Quick Sorting -->
<!---------------------------------------------------------------------------------------------->
<details>
  <summary>4.<a href="https://github.com/aswnss-m/python_projects/blob/master/Sorting/quick_sort.py">Quick Sort</a> <br>
  <b>Quick Sort</b> is a Divide and Conquer algorithm. It picks an element as pivot and partitions the given array around the picked pivot.
  There are many different versions of quickSort that pick pivot in different ways. </summary><br>
  The key process in quickSort is partition(). Target of partitions is, given an array and an element x of array as pivot, put x at its correct 
  position in sorted array and put all smaller elements (smaller than x) before x, and put all greater elements (greater than x) after x.
  All this should be done in linear time.

### Algorithm

  <blockquote>
  <ol>
  <li>Pick an element as a pivot</li>
  <li>Compare the other element with the pivot and partition the list</li>
  <li>Apply quick sort on the partiotioned lists</li>
  <li>Join all the partitions together</li>
  </ol>
  </blockquote>
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/Sorting_quicksort_anim.gif">

</details>

<!---------------------------------------------------------------------------------------------->
<!-- Merge Sorting -->
<!---------------------------------------------------------------------------------------------->
<details>
<summary>6.<a href = "https://github.com/Anjan50/Python/blob/main/Algorithms/Sorting%20Algorithms/MergeSort.py">Merge Sort</a><br>
<b>Merge Sort</b> is a Divide and Conquer algorithm. It divides input array in two halves, calls itself for the two halves and then merges the two sorted halves. 
</summary><br> 
The merge() function is used for merging two halves.The merge(arr, l, m, r) is key process that assumes that arr[l..m] and arr[m+1..r] are sorted and merges the two sorted sub-arrays into one. See following C implementation for details.

### Algorithm
<blockquote>
following C implementation for details.

MergeSort(arr[], l,  r) <br>
If r > l <br>
<ol>
     1. Find the middle point to divide the array into two halves:  <br>
             middle m = (l+r)/2 <br>
     2. Call mergeSort for first half:   <br>
             Call mergeSort(arr, l, m)<br>
     3. Call mergeSort for second half:<br>
             Call mergeSort(arr, m+1, r)<br>
     4. Merge the two halves sorted in step 2 and 3:<br>
             Call merge(arr, l, m, r)<br>
</blockquote>
<img src="https://upload.wikimedia.org/wikipedia/commons/c/cc/Merge-sort-example-300px.gif">
</details>