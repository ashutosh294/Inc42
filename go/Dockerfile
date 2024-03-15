# Use an official Golang runtime as a parent image
FROM golang:1.17-alpine

# Set the working directory inside the container
WORKDIR /go

# Copy the local package files to the container's workspace
COPY . .

# Build the Go application
RUN go build -o myapp

# Expose the port on which the service will run
EXPOSE 8080

# Command to run the executable
CMD ["./myapp"]
