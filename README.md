# DataStrucs

This file contains notes about various Data Structures and the alorithms used to them. I learnt everything from an excellent book called "Grokking Algorithms" (https://www.manning.com/books/grokking-algorithms?gclid=Cj0KCQjwivbsBRDsARIsADyISJ95hy8r_5mac1eiFFX5V_f7Fqxod_Kw_bHOwp4hbFSUPd4i12kTMz4aAvsVEALw_wcB).

# Simple Search:
O(n)

# Binary Search:
• (log n) binary_search{low, high, guess}
• Binary search is a lot faster than simple search.
• O(log n) is faster than O(n), but it gets a lot faster once the list of items you’re searching through grows.
• Algorithm speed isn’t measured in seconds.
• Algorithm times are measured in terms of growth of an algorithm.
• Algorithm times are written in Big O notation.


# Arrays and Linked Lists:
• Your computer’s memory is like a giant set of drawers.
• When you want to store multiple elements, use an array or a list.
• With an array, all your elements are stored right next to each other.
• With a list, elements are strewn all over, and one element stores the address of the next one.
• Arrays allow fast reads.
• Linked lists allow fast inserts and deletes.
• All elements in the array should be the same type (all ints, all doubles, and so on).

# Selection Sort:
O(n-square) sort{findsmallest/findlargest{return index}}

# Recursion:
• Recursion is when a function calls itself.
• Every recursive function has two cases: the base case and the recursive case.
• A stack has two operations: push and pop.
• All function calls go onto the call stack.
• The call stack can get very large, which takes up a lot of memory.

# Divide and Conquer:
• Uses recursion.
• Binary search uses DC.
• Quicksort is based on DC.
• D&C works by breaking a problem down into smaller and smaller pieces. If you’re using D&C on a list, the base case will be an empty array or an array with one element.
• If you’re implementing quicksort, choose a random element as the pivot. The average runtime of quicksort is O(n log n)!
• The constant in Big O notation can matter sometimes. That’s why quicksort is faster than merge sort.
• The constant almost never matters for simple search versus binary search, because O(log n) is so much faster than O(n) when your list gets big.

# Quicksort:
• O(n log n) quicksort{pivot, less, great}

# Hash:
Hashes are good for - 
• Modeling relationships from one thing to another thing
• Filtering out duplicates
• Caching/memorizing data instead of making your server do work
• You can make a hash table by combining a hash function with an array.
• Collisions are bad. You need a hash function that minimizes collisions.
• Hash tables have really fast search, insert, and delete.
• Hash tables are good for modeling relationships from one item to another item.
• Once your load factor is greater than .07, it’s time to resize your hash table.
• Hash tables are used for caching data (for example, with a web server).
• Hash tables are great for catching duplicates.
