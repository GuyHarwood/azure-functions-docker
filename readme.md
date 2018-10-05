# Dockerized Azure Functions

Simple example of azure function app in a container.

## Instructions

open terminal and run the commands below.  Be sure to replace `your-storage-connection-string` with your actual Azure storage connection string.

```
func extensions install
docker build -t dockerfunctions .
docker run -p 8080:80 -e StorageConnection='your-storage-connection-string' dockerfunctions
```
