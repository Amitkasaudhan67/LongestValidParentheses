# Longest Valid Parentheses

## Problem
Given a string containing only '(' and ')', return the length of the longest valid (well-formed) parentheses substring.

## Approach
- Use a stack to store indices.
- Push -1 initially.
- Push the index of every '('.
- For every ')', pop the stack.
- If the stack becomes empty, push the current index.
- Otherwise, calculate the valid substring length using:
  currentLength = i - stack.peek()

## Time Complexity
O(n)

## Space Complexity
O(n)
