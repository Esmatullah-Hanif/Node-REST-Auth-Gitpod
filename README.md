###### A NodeJs/Express RESTful API for User Authentication + Authorization using MongoDB and Gitpod Docker
Just Simplly run
```
npm install
or 
yarn install
```

and  then run:
```
npm start
```
------> so the server will be starting on a gitpod docker container and will listening on port 3000, the server will log that:

> Server is running on port 3000. Successfully connected to MongoDB.

###### NOTE: The backend database is in MongoDB, which is hosted on MongoDB Atlas Cluster, you can find its URL in (app/config/db.config.js). So, if you want to use your own MongoDB, simple put your online cluster url or your mongodb local database URL.


Then you can call RESTful API endpoints; 


###### The following are the endpoints with their brief description: (you can use POSTMAN or any other api caller....(however, I used PSOTMAN for TESTING)).

```
POST:   /api/auth/signup 
	Description:   for SignUp/Registeration      example request body---> {
		"email": "mytest5@gmail.com",
		"password": "EsmatHanif123",
		"username": "esmathanif5",
		"role": ["admin"]
	}

POST:   /api/auth/signin
	Description:   for Login/SignIn
	example request body---> {
		"password": "Ahmadkhan1",
		"username": "khanan"
	}

POST:   /api/auth/signout
	Description:   for Logout/SignOut

GET:   /api/test/all
	Description:   for Public Content Authroization  


GET:   /api/test/user
	Description:   for User Content Authorization
	authToken is required (Should be signed in first)

GET:   /api/test/mod
	Description:   for Modereator Content Authorization
	authToken + moderator role is required (Should be signed in first)

GET:   /api/test/admin
	Description:   for Admin Content Authorization
	authToken + admin role is required (Should be signed in first)
```

