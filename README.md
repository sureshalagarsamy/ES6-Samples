### ES6 Samples

* How to add key, value pair in the existing array.

```javascript
var employeeList = [{id:'1', name:'A'},{id:'2', name:'B'}];
var isPermanent = {flag:true};
var newEmployeeList = ids.map((eachObj) => ({...eachObj, ...isPermanent}));
console.log(newEmployeeList);
```

![image](https://user-images.githubusercontent.com/6780840/49143435-077e7b00-f321-11e8-8a8c-88e3ba66fe67.png)

#### From `var` to `const / let`

* `const` - You can use it for all variables whose values never change.
* `let` – for variables whose values do change.
* Avoid `var`

#### template literals
* String interpolation

```javascript
const first = "SURESH";
const last = "A";
console.log(`(${first} ${last})`);
```

* Multi-line strings

```javascript
const HTML5_SKELETON = `
    <!doctype html>
    <html>
    <head>
        <meta charset="UTF-8">
        <title></title>
    </head>
    <body>
    </body>
    </html>`;
```


#### From `for` to `forEach()` to `for-of`

Prior to `ES5`, you iterated over Arrays as follows:

```javascript
var arr = ['a', 'b', 'c'];
for (var i=0; i<arr.length; i++) {
    var elem = arr[i];
    console.log(elem);
}
```

In `ES5`, you have the option of using the Array method `forEach()`

```javascript
arr.forEach(function (elem) {
    console.log(elem);
});
```

In `ES6`, the for-of loop combines both advantages:

```javascript
const arr = ['a', 'b', 'c'];
for (const elem of arr) {
    console.log(elem);
}
```

If you want both index and value of each array element, 

```javascript
var employee =[{id:1, name:'A'},{id:2, name:'B'}];
for (const [index, elem] of employee.entries()) {
    console.log(index+'. '+elem.name);
}
```
