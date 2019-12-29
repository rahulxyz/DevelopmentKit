# Require and Export

```javascript
// File: demo.js
const fetch = require('node-fetch');

function sum(a,b){
    return a+b;
}

const fetchData = fetch('https://jsonplaceholder.typicode.com/todos/1')
  .then(response => response.json())
  .then(json => console.log(json))

module.exports = {
  sum: sum,
  fetchData: fetchData
}
```

```javascript
//Another file where we will require
const demo = require('./demo');

console.log(demo.sum(1,2));
console.log(demo.fetchData());
```
