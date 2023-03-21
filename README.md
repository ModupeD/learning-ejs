# learning-ejs


I decided to use a Postgresql Database because it is compatible with my Mac OS. I created a database called studentschedler, with a user , all the information is in the .env file


I created a server JS file and set it to run on port 5000

Then I installed express and express - flask. I set my view engine to ejs.

I started by creating five endpoints
/
/users/login
/users/register
/users/dashboard
/users/logout

I created get requests for these endpoints and then two post requests for login and register

The register post request stored the name, email and password of users, checks if the information is in the right format and populates the database if there are no errors.

The login post request checks if the user is in the database and that the information is the same, then it redirects them to the dashboard if it is correct, if it is wrong it redirects them to the login page.

I created four views for the different endpoints

Dashboard.ejs
Login.ejs
Register.ejs
Index.ejs

I created a dbConfig file where i stored my connection strings that would link my database with my code

I created a paaswordConfig.js file that stored code for authenticating the user, checking if the passwords are correct and if the account exists already. 

The server.js had Post requests for registering a new user and logging in. If the user is authenticated they get rerouted to the dashboard. If user is not logged in reroute them to the login.


I had to install the following dependencies for my code to work
