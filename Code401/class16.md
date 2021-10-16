 # Spring Security:
 Spring Security has an architecture that is designed to separate authentication from authorization and has strategies and extension points for both.

 ## Authentication:
 The main strategy interface for authentication is AuthenticationManager, which has only one method:
 

 public interface AuthenticationManager
  {


  Authentication authenticate(Authentication authentication)

    throws AuthenticationException;


}

An AuthenticationManager can do one of 3 things in its authenticate() method:
1. Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.
2. Throw an AuthenticationException if it believes that the input represents an invalid principal.
3. Return null if it cannot decide.


What is AuthenticationException??
A: is a runtime exception. It is usually handled by an application in a generic way, depending on the style or purpose of the application.

The most commonly used implementation of **AuthenticationManager** is **ProviderManager**, which delegates to a chain of AuthenticationProvider instances. An AuthenticationProvider is a bit like an AuthenticationManager, but it has an extra method to allow the caller to query whether it supports a given Authentication type

Spring Security **provides some configuration helpers to quickly get common authentication manager features set up in your application**. **The most commonly used helper is the AuthenticationManagerBuilder**, **which is great for setting up in-memory, JDBC, or LDAP user details or for adding a custom UserDetailsService**

**Important to note that** the AuthenticationManagerBuilder is @Autowired into a method in a @Bean — that is what makes it build the global (parent) AuthenticationManager.


## Authorization:
Once authentication is successful, we can move on to authorization, and the core strategy here is AccessDecisionManager. There are three implementations provided by the framework and all three delegate to a chain of AccessDecisionVoter instances, a bit like the ProviderManager delegates to AuthenticationProviders.

**Most people use the default AccessDecisionManager, which is AffirmativeBased**


## Web Security:
 is based on Servlet Filters, so it is helpful to first look at the role of Filters generally. The following picture shows the typical layering of the handlers for a single HTTP request.

 How Does the Security works:

 1. The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI.

 2. At most, one servlet can handle a single request, but filters form a chain, so they are ordered. In fact, a filter can veto the rest of the chain if it wants to handle the request itself.

 3.  A filter can also modify the request or the response used in the downstream filters and servlet. The order of the filter chain is very important, and Spring Boot manages it through two mechanisms: @Beans of type Filter can have an @Order or implement Ordered, and they can be part of a FilterRegistrationBean that itself has an order as part of its API.
 