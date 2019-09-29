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
