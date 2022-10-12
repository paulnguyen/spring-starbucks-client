
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


### Version 3.1 

* Added Spring Security Bare Bones Configuration Class
* Added In-Memory User Config for Authentication
* Disabled CSRF Protection for POST Processing

	Spring Security:
	
	* https://docs.spring.io/spring-security/reference/servlet/authentication/passwords/storage.html
	
	Storage Mechanisms
	
	Each of the supported mechanisms for reading a username and password can leverage any of 
	the supported storage mechanisms:
	
	    * Simple Storage with In-Memory Authentication
	    * Relational Databases with JDBC Authentication
	    * Custom data stores with UserDetailsService
	    * LDAP storage with LDAP Authentication


### Version 3.2

* Added Support for CSRF Protection
* Updated Web Forms to include CSRF Token
* Added Home Controller (Redirects to Console)
* Added Login Controller & Custom Login Page

	Cross Site Request Forgery (CSRF)

	* https://docs.spring.io/spring-security/reference/features/exploits/csrf.html
	* https://docs.spring.io/spring-security/reference/servlet/exploits/csrf.html

	Custom Login Form Example

	* https://docs.spring.io/spring-security/reference/servlet/authentication/passwords/form.html
	* https://codepen.io/khadkamhn/pen/ZGvPLo




