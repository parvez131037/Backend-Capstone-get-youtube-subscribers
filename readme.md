<div id="header" align="center">
  <img src="https://cdn-icons-png.flaticon.com/128/8841/8841503.png" width="100"/>
</div>
<div align="center">
<h2>Hey there! <h2>
  <p>Myself Parvez Ahmed Ansari !</p> 
</div>
  
  <div id="badges" align="center">
  <a href="https://www.linkedin.com/in/parvez-ansari-b211a6144/">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a>
  <a href="https://youtu.be/jXC75HJjvnM">
    <img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube Badge"/>
  </a>
  <a href="https://twitter.com/parvez_ansari45">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
</div>

 ## Getting Started
 

# Building a RESTful CRUD (Create, Retrieve, Update, Delete) API with Node.js, Express js and MongoDB. ##
### Used Mongoose for interacting with the MongoDB instance. ###

Express is one of the most popular web frameworks for node.js. It is built on top of node.js http module, and adds support for routing, middleware, view system etc. It is very simple and minimal, unlike other frameworks that try do way to much, thereby reducing the flexibility for developers to have their own design choices.  

Mongoose is an ODM (Object Document Mapping) tool for Node.js and MongoDB. It helps you convert the objects in your code to documents in the database and vice versa. 

## Prerequisites:  
Please install MongoDB in your machine if you have not done already. Checkout the official MogngoDB installation manual for any help with the installation.



<h2>Project Description</h2>
  <b>Project Name : Almabetter (backend) Capstone project "get-youtube-subscribers" Restful API </b>
  <a href="https://get-youtube-subscribers.onrender.com/api/subscribers"> Live Here</a>
  
 
 <br>
 </br>

<b>Languages and Tools used: </b>  
 <div>
  <img src="https://img.icons8.com/offices/512/express-js.png" title="Express js" alt="Express js" width="50" height="50"/>&nbsp;
  <img src="https://www.svgrepo.com/show/331488/mongodb.svg" title="MongoDB" alt="MongoDB" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/npm/npm-original-wordmark.svg"  title="npm" alt="npm" width="40" height="40"/>&nbsp;
  <img src="https://github.com/detain/svg-logos/blob/master/svg/mongoose-1.svg" title="Mongoose" alt="Mongoose" width="40" height="40"/>&nbsp;
  <img src="https://www.svgrepo.com/show/354202/postman-icon.svg" title="Postman" alt="Postman" width="40" height="40"/>&nbsp;
 <img src="https://upload.vectorlogo.zone/logos/render/images/bb711e6b-3dc7-496f-b665-10558e88ceed.svg" title="Render app" alt="Render app" width="60" height="60"/>&nbsp;
 <img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="Javascript" alt="JavaScript" width="40" height="40"/>&nbsp;
  <img src="https://www.svgrepo.com/show/217753/github.svg" title="Github" alt="Github" width="40" height="40"/>&nbsp; 
  <img src="https://raw.githubusercontent.com/hapijs/assets/master/images/hapi.png" title="Happi Joi validation" alt="Happi Joi validation" width="40" height="40"/>&nbsp; 
  
</div><br>

### Our Application ###
In this project, We will be building a simple get-youtube-subscribers application. We will build Rest APIs for creating, listing, editing and deleting a Subscriber.  

We’ll start by building a simple web server and then move on to configuring the database, building the Subscriber model and different routes for handling all the CRUD operations.  

Finally, we’ll test our REST APIs using Postman.  

We’ll heavily use ES6 features like let, const, arrow functions, promises etc. 

### API Schema Documentation 

+ API URL: `https://documenter.getpostman.com/view/23674753/2s8Ysp2b4h` <br></br>
+ Local host: `https://documenter.getpostman.com/view/23674753/2s8Ysp2b4h` <br></br>

## Installation
```sh
$ git clone https://github.com/parvez131037/Backend-Capstone-get-youtube-subscribers.git
$ cd Backend-Capstone-get-youtube-subscribers
$ npm install
$ npm start
```

## Routes
### GET `http://localhost:3000/subscribers`

This request returns list of all subscribers with respect to  its _id, name, subscribed channel and subscribed date and time.

### GET `http://localhost:3000/subscribers/name`

This request return list of all subscribers with only thiers name and subscribed channel.

### GET `http://localhost:3000/subscribers/:id`

This request return one subscriber data from database followed by its id field.



### POST `http://localhost:3000/subscribers/add`

Create a new subscriber.

+ Method: `POST`
+ URL: `http://localhost:3000/subscribers/add`
+ Body:

```js
{
  "name": "Parvez ahmed ansari"
  "subscribedChannel": "Almabetter"
}
```



### PATCH `http://localhost:3000/subscribers/update/:Id`

Update entire subscriber with specific id.

+ Method: `PATCH`
+ URL: `http://localhost:3000/subscribers/update/6388da5b0c1189fa1438ef`
+ Body:

```js
{
  "name": "Parvez ahmed ansari"
  "subscribedChannel": "Almabetter Web Developement Programm"
}
```

### POST `http://localhost:3000/subscribers/addMany`

This request create multiple subscribers at one time. Data must be entered in an array of objects.

+ Method: `POST`
+ URL: `http://localhost:3000/subscribers/addMany`
+ Body:

```js
[
    {
        "name":"Dan Williams",
        "subscribedChannel":"adidas"
    },
    {
        "name":"Christina Robinson",
        "subscribedChannel":"Walmart"
    },
    {
        "name":"Charlie Howard",
        "subscribedChannel":"Amazon"
    },
    {
        "name":"Nathalie Holland",
        "subscribedChannel":"Microsoft"
    },
    {
        "name":"Harvey Norman",
        "subscribedChannel":"Verizon"
    }

]
```

### DELETE `http://localhost:3000/subscribers/delete/:id`

This request delete a subscriber with specific id.

+ Method: `DELETE`
+ URL: `http://localhost:3000/subscribers/delete/6388da5b0c1189fa1438ef`



<b>Key Features:</b><br>
  <b>➤ Validation:</b>  This application uses @happi/joi validation. Validating data can be very helpful in making sure that your application is stable and secure. Hapi allows this functionality by using the module Joi, which allows you to create your validations with a simple and clear object syntax.
  
  <b>➤User Experience</b> This is a optional but usable frontend  part. Frontend app that lists all the available subscribers in the database. The following application covers how to fetch information from our API and then displaying it in the form of a table to the user.. In this project i uses our project created deployed API 

Github link of frontend app-

+ URL: `https://github.com/parvez131037/get-youtube-subscribers-frontend-` <br></br>

# Preview
![](https://github.com/parvez131037/get-youtube-subscribers-frontend-/blob/main/src/assets/front.gif)
