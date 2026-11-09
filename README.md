# Fruit API 
This project was built in the process of learning how a backend of an application is built with a RESTful API and using the MVC framework. 
## MVC (Model, View and Controller) framework
MVC framework is used to structure the backend code of an application by separating the code into 3 components.
- **Model** manages the application's data including the database interactions. So it handles the data that is transferred between the view and controller.
- **View** is the user interface(UI) that the user of the application interacts with and it is linked to the controller. As it displays data provided by the
  controller as a result that is presented to the user through the UI.
- **Controller** is the intermediary between the views and model components. It receives and processes the incoming request from the user into the model and
  then renders the output/result to the UI.

## RESTful API 
RESTful API is how software systems are able to communicate with each other following a set of design principles Representational State Transfer (REST). 
The principles are:
- Uniform interface
- Statelessness
- Layered system
- Cachebility
- Code on demand 

### HTTP methods
In terms of the actions and interactions, they will all have a unique URL which will be called using HTTP methods. The HTTP methods are:
|Method    | Purpose   | example     | explanation|
|----------|------------|-------------|------------|
|GET        | Purpose   | GET '/name'     | explanation|
|POST       | Purpose   | POST  '/'     | explanation|
|PUT/PATCH   | Purpose   | PATCH '/:name'   | explanation|
|DELETE     | Purpose   | DELETE '/:name'     | explanation|

- These HTTP methods are usually found in the Routes folder which will alos include the imports of express, Router and the controllers script.
  ```js
    const express = require('express')
    const router = express.Router()
    const fruits = require('../controllers/fruitsControllers')
  ```
    - Express is a backend application framework for Node.js that is used to build web applications and APIs.
    - Express.Router() is an function called from express that is used to create a new router that is used to handle requests called from express library and it is used.
      eg. `router.get('/:name', fruits.show)` 
- router is then exported and imported into the ...
  ```js
  module.exports =  router
  ```

  
  

