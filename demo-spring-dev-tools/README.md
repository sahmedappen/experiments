Example for a REST-enabled Spring Boot application with spring-dev-tools restart ability 

# Prerequisites
1. Added the following dependency in your spring boot project build.gradle dependencies

```
 developmentOnly('org.springframework.boot:spring-boot-devtools')
```

2. Running

   - To build ./gradlew clean build 
   - To run ./gradlew bootRun 
   - Access http://localhost:8080/v1/greetings?name="syed" and see it outputs "Hello syed"
   
3. Make a code change and the boot app is re-initialized automatically
   - Go to DemoController class and change the display text from "Hello" to "Hi" 
   - build the project ./gradlew clean build in separate terminal tab 
   - see that spring boot is reinitializing & http://localhost:8080/v1/greetings?name="name"
      outputs now "Hi Syed"


# Resources
* [Spring Boot Dev Tools](https://docs.spring.io/spring-boot/docs/1.5.16.RELEASE/reference/html/using-boot-devtools.html)



