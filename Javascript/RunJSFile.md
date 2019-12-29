# Run JS file

```javascript
//write this in package.json
//Filename to be run: demo.js
"scripts": {
    ...
    "start": "node demo",
    ...
},
```
```
npm start OR npm run start
```

You can also write individual filenames here:
```javascript
//write this in package.json
//Filename: demo.js
"scripts": {
    ...
    "demo": "node demo",
    ...
},
```

```
npm demo OR npm run demo
```
