# 100 Days Of Code - Log

### Day 1: December 31, 2017 

**Today's Progress**: 
+ I try to play with the Twitter API on the browser. I found that the Twitter API can't be query from the browser because the servers of Twitter doesn't implement CORS.

+ I've done some 5 Basic Algorithme



**Things I learned:** 

**CORS**: Cross-origin ressource sharing. The server need to implement CORS if the site sending the request is not on the same domain or port.
To allow CORS on the server, the server must send this headers in the response:
```
Access-Control-Allow-Origin: *
Access-Control-Allow-Headers: Origin, X-Requested-With, Content-Type, Accept
```

The response doesn't contain these headers and the site on another domain or port the browser will throw a CORS issue.

**Today's Progress**: 
I've done some 5 Basic Algorithme.
I use Array.slice and Array.splice() as I often inverted these methods I'll write a memo.

### Day 2: January 1, 2017 

**Things I learned:**

**Array.prototype.slice()**

The slice() method returns a shallow copy of a portion of an array into a new array object selected from begin to end **(end not included)**. The original array will not be modified.
``` 
var animals = ['ant', 'bison', 'camel', 'duck', 'elephant'];

console.log(animals.slice(2));
// expected output: Array ["camel", "duck", "elephant"]

console.log(animals.slice(2, 4));
// expected output: Array ["camel", "duck"]

console.log(animals.slice(1, 5));
// expected output: Array ["bison", "camel", "duck", "elephant"]
```

**Array.prototype.splice()**

The splice() method **change** the array by removing or adding the elements to the array.
```
var myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];

myFish.splice(2, 0, 'drum'); // insert 'drum' at 2-index position
// myFish is ["angel", "clown", "drum", "mandarin", "sturgeon"]

myFish.splice(2, 1); // remove 1 item at 2-index position (that is, "drum")
// myFish is ["angel", "clown", "mandarin", "sturgeon"]
```

The exemples for this two methods are from the Mozilla website.


