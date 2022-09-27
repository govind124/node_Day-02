Q.01 What are the different types of HTTP requests?
1.GET(The GET method is used to retrieve information from the given server using a given URI. Requests using GET should only retrieve data and should have no other effect on the data.)
2.POST(A POST request is used to send data to the server, for example, customer information, file upload, etc. using HTML forms.)
3.PUT(Replaces all current representations of the target resource with the uploaded content.)
4.PATCH(PATCH is similar to PUT request, but the only difference is, it modifies a part of the data. It will only replace the content that you want to update.)
5.DELETE(Removes all current representations of the target resourcCORS stands for Cross-Origin Resource Sharing. It allows us to relax the security applied to an API. This is done by bypassing the Access-Control-Allow-Origin headers, which specify which origins can access the API.e given by a URI.)

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

Q.03 Explain CORS
CORS stands for Cross-Origin Resource Sharing. It allows us to relax the security applied to an API. This is done by bypassing the Access-Control-Allow-Origin headers, 
which specify which origins can access the API. CORS is a browser security feature that restricts cross-origin HTTP requests with other servers and specifies 
which domains access your resources.
Ex-const cors = require('cors');
  app.use(cors({
    origin: ['https://www.section.io', 'https://www.google.com/']
  }));

Q.4 What is Express. how it helps you to create a backend application
Express is a Node.js framework for building web applications. According to the official website, it is a Fast, unopinionated, minimalist web framework for Node.js.

Q.05 Explain min 5 status codes gets used in Backend development
Q.06 Difference between HTTP and HTTPS
Q.07 What are JWT tokens?
