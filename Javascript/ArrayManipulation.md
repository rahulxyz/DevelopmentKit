# Iterating and Manipulation of data in arrays:

1. You have 2 arrays big[] and small[]. Remove all elements from big[] that are common in both array.
```javascript
let big = [1,2,3,4,5];
let small= [10,20,3,4,50];

let output = big.filter(e=>{
  return !small.includes(e);
})

```
