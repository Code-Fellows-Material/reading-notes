# Class 12 Reading Notes

---

## Things I want to know more about

- Is it generally up to us as developers to use these codes, or are they baked in to some client/server languages?

---  
## Status Codes Based On REST Methods

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

*In your own words, describe what each group of status code represents:*
    - 100’s = Informational Codes,  that tell the client that the server has received the code and will attempt to do what is asked of it.
    - 200’s = Success Codes, not that it was successfully processed, but that the request was accepted.
    - 300’s = Redirect Codes, these aren't the resources you're looking for~~~
    - 400’s = Request Error Codes, these indicate invalid requests.
    - 500’s = Server Error Codes, these indicate an error server side. 
  
*What is a status code 202?*
    - Accepted, used with async code, tells the client the request was properly received and it will return the info when it's done processing.

*What is a status code 308?*
    - Permanent Redirect, tells the client to use another URL to make the request. 

*What code would you use if an update didn’t return data to a client?*
    - 204

*What code would you use if a resource used to exist but no longer does?*
    - 308

*What is the ‘Forbidden’ status code?*
    - 403

---

## Build A REST API With Node.js, Express, & MongoDB - Quick 

- [Build A REST API With Node.js, Express, & MongoDB - Quick - Video](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

### Question Answers: 

*Why do we need to pull our MongoDB database string out of our server and put it into our .env?*
    - Because that string will be different in production.

*What is middleware?*
    - code that runs when your server gets requests, but before it gets passed to your routes. 

*What does app.use(express.json()) do?*
    - Lets our server accept JSON as a body.

*What does the /:id mean in a route?*
    - It is a parameter, one that will allow you to access an individual piece of data.

*What is the difference between PUT and PATCH?*
    - Patch allows us to update only what the user passes to us, vs PUT which will replace everything.

*How do you make a default value in a schema?*
    - we can use 'default: ' and a default value in our schema.

*What does a 500 error status code mean?*
    - Internal Server Error, it means something has gone wrong at the server.

*What is the difference between a status 200 and a status 201?*
    - A 201 code is a more specific success code than a 200, it means successfully created an object. 