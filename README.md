# Eureka Server

Simple eureka server. 

## Build Docker Image

```
gradle bootBuildImage
```

## Run Docker Image

```
DOCKER_HOST=tcp://valery2014.local:2375
docker run -p 8761:8761 eureka:0.0.1
```

Note: Docker context is not visible inside gradle tasks, need to specify envrironment
variable DOCKER_HOST.


## Links

- [Service Registration and Discovery](https://spring.io/guides/gs/service-registration-and-discovery/)
- [Spring Cloud Netflix](https://spring.io/projects/spring-cloud-netflix)





