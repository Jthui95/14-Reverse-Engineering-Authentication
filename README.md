# 14-Reverse-Engineering-Authentication Explanation 

##  Files explained

###  Config
1. Middleware file makes sure that the user has to be logged in in order to utilize the application.
2. The config.json file connects to the server and the database
3. passport.js tells the user that in order to login we need an email and a password. 

### Models
1. index.js this file allows the user to connect to the database and imports the users login data.
2. user.js uses bycrpt to protect the password. 

### Routes
1. api-routes.js contains all the routes for logging in, signing out, and displaying pertient data.
2. html-routes.js this file checks to see if the user is logged in and has a valid account that they can use. If they are logged in it will send them to the right page.

### Package.json
Contains the packages, node modules and necesarry npm install files. 

### Server.js
this requires the packages, contains the port that will be used, creates the express and middleware, creates the routes, syncs up the databases and displays a message when you have successfully connected to the server. 