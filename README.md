# WAR files with Spring Boot

This is the code developed in the tutorial on deploying Spring Boot apps as a WAR.

It modifies an existing simple REST app https://github.com/stormpath/stormpath-spring-boot-jpa-example

### Requirements

- Maven
- JDK 7
- Tomcat 7

### Running

To build and start the server simply type

```sh
$ mvn spring-boot:run
```

from the root directory.

### Deploying on Tomcat

TODO

### Using

You can see what urls are available using curl:

```sh
$ curl localhost:8080
```

You can view existing people objects using a similar request:

```sh
$ curl localhost:8080/persons
```

and can create new ones using a POST:

```sh
$ curl -x POST -H "Content-Type:application/json" -d '{ "firstName" : "Karl", "lastName" : "Penzhorn" }' localhost:8080/persons
```

### Todo

 - Different build profiles

### License
----

MIT
