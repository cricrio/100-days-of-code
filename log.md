# 100 Days Of Code - Log

### Day 2: December 31, 2017 

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


