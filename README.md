# java-servlets
### Description
This app demonstrates how to use servlets in Spring-Boot
### Procedure
Create a "demo" template using Spring Initializr. Navigate to Spring Initializr at [Spring Initializr](https://start.spring.io/), then select Maven, and add the "Spring Web" dependency. Click on the Generate button to download the template

![Spring Initializr](https://raw.githubusercontent.com/mmackenzie-syd/java-servlets/main/spring-boot-initiliser.png)

Add the "@ServletComponentScan" annotation to the DemoApplication class as shown:

![DempApplication Class](https://raw.githubusercontent.com/mmackenzie-syd/java-servlets/main/demo-application.png)

Add the "Location" class which extends the "HttpServlet" class as shown:

![Location Class](https://raw.githubusercontent.com/mmackenzie-syd/java-servlets/main/location.png)

### Running the App
You can run the application by using 
```
./mvnw spring-boot:run
```
Alternatively, you can build the JAR file with 
```
./mvnw clean package
``` 
and then run the JAR file, as follows:
```
java -jar target/gs-serving-web-content-0.1.0.jar
```
In a browser, navigate to localhost:8080/location to view the servlet response.

### References:
https://stackoverflow.com/questions/55978959/how-can-i-register-a-servlet-with-spring-boot
