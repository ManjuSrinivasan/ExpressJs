# Express.js  

>> Express.js is a modular web framework for Node.js. 
>> It is used for easier creation of web applications and services.
>> Express.js simplifies development and makes it easier to write secure, modular and fast applications.

# What is Express :

  -> Express is a fast,Unopinionated and minimalist web framework for Node.js
  -> Express is a "Server-side" or "backend" framework.
  -> It is not comparable to client-side framework like React,Angular & Vue. 
  -> It can be used in combination with those frameworks to build full stack applications.

# Why Use Express :
  
  $ Makes Building web applications with Node.js MUCH easier
  $ Used for both server rendered apps as well as API / Miicroservices
  $ Extremley light,fast and free
  $ Full controll of request and response
  $ By far the most popular Node framework
  $ Great to use with client side frameworks as it's all JavaScript

# Basic Server Syntax :

  const express = require('express');

  //init express

  const app=express();

  //create your endpoints/route handlers

  app.get('/',function(req,res){
      res.send("Hello World");
      //fetch from database
      //load pages
      //return json
      //full acess to request and response
  });

  //Listen on a port

  app.listen(5000);


# Basic route handling

  => Handling request/response is simple
  => app.get(),app.post(),app.put(),app.delete(),etc 
  => Access to params,query strings,url parts,etc
  => Express has a router so we can store routes in separate files and export
  => We can parse incoming data with Body parser

app.get('/',function(req,res){
      res.send("Hello World");
      //fetch from database
      //load pages
      //return json
      //full acess to request and response
  });

# Express Middleware :
  
 >> Middleware functions are functions that have access to the request and response object.
 >> Express has built in Middleware but Middleware also comes from 3rd party packages as well as custom Middleware
     
     -> Executes any code
     -> Make changes to the request/response objects
     -> End response cycle
     -> call next Middleware in the stack
