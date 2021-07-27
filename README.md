## FUll Stack Javascript Online Store CRUD App

Building a full stack application that allows users to view products, add products, update products and delete products.

[Go to live app store](url)(https://aidens-store.vercel.app/){:target="_blank"}

Using:

-  Client:
   -  Vanilla javascript for DOM manipulation and fetch for AJAX requests
   -  bootstrap for layout and style
-  Server:

   -  Postgres for our database
   -  knex.js for our database migrations, seeds and queries
   -  express.js for JSON routes

-  Prerequisites
   -  latest version of Node.js
   -  lite-server
   -  Postgres

## Server Check List

-  [x] Setup client folder
   -  [x] index.html
   -  [x] add bootswatch CDN
   -  [x] create app.js
   -  [x] git init
-  [x] Create server folder
   -  [x] generate express app
   -  [x] git init
-  [ ] Convert Express App to JSON API
   -  [x] Remove view rendering/views folder
   -  [x] Remove routes folder
   -  [x] Remove static server and public folder
   -  [x] Update error handler
   -  [x] Add GET `/` endpoint
-  [x] Client: Try to make a request
   -  [x] See the CORS error and remember this moment
   -  [x] Add CORS to the API
-  [x] Create Database
-  [ ] Initialize knex project
   -  [x] Install knex and pg
   -  [x] Create knexfile.js
-  [x] Create product table migration
-  [x] Seed product table with sample data
-  [x] Add api folder and create/mount router
-  [x] Connect to the database
   -  [x] Create database connection file
   -  [x] Create a queries file
-  [ ] List all records with GET /api/v1/products
   -  [x] Create query
   -  [x] Create route
-  [ ] List all records in /index.html
   -  [x] AJAX Request to GET /products
   -  [x] Append to DOM
   -  [x] Each product links to /product.html?id=:id
   -  [x] Display a link to /create.html
-  [x] Show one record with GET /api/v1/products/:id
   -  [x] Validate id
   -  [x] Create query
   -  [x] Create route
-  [x] Show one record in /product.html?id=:id
   -  [x] Parse query string to get id
   -  [x] AJAX Request to GET /products/:id
   -  [x] Append to DOM
   -  [x] Display link to /edit.html?id=:id
-  [ ] Create a record with POST /api/v1/products
   -  [x] Create route
   -  [x] Validate product
   -  [x] Create query
-  [x] Create a record in /create.html
   -  [x] Display a form with input boxes for all fields
   -  [x] Display a button to submit the creation of the resource
      -  [x] Validate all inputs
      -  [x] POST /products
      -  [x] Successful creation should redirect to /product/html?id=:id
   *  [x] Update a record with PUT /api/v1/products/:id
      -  [x] Create route
      -  [x] Validate id
      -  [x] Validate updates
      -  [x] Create query
   *  [x] Update one record in /product.html?id=:id
      -  [x] Display a form with input boxes for all fields
      -  [x] Display a button to submit the update of the resource
         -  [x] Validate all inputs
         -  [x] PUT /products/:id
         -  [x] Successful update should redirect to /product.html?id=:id
   *  [x] Delete a record with DELETE /api/v1/products/:id
      -  [x] Create route
      -  [x] Validate id
      -  [x] Create query
   *  [x] Delete a record
      -  [x] Add a delete button to the /product.html page
         -  [x] DELETE /products/:id
         -  [x] Successful deletion should redirect to index.html
   *  [x] Deploy server to Heroku
      -  [x] Signup and login to Heroku
      -  [x] Install the Heroku CLI
      -  [x] Create a Heroku app
      -  [x] Push to Heroku
      *  [x] View Heroku logs
   *  [x] Add Postgres DB to Heroku
      -  [x] Add postgress addon
      -  [x] Add production connection to knex
      -  [x] Run migration to production DB
      -  [x] Run seeds on production DB
   *  [ ] Deploy client to firebase
      -  [ ] Signup and login to firebase
