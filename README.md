# java-baseimage

This is a base docker image for Java applications.  Currently this image will have installed:

* Java 8

This image is build off of [debian](https://registry.hub.docker.com/_/debian/)

This image is available on Dockerhub ([here](https://registry.hub.docker.com/u/broadinstitute/java-baseimage/))

An example of a Dockerfile which utilizes this image:

```
FROM broadinstitute/java-baseimage

COPY helloworld.jar /usr/helloworld.jar
WORKDIR /usr

ENTRYPOINT ["java", "-jar", "helloworld.jar"]
```
