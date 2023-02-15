Express REST API

Classes are a template for creating __objects__.

Can a class declaration be hoisted? No. "Class declarations have the same temporal dead zone restrictions as const or let and behave as if they are not hoisted."

How would you describe a constructor and contextual “this” to a non-technical friend?
  a constructor is kind of like the recipe for an object instance of a class. It contains properties which are sort of like the ingredients. Using "this" allows us to refer to the object.

Using Express Routing

Within Express, what does routing refer to? Routing refers to the endpoints

What is the difference between a route path and a route method?
  Route paths: "Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions."

  Route methods: "A route method is derived from one of the HTTP methods, and is attached to an instance of the express class."

When is it appropriate to add next as a parameter to a route handler and what must 
you do if next has been passed to your middleware as a parameter? 

1. "With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback."
2. To bypass remaining route callbacks. "You can use this mechanism to impose pre-conditions on a route, then pass control to subsequent routes if there’s no reason to proceed with the current route."


Express Routing

What is an Express Router?
"Router is like a mini-Express application. It doesn’t bring in views or settings but provides us with the routing APIs like .use, .get, .param, and route."

By what mean do we initialize express.Router() in an express server?
  "// get an instance of router
    var router = express.Router();"

What do we use route middleware for?
"Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we’d like to do before we actually spit out information to our user."

Reflection
What are your learning goals after reading and reviewing the class README?
Continuing to solidify the pieces needed to build a REST API server and how that's modified with express. Also routes.


Sources:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes
https://expressjs.com/en/guide/routing.html
https://www.digitalocean.com/community/tutorials/learn-to-use-the-new-router-in-expressjs-4
