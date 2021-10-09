# Create a Web Controller:
HTTP requests are handled by a controller where you can easily identify the controller by the @Controller annotation.

**@Controller Annotation:** Are classes that are responsible for preparing a model map with data and selecting a view to be rendered. This model map allows for the complete abstraction of the view technology.

GET request is used to return  a view. view is responsible for rendering the HTML content.
1. @GetMapping:  annotation ensures that HTTP GET requests are mapped to the greeting() method.
2. @RequestParam binds the value of the query string parameter name into the name parameter of the greeting() method. This query string parameter is not required. If it is absent in the request, the defaultValue of World is used. The value of the name parameter is added to a Model object, ultimately making it accessible to the view template.

3. to perform server-side rendering of the HTML. Thymeleaf parses the greeting.html template and evaluates the th:text expression to render the value of the ${name} parameter that was set in the controller.

## Spring boot Devtools:
A common feature of developing web applications is coding a change, restarting your application, and refreshing the browser to view the change. This entire process can eat up a lot of time. To speed up this refresh cycle, Spring Boot offers with a handy module known as spring-boot-devtools. Spring Boot Devtools:
1. Enables hot swapping.
2. Switches template engines to disable caching.
3. Enables LiveReload to automatically refresh the browser.
4. Other reasonable defaults based on development instead of production.

## Hot Swapping:
1. It  Reload Static Content: This means that static resource changes must be "built" for the change to take effect. By default, this happens automatically in Eclipse when you save your changes. In IntelliJ IDEA, the Make Project command triggers the necessary build.

2.  Reload Templates without Restarting the Container: Most of the templating technologies supported by Spring Boot include a configuration option to disable caching.
Number of templates:
 * Thymeleaf Templates: Is to set spring.thymeleaf.cache to false.
 * FreeMarker Templates: set spring.freemarker.cache to false.
 * Groovy Templates: set spring.groovy.template.cache to false.

3.  Fast Application Restarts.
4. Reload Java Classes without Restarting the Container.


## Thymeleaf context object:
it makes all the defined variables available to expressions executed in templates.

What is the Spring model Attributes ??
It calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.

There are several ways of adding model attributes to a view in Spring MVC. Below you will find some common cases:
1. Add attribute to Model via its addAttribute method
2. Return ModelAndView with model attributes 
3. Expose common attributes via methods annotated with @ModelAttribute

## Requesting Parameters:
can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server.

## Session attributes:
Similarly to the request parameters, session attributes can be accessed by using the session. prefix. Or by using #session, that gives you direct access to the javax.servlet.http.HttpSession object.

## ServletContext attributes:
are shared between requests and sessions. In order to access ServletContext attributes in Thymeleaf you can use the #servletContext. prefix.

## Spring Beans:
Thymeleaf allows accessing beans registered at the Spring Application Context with the @beanName syntax,
