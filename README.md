# React-Neagoie

## React Components

* [Material UI](https://material-ui.com/)

## Databases

### JSON Placeholder Data

* [User Data Sample](https://jsonplaceholder.typicode.com/users)

## JavaScript Notes

### Map

```
const myArray = [1,2,3,4]

myArray.map( el => el + 1)
// returns [2,3,4,5]

myArray.map( el => "c")
// returns ["c", "c", "c", "c"]

myArray.map(() => 1 )
// returns [1,1,1,1]
```

### Promises

```
const myPromise = new Promise((resolve, reject) => {
  if (true) {
    setTimeout(() => {
      resolve('I have succeeded');  
    }, 1000);
  } else {
    reject('I have failed!');
  }
  
  // 1000 is number of milliseconds, or 1 second in this case
  
  myPromise.then(value => console.log(value));

})

```

### Filter

Filter is similar to map in that it takes a function that iterates over each element in an array. 

```
const myArray = [1,3,5,7,9]

myArray.filter( el => el > 5)
// returns [5,7,9]
```

### Includes

We can use "includes" with one argument to determine whether a value exists in an array. 

```
const myArray = [1,3,5,7,9]

myArray.includes(3)
// returns true
```

The second argument in includes() can be an index we want to start searching. 

```
const myArray = [1,3,5,7,9]

myArray.includes(3,2)
// returns false
// it's asking if "3" exists after index=2 (which is 5); it does not, hence false
```

However, this method only works with primitive data types. For other data types (arrays, objects, etc), this doesn't work because we are pointing to a specific location in the memory. For instance, this returns false:

```
const myArray = [ {id: 1} ]

myArray.includes({id:1)
// returns false
```

In order to make it work for an object, we'd need something like this:

```
const o1 = {id: 1} 
const o2 = {id: 2}

myArray = [o1, o2]

myArray.includes(o1)
// returns true
```

