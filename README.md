# Pet_Store_Assignment
This application is using Quarkus. To run and build the appication follow the below instructions.

## Packaging and running the application
### The application can be  packaged using:
```
  ./gradlew build
```
### To run the application:
```
  java -jar build/petstore-runner.jar
```
### To launch the test page, open your browser at the following URL
```
  http://localhost:8080
```
### To see all the endpoints 
```
  http://localhost:8080/swagger-ui/#/
```
** Can test all the enpoints and execute the using the swagger.

## Build Docker Container

### Before building the container image run:
```
  ./gradlew build
```
### Then, build the image with:
```
  docker build -f src/main/docker/Dockerfile.jvm -t quarkus/code-with-quarkus-jvm .
```
### Then run the container using:
```
  docker run -i --rm -p 8080:8080 quarkus/code-with-quarkus-jvm
```



