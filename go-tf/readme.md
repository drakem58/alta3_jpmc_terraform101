The objective of this lab is to introduce deploying a Go microservice with Terraform. Docker provides the ability to package and run an application in a loosely isolated environment called a, container. The isolation and security allow you to run many containers simultaneously on a given host. Containers are not exclusive to Docker, other Container Runtime Environments exist, such as rkt and containerd, however, Docker is by far the most popular.

The application we will build will mimic a RESTful microservice. This minimal HTTP server has only three (3) features:

HTTP GET sent to / returns a heart symbol (<3) via a 200 OK
HTTP GET sent to /ping returns simple health reports in the form of simple JSON, {"Status" : "OK"}
HTTP GET sent to /spock returns Spock's response in a simple JSON format, {"Status" : "Live long and prosper"}
The port it listens on is configurable using the environment variable HTTP_PORT. The default value is 9876.
For simplicity's sake, this lab is broken into several phases. Feel free to take a break between each phase.

Resources:

Docker
Docker Hub
GitHub.com - Labstack "Echo" HTTP Server
