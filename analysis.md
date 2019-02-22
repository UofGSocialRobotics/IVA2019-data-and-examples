## Analysis of rank-ordered data

A thorough description with code snippits to analyse results of 9 conditions of rank-ordered statements. 

### Comparing statements within-condition

In order to visualize how statements were ranked within each condition, each statement was given a score that is normalized 
between 0-n, where n is the number of statement options (in this case, 10). Scores are calculated by the following formula: 

```
# w = weighted rank of position
# x = response count for answer choice
x1(w1) + x2(w2) + x3(w3) .... + xn(wn) 
_____________________________________________
           total_response_count
```

In other words, the most preferred choice (ranked #1) has weight `n`, second choice has weight `n-1`, until the last choice has 
weight 1. 
For example, in this data, choice #1 has weight of 10, choice #2 has a weight of 9, ... choice #10 has a weight of 1. 

This formula allows us to have normalized scores within condition to visualize which choices were preferred over others. 
