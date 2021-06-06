# June 2021

## 5

Today I did a small exercise where I did an HTTP GET request. The goal of the exercise was to make an HTTP GET request to look through sever data - in this case courses - and find the course which ID matches the requested ID.  
In case no match was found, I returned a status error message 404 and if a match *was* found, I returned the data and displayed it in the live server.

I also learned how to make an HTTP POST request where I created a new course and added it to existing server data. I made the request by using a program called POSTMAN. It did the coding in Node.js and made sure that the CRUD application and POSTMAN listen to the same port.   
I was challenged to ensure that for each new element created, the ID increases with 1 compared to the last one created.  

I also learned how to validate an HTTP POST request by using an npm package called joi. I created a constant object called schema where I set criteria as to what is a valid request is. For example, I expect an object and I require a property called 'name'. The value of the name property, I expect to be a string containing alfanumeric characters, of minimum 3 to maximum 30 characters.   
However, since the validation process does not happen automatically, I had to call the validate method and store the result in a constant variable for later use. In the source code, the function call looked like this:   
```js
const Joi = require('joi');
const express = require('express');
const app = express();
const config = require('./server.config.json');

app.use(express.json());

app.post('/api/courses', (req, res) => {
    const schema = Joi.object({
        name: Joi.string().alphanum().min(3).max(30).required()
    })

    const result = schema.validate(req.body);

    if(result.error) {
        res.status(400).send(result.error.details[0].message);
        return;
    }

    const newId = courses[courses.length-1].id +1;

    const course = {
        id: newId, 
        name: req.body.name,
    }
    courses.push(course);
    res.send(course);
})
``` 
In case no name property exists in the HTTP POST request or the value of insert property does not match the criteria set in the schema constant, I wanted an HTTP error message 400 returned.