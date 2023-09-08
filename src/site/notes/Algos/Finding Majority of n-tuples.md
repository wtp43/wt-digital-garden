---
{"dg-publish":true,"permalink":"/algos/finding-majority-of-n-tuples/","title":"Finding Majority of n tuples"}
---


>[!summary]+ Contents
>```toc
style: number
min_depth:1
max_depth:6 
>```


# Finding Majority of n-tuples
[[Algos/Boyer-Moore Voting Algorithm\|Boyer-Moore Voting Algorithm]] or using a dictionary
# Dictionary Implementation

```python
def majority(L): count = {}
	for word in L:
		if word in count:
			count[word] += 1 
		else:
	        count[word] = 1
# Using min() like this gives the first word with
# maximal count "for free"
val_1st_max, arg_1st_max = min((-count[word], word) for word in count) 
return arg_1st_max

```

## Optimizations

## Optimized Complexity

>[!Time Complexity]+
>O($n^2k$)
>The average complexity is O($nk$) but O($n^2k$) because of the use of a dictionary. In the worst case, your hash map will degenerate into a linked list and you will suffer an O(N) penalty for lookups, as well as inserts and deletions, both of which require a lookup operation.

>[!Space Complexity]+
>O(n)

# Related
[[Algos/Boyer-Moore Voting Algorithm\|Boyer-Moore Voting Algorithm]]