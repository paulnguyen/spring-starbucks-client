
## Spring Starbucks Client


### Version 1.0

* Initial Implementation of Starbucks REST API Client
* Hard Coded to Localhost Port 8080


### Version 2.0

* Implementation of Starbucks REST API Client
* Configured Endpoints and Port to Localhost Port 80 with API Keys (i.e. for use with Kong)


### Version 3.0 

* Added Spring Security Spring Boot Starter
* Default Authentication Web Form Injected 
* Default User Name:  user
* Default User Password: (look for generated password during startup logs)
* Note: CSRF Token not included in Web Form (Fails on Startup)
	
	By doing nothing more than adding the security starter to the project build, 
	you get the following security features:
	
	* All HTTP request paths require authentication.
	* No specific roles or authorities are required.
	* Authentication is prompted with a simple login page.
	* There’s only one user; the username is user.

