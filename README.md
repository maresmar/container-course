# Containers practice

Sources for practice lecture about containers used in NSWI026 MFF UK and SEPA4M33SEP, FEL CVUT. This should be a simple example for containers, it's not recommended for a production usage.

## Tasks

1. Run image `quay.io/podman/hello`
    - https://learnxinyminutes.com/docs/docker/

2. Create a Dockerfile that run `apache2` in Debian Linux
    - Serve a html file from `task_2` folder on <http://localhost:8090/>
    - Use command `apachectl -D FOREGROUND`, install `apache2`
    - Try it on <http://localhost:8090/>

3. Try a Redis + Flask with podman-compose
    - Use a compose from `task_3` or fetch https://github.com/docker/awesome-compose/tree/master/flask-redis
    - Try it on <http://localhost:8000/>

4. Crate own image for FlightLog
    - Java - https://spring.io/guides/topicals/spring-boot-docker/ 
    - .NET - https://learn.microsoft.com/en-us/dotnet/core/docker/build-container
