---
{"dg-publish":true,"permalink":"/algos/backtracking/","title":"Backtracking","tags":["backtracking"]}
---


>[!summary]+ Contents
>```toc
style: number
min_depth:1
max_depth:6 
>```


# Backtracking

# Implementation

```python
def backtrack(candidate):
    if find_solution(candidate):
        output(candidate)
        return
    
    # iterate all possible candidates.
    for next_candidate in list_of_candidates:
        if is_valid(next_candidate):
            # try this partial candidate solution
            place(next_candidate)
            # given the candidate, explore further.
            backtrack(next_candidate)
            # backtrack
            remove(next_candidate)
```

## Optimizations

## Optimized Complexity

>[!Time Complexity]+

>[!Space Complexity]+

# Spiral Backtracking



# Related
