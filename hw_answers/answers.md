1) What is responsible for defining the routes of the games resource?

    in server/server.js the gamesRouter, which is built using the create_router from server/helpers/create_router.js

2) What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?

    The structure is more seperated than we've previously seen.

    The server is responsible for handling requests and storing information in the db.

    The client is responsible for displaying the server responses on the web browser and handling user inputs

3) What are the the responsibilities of server.js?

    Server.js  connects with the db and accesses the desired collection
    It also creates a router which defines CRUD methods for that collection

    it also allows the client to connect and utilise these tools


4) What are the responsibilities of the gamesRouter?

    gamesRouter defines CRUD methods for the gamesCollection in the db

5) What process does the the client (front-end) use to communicate with the server?

    the client makes http requests to the server via the fetch() method

6) What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs

    the fetch method takes an optional arg which is a js object

    it sets out the different options for the fetch request e.g. method type (GET, POST), request body, and headers

7) Which of the games API routes does the front-end application consume (i.e. make requests to)?

    INDEX   -  to display all games
    INSERT -    to add a new game to db
    DELETE - to remove a game from the db


8) What are we using the MongoDB Driver for?

    the driver allows our application to connect with the db and use the data meaningfully via callbacks or promises

    it allows us to use the db methods such as insertOne() or find().