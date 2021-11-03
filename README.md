# Spring Boot Hello World App

This is a service that accepts HTTP GET requests at

```sh
curl http://localhost:8080/greeting
```

It will respond with a JSON representation of a greeting, as the following listing shows:

```json
{ "id": 1, "content": "Hello, World!" }
```

You can customize the greeting with an optional `name` parameter in the query string, as
the following listing shows:

```sh
curl http://localhost:8080/greeting?name=User
```

The `name` parameter value overrides the default value of `World` and is reflected in the
response, as the following listing shows:

```json
{ "id": 1, "content": "Hello, User!" }
```

## Running the Application

To start the application execute the Maven script:

```sh
./mvnw spring-boot:run
```

## Credits

This app is one of the Spring Boot examples at [Spring: Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/#initial)
