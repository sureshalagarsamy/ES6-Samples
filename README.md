### ES6 Samples

* How to add key, value pair in the existing array.

```javascript
var employeeList = [{id:'1', name:'A'},{id:'2', name:'B'}];
var isPermanent = {flag:true};
var newEmployeeList = ids.map((eachObj) => ({...eachObj, ...isPermanent}));
console.log(newEmployeeList);
```

![image](https://user-images.githubusercontent.com/6780840/49143435-077e7b00-f321-11e8-8a8c-88e3ba66fe67.png)
