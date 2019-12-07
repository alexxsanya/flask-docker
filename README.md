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

Flask Application Dock