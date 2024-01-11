This directory contains:

- `main.go` contains the HTTP server implementation. It responds to all HTTP
  requests with a  `Hello, world!` response.
- `Dockerfile` is used to build the Docker image for the application.

```
go version
go help version
go mod init
go mod init v1
go mod tidy
```

```
package main

import "fmt"

func main() {
    fmt.Println("Hello World!")
}
```
```
go build -o hello-world
```
```
go version hello-world
```
```
package main

import (
    "fmt"
    "runtime"
)

func main() {
    fmt.Println("Hello World!")
    fmt.Printf("The application was built with the Go version: %s\n", runtime.Version())
}
```
```
go build -o hello-world-with-version
```
```
go build -o hello-world-with-version
```
```
./hello-world-with-version
```

cd D:/Project
ls
mkdir k8sApp
cd k8sApp
clear
git clone https://github.com/GoogleCloudPlatform/kubernetes-engine-samples
ls
docker build -t hello-app:v1 .
docker build -t hello-app:v1 .
docker images
docker run -d -p 8080:8080 hello-app:v1
docker logs 14a9ca29ced83

http://localhost:8080/