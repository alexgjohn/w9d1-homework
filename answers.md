1. The routes of the games resource are defined as templates in the create_router file and then tailored to the games API in the server.js file.
2. In short, the client folder handles the front end and the server folder handles the back end. 
3. I believe server.js handles the dialogue between the server side and the database. 
4. As noted above, the games router is a tailored version of the router template that has been pre-made. This would allow for multiple APIs and databases to be accessed using the same methods. 
5. The client end passes information to GamesServices, which makes fetch requests to the sever end.
6. The optional second argument specifies settings for the fetch request, allowing this to be changed to a POST or PUT and entering other valuable information (like the data to be added)
7. The  application 'consumes' (weird choice of words, if you don't mind me saying) different routes depending on which http request is being made. It has a base url and the create_router module specifies what it would add to this, depending on the needs of a specific process. 
8.  Look, I don't really know. chatGPT says a driver is something that enables communication between an application and a database, so I guess if the server is the go-between here for our client-side and our database, then the driver is what lets it fulfil this role. But I also am not confident in this answer, because I've never used mongodb.

9. It looks like ObjectID is the unique id created for each item (row?) in the database, so using this to access and manipulate an item here seems sensible. 
