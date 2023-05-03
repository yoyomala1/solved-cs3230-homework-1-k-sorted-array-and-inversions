Download Link: https://assignmentchef.com/product/solved-cs3230-homework-1-k-sorted-array-and-inversions
<br>
<h1>1         K-Sorted Array</h1>

We say that an array of distinct integers <em>A</em>[1<em>..n</em>] is <em>k</em>-sorted if for each 1 ≤ <em>i </em>≤ <em>n</em>, the i’th smallest element is in positions <em>A</em>[1]<em>,…,A</em>[<em>i </em>+ <em>k</em>]. Given below is the pseudocode for sorting a <em>k</em>-sorted array using heap as an auxilary data structure.

<strong>Algorithm 1: </strong>Sort K-sorted array

<strong>Input: </strong>A <em>k</em>-sorted array <em>A</em>[1<em>,…,n</em>]<em>,k</em>

<strong>Output: </strong>Sorted array of A

<strong>1 </strong>Initialize array B[1,…,n]

1

Algorithm 1 uses two auxilary data structures, array <em>B </em>and heap <em>S</em>. It puts <em>k </em>+ 1 elements in heap and extracts minimum from the heap iteratively while adding a new element from array A into the heap. We want to prove correctness of the algorithm from this intuition: <em>given that first t elements in array B are in their ”correct” place, then t </em>+ 1<em><sup>th </sup>element must also be “correct”.</em>

Work through the following questions to show that this algorithm correctly sorts the array.

<h2>1.1</h2>

Make a statement, capturing the above intuition, on the value extracted from heap at line 6.

<strong>1.2</strong>

Prove the statement you made in 1<em>.</em>1

<h2>1.3</h2>

Now using induction on elements of array B, prove the correctness of the algorithm.

<h1>2         Inversions</h1>

Let <em>A</em>[1<em>…n</em>] be an array of <em>n </em>distinct numbers. If <em>i &lt; j </em>and <em>A</em>[<em>i</em>] <em>&gt; A</em>[<em>j</em>], then the pair (i, j) is called an inversion of A.

<strong>2.1</strong>

List the five inversions of the array h2<em>,</em>3<em>,</em>8<em>,</em>6<em>,</em>1i

<h2>2.2</h2>

What array with elements from the set {1, 2, …, n} has the most inversions? How many does it have?

<h2>2.3</h2>

Give an algorithm that determines the number of inversions in any permutation on n elements in Θ(<em>n</em>log<em>n</em>) worst-case time. (Hint: Modify merge sort.)