Q.01 What are the different types of HTTP requests?
1.GET(The GET method is used to retrieve information from the given server using a given URI. Requests using GET should only retrieve data and should have no other effect on the data.)
2.POST(A POST request is used to send data to the server, for example, customer information, file upload, etc. using HTML forms.)
3.PUT(Replaces all current representations of the target resource with the uploaded content.)
4.PATCH(PATCH is similar to PUT request, but the only difference is, it modifies a part of the data. It will only replace the content that you want to update.)
5.DELETE(Removes all current representations of the target resourcCORS stands for Cross-Origin Resource Sharing. It allows us to relax the security applied to an API. This is done by bypassing the Access-Control-Allow-Origin headers, which specify which origins can access the API.e given by a URI.)
-------------------------------------------------------------------------------------------------------------------------------------------------
Q.02 Explain the concept of middleware in Node.js.
Middleware:-Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in 
the application’s request-response cycle.The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.
1.Execute any code.
2.Make changes to the request and the response objects.
3.End the request-response cycle.
4.Call the next middleware in the stack.
Ex-const myLogger = function (req, res, next) {
  console.log('LOGGED')
  next()
 }
 
-------------------------------------------------------------------------------------------------------------------------------------------------
Q.03 Explain CORS
CORS stands for Cross-Origin Resource Sharing. It allows us to relax the security applied to an API. This is done by bypassing the Access-Control-Allow-Origin headers, 
which specify which origins can access the API. CORS is a browser security feature that restricts cross-origin HTTP requests with other servers and specifies 
which domains access your resources.
Ex-const cors = require('cors');
  app.use(cors({
    origin: ['https://www.section.io', 'https://www.google.com/']
  }));
  
--------------------------------------------------------------------------------------------------------------------------------------------------
Q.4 What is Express. how it helps you to create a backend application
Express is a Node.js framework for building web applications. According to the official website, it is a Fast, unopinionated, minimalist web framework for Node.js.
Middleware gets executed after the server receives the request and before the controller actions send the response. Middleware has the access to the request object, responses object, and next, it can process the request before the server send a response. An Express-based application is a series of middleware function calls.

--------------------------------------------------------------------------------------------------------------------------------------------------

Q.05 Explain min 5 status codes gets used in Backend development
HTTP status codes are delivered to your browser in the HTTP header. While status codes are returned every single time your browser requests a web page or resource, most of the time you don’t see them.
100s: Informational codes indicating that the request initiated by the browser is continuing.
200s: Success codes returned when browser request was received, understood, and processed by the server.
300s: Redirection codes returned when a new resource has been substituted for the requested resource.
400s: Client error codes indicating that there was a problem with the request.
500s: Server error codes indicating that the request was accepted, but that an error on the server prevented the fulfillment of the request.

--------------------------------------------------------------------------------------------------------------------------------------------------
Q.06 Difference between HTTP and HTTPS
HTTP--HTTP stands for Hypertext Transfer Protocol, and it is a protocol—or a prescribed order and syntax for presenting information—used for transferring data over a network. Most information that is sent over the Internet, including website content and API calls, uses the HTTP protocol.
HTTPS--HTTPS stands for Hypertext Transfer Protocol Secure (also referred to as HTTP over TLS or HTTP over SSL). HTTPS uses TLS (or SSL) to encrypt HTTP requests and responses, so instead of the plaintext, an attacker would see a series of seemingly random characters.

--------------------------------------------------------------------------------------------------------------------------------------------------
Q.07 What are JWT tokens?
JWT specifies a compact and self-contained method for communicating information as a JSON object between two parties. Because it is signed, this information can be checked and trusted. JWTs can be signed using a secret (using the HMAC algorithm) or an RSA or ECDSA public/private key combination. In a moment, we’ll see some examples of how to use them.
Prerequisites--
1.A working knowledge of JavaScript.
2.A good understanding of Node.js.
3.A basic understanding of MongoDB or any database of your choice.
4.Postman and some knowledge on how to use Postman.

-------------------------------------------------------------------------END-------------------------------------------------------------------------
