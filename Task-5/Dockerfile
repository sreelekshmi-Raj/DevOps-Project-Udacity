# Docker file for go-helloworld:v2.0.0
# Docker file for go-helloworld:v1.0.0 in the Task-3 folder
# use the golang:alpine base image
FROM golang:alpine

# set the working directory to /go/src/app
WORKDIR /go/src/app

# copy all the files from the current directory to the container working directory
ADD . .

# import dependencies using `go mod init` and build the application using `go build -o helloworld` command
RUN  go mod init && go build -o helloworld

# expose the port 6112 for the application app:v2.go
EXPOSE 6112

# start the container
CMD ["./helloworld"]