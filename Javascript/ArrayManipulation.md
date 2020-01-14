# Iterating and Manipulation of data in arrays:

1. You have 2 arrays big[] and small[]. Remove all elements from big[] that are common in both array.
```javascript
let big = [1,2,3,4,5];
let small= [10,20,3,4,50];

let output = big.filter(e=>{
  return !small.includes(e);
})

```

2. You have 2 arrays of objects A[] and B[]. Remove all elements from B[] that are common in both array.
```javascript
let A = [
  {name: 'a', age: 20},
  {name: 'b', age: 30},
  {name: 'c', age: 10},
]

let B = [
  {name: 'a', age: 20},
  {name: 'b', age: 40},
  {name: 'd', age: 10},
  {name: 'e', age: 20},
  {name: 'f', age: 10},
]

const compareName = (obj1, obj2)=>{
  return (obj1.name === obj2.name);
}

const compareAll = (obj1, obj2)=>{
  return (obj1.name === obj2.name && obj1.age=== obj2.age);
}

let newArr = B.filter(b=>{
  let indexFound = A.findIndex(a => compareName(a, b));
  return indexFound==-1
})


```

3. You are given an array of numbers or strings. Remove all duplicate elements from it.
```javascript
let big = ["a","b","c","a","b","c","e","f"]

function removeDuplicate(element,pos){
  return big.indexOf(element) === pos;
}

let output = big.filter(removeDuplicate);
```
