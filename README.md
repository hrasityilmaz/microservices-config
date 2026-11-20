
# Microservices Configuration

Centralized configuration repository for the **Spring Cloud Microservices** project.

Main Repository: [spring-cloud-microservices](https://github.com/hrasityilmaz/spring-cloud-microservices)

This repository stores externalized configuration properties for all microservices. Config server reading from this repo.



| File | Description |
|---|---|
| `api-gateway.properties` | API Gateway configuration |
| `users-ws.properties` | Users Service configuration |
| `todos-ws.properties` | Todos Service configuration |


Example client configuration:

```properties
spring.application.name=users-ws
spring.config.import=configserver:http://localhost:8012
```
