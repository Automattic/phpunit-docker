# PHPUnit image for Docker

This repository contains a Docker image with PHPUnit 7.5. It is based in Alpine 3.12. The image is published in GitHub Packages. To use it:

```
docker pull ghcr.io/automattic/phpunit-docker/phpunit:latest
```

## Building

The image is automatically built by a GitHub action and published to GitHub Packages. To build it locally, clone this repository and:

```
cd phpunit-docker
docker build . -t phpunit
```
