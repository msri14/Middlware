# Middlware
This repo is to learn writing custom middleware and use the existing ones to the project.
Things Middleware can do:
- Preprocessing 
- logging
- Error Handling
- Authentication

1. body-parser (preprocessing Middleware)
       - pre-process the requests before it reaches the route handlers.
       - After Pre-processing, the final request can be found in the req.body
   run "node index.js" to see it's implementation.

2. morgan (logging)
       - logs the requests
       - available in predefined formats Ex: combined, tiny, short
   run "node index2.js"

3. Custom Middleware
       - takes the inputs req, res and next
       - perform the operations in the function and call next() method.
       - next() method should be called else the website hangs as it never reaches the route handler.
   run "node index3.js"

   Middleware code should be written before the route handlers.
