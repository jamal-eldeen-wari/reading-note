#  Spring Authorization

* **OAuth2** is an authorization framework that enables the application Web Security to access the resources from the client.

There are several samples building on each other, adding new features at each step:

1. Simple: It is a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties.

2. Click: adds an explicit link that the user has to click to login.

3. Logout: It adds a logout link as well for authenticated users.

4. Two Provided: Adds a second login provider so the user can choose on the home page which one to use.

5. Custom Error: It adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.


