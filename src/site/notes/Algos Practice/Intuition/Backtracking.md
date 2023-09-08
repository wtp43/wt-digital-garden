---
{"dg-publish":true,"permalink":"/algos-practice/intuition/backtracking/"}
---

It's important to remember that backtracking is just DFS except we can visit a node n times. Time complexity O(n!)

# Backtracking
- [x] <mark style="background: #cc085d;">+</mark> [[Leetcode Questions/LC-51. N-Queens\|LC-51. N-Queens]]
- [ ] Maze Solving 
- [ ] Knights Tour
- [ ] Hamiltonian Paths
- [ ] [[Leetcode Questions/LC-489. Robot Room Cleaner\|LC-489. Robot Room Cleaner]]

- [ ] [[Leetcode Questions/LC-131. Palindrome Partitioning\|LC-131. Palindrome Partitioning]]
- We want to partition a string s such that every substring of the partition is a palindrome
- When backtracking, it's important to determine if we are at a valid step. Only if we are do we proceed to the next step (continue recursing).


- [ ] [[Leetcode Questions/LC-647. Palindromic Substrings\|LC-647. Palindromic Substrings]]

- [ ] [[Leetcode Questions/LC-131. Palindrome Partitioning\|LC-131. Palindrome Partitioning]]
- We want to partition a string s such that every substring of the partition is a palindrome
- When backtracking, it's important to determine if we are at a valid step. Only if we are do we proceed to the next step (continue recursing).
# Advanced Backtracking
[[Leetcode Questions/LC-465. Optimal Account Balancing\|LC-465. Optimal Account Balancing]]
- After a given list of transactions, we want to settle all the debts
- `debt[i] > 0` means a person needs to pay `$ debt[i]` to  person(s); * `debt[i] < 0` means a person needs to collect `$ debt[i]` back from other person(s).
- Settle the debt of all possible pairs of `debt[i] * debt[j] < 0
- Order does not matter because we try all possible pairs. 
- Reduces to subset-sum n times
- Time complexity: O(n!)
- To iterate a dictionary 
	- list(dict.keys()) or list(dict.values())

