# Node 3

## What is middleware?
Funcitons that are in the middle of client and server (but they are on the server)
In fact all endpoints are middleware too, we just dont normally includes 'next' in the parameters. YOu can have as manny middleware that you would like and they have to use the word next in the function of the middleware so it will continue on the path

Middleware function are run in the order that they are declared in the route, or in the order that they are written in the app.use()


## When do we use app.use() vs inline middleware?
app.use is for middleware that you want to use with evry single route (example is body-parser and cors)

Inline is useful when you want a middleware to run for one or more particular routes


## What is the 'next' parameter in a middleware function? What makes it useful, say, compared to if you were expect to use a return statement?
Calling next will run the next in line middleware or tge endpoint if there us no other middleware. Having a next function, as opposed to a simple return, is useful in case we need async functionlity


## What's an HTTP session?



