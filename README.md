CI Image: Go
============

This repo contains a Dockerfile for building a [Docker] image that can be used to build and test Go apps in a CI environment.
It's originally designed to work with Circle CI 2.0, however, may fit other CI systems too.

This image is based on official [golang] image, but additionally includes:

- [Masterminds/glide] for dependency management;
- [jstemmer/go-junit-report] for converting `go test` output to JUnit format;
- [docker] for building a docker images with compiled binary;
- [Google Cloud SDK] for pushing built Docker images to Google Cloud.


[//]: # (These are reference links used in the body of this document)

[Docker]: <http://docker.com/>
[golang]: <https://hub.docker.com/_/golang/>
[Google Cloud SDK]: <https://cloud.google.com/sdk/gcloud/>
[Masterminds/glide]: <https://github.com/Masterminds/glide>
[jstemmer/go-junit-report]: <https://github.com/jstemmer/go-junit-report>