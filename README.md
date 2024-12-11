# Containers practice

Sources for practice lecture about containers used in NSWI026 MFF UK and SEPA4M33SEP, FEL CVUT. This should be a simple example for containers, it's not recommended for a production usage.

## Tasks

1. Run the image `quay.io/podman/hello`
    - Refer to https://learnxinyminutes.com/docs/docker/

2. Create and run simple web server
    - Create a `Dockerfile` in the `task_2` folder 
    - Select Debian Linux as your base image
    - Install the `apache2` package
    - Use the command `apachectl -D FOREGROUND` to start the server
    - (Optional) Try to serve an HTML file from the `task_2` folder by coping it to `/var/www/html` in the image
    - Build the image using `task_2` folder
    - Run container
        - Apache runs on port 80 in the container; map this port to 8080 on your machine
        - Try it on <http://localhost:8080/>

3. Try a Redis + Flask with podman-compose
    - Use a compose file from `task_3` or fetch https://github.com/docker/awesome-compose/tree/master/flask-redis
        - Use `podman compose up` in folder `task_3`
    - Review files in the `task_3` folder
    - Try it at <http://localhost:8000/>

4. Crate own image for FlightLog
    - Java - https://spring.io/guides/gs/spring-boot-docker
    - .NET - https://learn.microsoft.com/en-us/dotnet/core/docker/build-container
