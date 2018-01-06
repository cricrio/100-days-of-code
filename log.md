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

If the response doesn't contain these headers and the site on another domain or port, the browser will throw a CORS issue.


**fetch()**
fetch is method use to make request.
```
init = {
  method, // GET, POST ....
  headers, 
  mode, // cors, no-cors (if no-cors mode enable Cache-Control, Content-Language,Content-Type,Expires,Last-Modified,Pragma can be added to request 
  cache, 
        }
fetch(url,[init]) : Promise<Response>
 


```

### Day 2: January 1, 2017 

**Today's Progress**: 

I've done some 5 Basic Algorithme.
I use Array.slice and Array.splice() as I often inverted these methods I'll write a memo.

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


### Day 3: January 2, 2017 

**Today's Progress**: 

I've finish the Basic Algorithme of Freecodecamp.

**Things I learned:**

**arguments of function**
To access the argument of a function use : 
```
function(...){
  const arg1 = arguments[0];
  const arg2 = arguments[1];
}
```
argument is not a array. It's only have the property length.
To transform arguments in a object use :
`const argArray = Array.from(arguments)`

**String.charCodeAt(...)**  
get the charCode of the char

```
const ZcharCode = 'Z'.charCodeAt(0)
```

**String.fromCharCode(...)**
create a string from the charCode



`const A = String.fromCharCode(65)` 

**Caesars Cipher**
Shift all alphanumeric char of 13 positions

```
var ZcharCode = 'Z'.charCodeAt(0);
var AcharCode = 'A'.charCodeAt(0);

function shift(charr){
 
  if(charr >=  'A' && charr <= 'Z'){
   
    var charCodeShift = charr.charCodeAt(0) + 13;
    if(charCodeShift > ZcharCode){
      charCodeShift = charCodeShift % ZcharCode + AcharCode -1;
    }
    return String.fromCharCode(charCodeShift);
  }
  return charr;
}

function rot13(str) { // LBH QVQ VG!
 return  str
   .toUpperCase()
   .split('')
   .map(shift)
   .join('');
}

```

**Array.sort(...)**
Sort the array. The default sort order is according to string Unicode code points. So if we want to sort the array of number we need to provide a function to compare the number.

```
function compare(a,b){
  if(a === b){
    return 0
  }
  return a > b ? 1 : -1;
}
```


### Day 3: January 3, 2017 
**Today's Progress**: I have done a major refractor of the cafe-litteraire-front repo

### Day 4: January 4, 2017 
**Today's Progress**:
I try to use ant-design, a UI framework. I wanted to use it for the date and time picker but the css of framework conflict with me css. I find the react-app-rewired to rewrite the config of create-react-app and add other babel plugin. I can use it to add the babel plugin transfrom the graphql file.

### Day 5: January 5, 2017 

**Today's Progress**: 
.
I install the firefox dev edition with ubuntu-make.
Ubuntu make is a command line tool wich allow you to download and install the latest version of popular developer tools.

`umake web firefox-dev`

### Day 5: January 6, 2017 

**Today's Progress**: 

I have done an algorithme to convert number to romain number.
I start my new blog with Gatsby and tackyons