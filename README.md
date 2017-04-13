# Dockerise my web app based on Spring Boot and Gradle


### Build an app from source and create Docker image

```
$ ./gradlew clean bootRepackage -Pprod buildDocker
```

### Run the container with the created image

```
$ docker run -it -p 9191:9191 --name myapp myapp:latest /bin/sh
```

### Find VM IP address 

```
$ docker-machine ip default
192.168.99.100
```

### Launch the deployed app 

```
/# java -jar app.jar
```

```
http://192.168.99.100:9191/
```





