# A NodeJs/Express RESTful API for User Authentication + Authorization using MongoDB and Gitpod Docker
The following are the endpoints with their brief description: (you can use POSTMAN or any other api caller....(however, I used PSOTMAN for TESTING))

================================================================
POST:   /api/auth/signup     
Description:   for SignUp/Registeration         
example request body---> {
	"email": "mytest5@gmail.com",
	"password": "EsmatHanif123",
	"username": "esmathanif5",
	"role": ["admin"]
}
================================================================
================================================================
POST:   /api/auth/signin
Description:   for Login/SignIn      
example request body---> {
	"password": "Ahmadkhan1",
	"username": "khanan"
}
================================================================
================================================================
POST:   /api/auth/signout
Description:   for Logout/SignOut

================================================================
================================================================
GET:   /api/test/all
Description:   for Public Content Authroization  

================================================================
================================================================
GET:   /api/test/user
Description:   for User Content Authorization
authToken is required (Should be signed in first)
================================================================
================================================================
GET:   /api/test/mod
Description:   for Modereator Content Authorization
authToken + moderator role is required (Should be signed in first)
================================================================
================================================================
GET:   /api/test/admin
Description:   for Admin Content Authorization
authToken + admin role is required (Should be signed in first)
================================================================
