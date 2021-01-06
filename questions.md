1. What is responsible for defining the routes of the games resource?

Create Router, which links to app.use in server.js

2. What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?

Server - Responsible for backend, manages routing, creates and seeds the database and also handles requests and responses through listening.

Client =  Responsible for frontend, creates interactive output on to the page (displays database), it also handle, functions such as adding or removing games. Creates useState hooks to set and store user input from the forms on the page.

3. What are the the responsibilities of server.js?

  1. Parses form input and stores it as a javascript object.
  2. Creates DB.
  3. Sets up the main route '/api/games'
  4. Creates port listener
  5. Sets up Http headers to enable Cross-Origin Resource Sharing


4. What are the responsibilities of the gamesRouter?

Sets up the CRUD action routes].

5. What process does the the client (front-end) use to communicate with the server?

Fetch(post and delete request), the client sends a request and server sends a response.


6. What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs

Fetch is taking an object as the second argument, postGame is adding a new game, delete is removing a game.


7. Which of the games API routes does the front-end application consume (i.e. make requests to)?

/api/games

8. What are we using the MongoDB Driver for?

To host the database

9. Why do we need to use ObjectId from the MongoDB Driver?

So unique ids can be created and referenced for each new game added to the database
