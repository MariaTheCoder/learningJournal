# July 2021

## 3

Today I learned about RESTful Services or API's which enable a client access to a server's data through HTTP requests. 

There are HTTP requests to
* Add new data to the server
* Update existing data on the server
* Delete existing data on the server
* Read existing data on the server

The server (software) can run on the localhost or a remote system in a different network. 

REST, which stands for "REpresentational State Transfer", is a convention for building HTTP services. It is by making use of this protocol that we are able to read, edit, delete and read the data of the server.

Today I learned how to read or review the data on the server by doing an HTTP request called get. 

I also learned how to change the port which the localhost listens to in two ways  
* by asking the CRUD application to listen to a different port in a js file or
* by creating a server.config.json configuation file from where a specific port can be typed

If desired, one can modify which data to review by using route parameters. Here is an example of how to get a list of movies from a server released in a specific year: 

```js
const express = require('express');
const app = express();

app.get('api/movies/:year', (req, res) => {
    res.send(req.params.year);
});
```
A user might also send a request to a server for a page which content is sorted by date, title etc. 

```js
'/api/movies/2017?sortBy=title'
```
I also learned the usefulness of a new npm package called Nodemon which if installed globally restarts the node application whenever code is saved. 