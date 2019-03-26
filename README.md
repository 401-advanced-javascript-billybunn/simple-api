![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

<!-- LINKS -->
<!-- Replace the link for each in brackets below -->
<!-- PR (working into submission) -->
[1]: http://xyz.com
<!-- travis build -->
[2]: https://www.travis-ci.com/YOUR_ORG_NAME/REPO_NAME
<!-- back-end -->
[3]: http://xyz.com
<!-- front-end -->
[4]: http://xyz.com
<!-- swagger -->
[5]: http://xyz.com
<!-- jsdoc-->
[6]: heroku-link/docs 

## Simple API

### Author: Billy Bunn

### Links and Resources
* [PR][1]
* [travis][2]
<!-- (when applicable) -->
* [back-end][3]
<!-- (when applicable) -->
* [front-end][4]

#### Documentation
<!-- API assignments only -->
* [swagger][5]
<!-- (All assignments) -->
* [jsdoc][6]

### HTTP requests
#### `/categories` GET, POST
GET: 
* `http :3000/categories`
POST: 
* `echo '{"name":"candy", "display_name":"Sweet Treats", "description":"These taste good, but dont look at the ingredient list."}' | http :3000/categories`
* `echo '{"name":"vegetables", "display_name":"Super Foods", "description":"Ewwwwww!"}' | http :3000/categories`
* `echo '{"name":"meat", "display_name":"Dead Animals", "description":"Its the circle of life"}' | http :3000/categories`

#### `/categories/:id/` PUT, DELETE
PUT: 
* `echo '{"name":"meat", "display_name":"Deli", "description":"Lets forget about animal cruelty for tonights dinner"}' | http put :3000/categories/3`
DELETE: 
* `http delete :3000/categories/3`

#### `/products` GET, POST
GET:
* `http :3000/products`
POST:
* `echo '{"name":"reeses", "display_name":"Reeses Peanut Butter Cups", "description":"Chocolate cup filled with peanut butter","category":"candy"}' | http :3000/products`
* `echo '{"name":"snickers", "display_name":"Snickers", "description":"Nougat topped with caramel and peanuts that has been enrobed in milk chocolate","category":"candy"}' | http :3000/products`
* `echo '{"name":"kale", "display_name":"Gross Green Stuff", "description":"I really dont care how healthy this is for me. Not worth it.","category":"vegetables"}' | http :3000/products`

#### `/products/:id/` PUT, DELETE
PUT: 
* `echo '{"name":"snickers", "display_name":"Snickers", "description":"My least favorite candy","category":"candy", "_id":2}' | http put :3000/products/2`
DELETE: 
* `http delete :3000/products/2`







### Modules
#### `modulename.js`
##### Exported Values and Methods

###### `foo(thing) -> string`
<!-- If you finished everything, you should be able to copy/paste the lab requirements and put them in present tense. -->
Usage Notes or examples

###### `bar(array) -> array`
Usage Notes or examples

### Setup
#### `.env` requirements
* `npm i`
* `PORT` - assign a port number
* `MONGODB_URI` - URL to the running mongo instance/db


#### Running the app
* `npm start`
* Endpoint: `/`
* Endpoint: `/foo/bar/`
  * Returns a JSON object with abc in it.
* Endpoint: `/bing/zing/`
  * Returns a JSON object with xyz in it.
  
#### Tests
* How do you run tests?
  * `npm run test`
  * `npm run lint`
* What assertions were made?
* What assertions need to be / should be made?

#### UML
Link to an image of the UML for your application and response to events
