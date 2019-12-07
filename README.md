# flask-docker

Build the image

`docker build -t test .`

Here, the `-t` flag is an alternate way of writing --test.

Run the container with the following command:

`docker run  -p 80:8080 test`

In this command, you are binding port 8080 of the container to the port 80 of your local machine. The flask application

Curl the endpoint
`curl http://0.0.0.0/`

When you are finished, get the id of the running container:

`docker ps`

You can then use the id to stop the container:

`docker stop <Container Id>`

### Note
Summary
In this concept, you practiced building two Docker containers from Dockerfiles. You also learned or revisited some of the commands and flags that are useful for this process, including:

docker build which will build an image based on a Dockerfile.

The `--tag` flag, which is used to name the image.

The docker run command, which is used to run a container based on the image.

The `-p` flag can be used to map container ports to host machine ports.