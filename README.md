# Quickselect in C and MIPS Assembly
Implementation of the quickselect algorithm, which finds the element at index k of an array without fully sorting it. The same algorithm is written twice, in C and in MIPS assembly, so the two versions can be compared line by line.

## How It Works 

Quickselect is a variation of quicksort. It picks a pivot, partitions the array around it, and then recurses into only one side, the one that contains index k.

**1.** partition(f, l) uses v[l] as the pivot (Lomuto scheme). Elements smaller than the pivot are moved to the left, and the pivot is placed in its final position p.

**2.** If p == k, the answer is v[p].

**3.** If k < p, continue on the left part [f, p-1].

**4.** Otherwise, continue on the right part [p+1, l].

Average time complexity is O(n), worst case O(n²).


Project for the ***Computer Organization course***, Department of Electrical & Computer Engineering (THMMY), Aristotle University of Thessaloniki.
