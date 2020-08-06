# prometheus-client-golang

A simple app that implements the corresponding packages to [export metrics](https://prometheus.io/docs/instrumenting/clientlibs/) to Prometheus.

## Build and run with Docker

```sh
go mod vendor
docker build -t prometheus-client-golang .
docker run --rm -it -p 8080:8080 prometheus-client-golang
```

Metrics accessible through `http://localhost:8080/metrics`