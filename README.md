# Eureka Server

Simple eureka server. 

## Set docker environment

If docker installed on remote host set `DOCKER_HOST` environment variable.

For tcp setup:
```
export DOCKER_HOST=tcp://computername:2375
```

or for ssh setup: 

```
export DOCKER_HOST=ssh://computername
```

Note: Docker context , doesn't work for gradle bootBuildImage. But of course 
you can use docker context for run docker or run with docker compose.


## Build Docker Image

```
gradle bootBuildImage
```

## Run Docker Image

```
docker run -p 8761:8761 eureka:0.0.1
```

Note: Docker context is not visible inside gradle tasks, need to specify
envrironment variable DOCKER_HOST.


## Links

- [Service Registration and Discovery](https://spring.io/guides/gs/service-registration-and-discovery/)
- [Spring Cloud Netflix](https://spring.io/projects/spring-cloud-netflix)





