## Array.map()

**The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.**

**Example :**
```
const array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]
```

## Array.reduce()

**The reduce() method executes a reducer function (that you provide) on each element of the array, resulting in single output value.**

**Example :**
```
const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// expected output: 10

// 5 + 1 + 2 + 3 + 4
console.log(array1.reduce(reducer, 5));
// expected output: 15
```

## Superagent :

const superagent = require('superagent');
 ```
// callback
superagent
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' }) // sends a JSON post body
  .set('X-API-Key', 'foobar')
  .set('accept', 'json')
  .end((err, res) => {
    // Calling the end function will send the request
  });
 
// promise with then/catch
superagent.post('/api/pet').then(console.log).catch(console.error);
 
// promise with async/await
(async () => {
  try {
    const res = await superagent.post('/api/pet');
    console.log(res);
  } catch (err) {
    console.error(err);
  }
})();
```

## Promises :

**A promise is used to handle the asynchronous result of an operation. JavaScript is designed to not wait for an asynchrnous block of code to completely execute before other synchronous parts of the code can run. For instance, when making API requests to servers, we have no idea if these servers are offline or online, or how long it takes to process the server request.**

**With Promises, we can defer execution of a code block until an async request is completed. This way, other operations can keep running without interruption.**


## Callback functions :

**When you pass a callback to a function, you expect that function to call your callback function some other time. However, it isn't automatically asynchronous.**

**the direct answer to the question is mostly yes. When you specify a callback to functions in Node.js, by convention they will be called on another callstack at a later point in time. But if you are using some bad code from someone who didn't know how to follow this convention, there is no guarantee.**



