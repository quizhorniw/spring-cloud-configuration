### Usage in Spring Cloud Config Server

To use these property files in your Config Server project, you have to add this Maven dependency:
```
<dependency>
  <groupId>org.springframework.cloud</groupId>
  <artifactId>spring-cloud-config-server</artifactId>
</dependency>
```

Also, you have to provide URL to this GitHub repo in your `application.yaml`:
```
spring:
  cloud:
    config:
      server:
        git:
          uri: https://github.com/quizhorniw/spring-cloud-configuration
```
or similarly using `application.properties`:
```
spring.cloud.config.server.git.uri=https://github.com/quizhorniw/spring-cloud-configuration
```
