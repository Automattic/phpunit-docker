# PHPUnit image for Docker

This repository contains a Docker image with PHPUnit 7, 8 and 9. They are all based on Alpine 3.12. The three images are build on GitHub Actions and published in GitHub Packages. To use it:

```bash
# PHPUnit 7
docker pull ghcr.io/automattic/phpunit-docker/phpunit:7

# PHPUnit 8
docker pull ghcr.io/automattic/phpunit-docker/phpunit:8

# PHPUnit 9
docker pull ghcr.io/automattic/phpunit-docker/phpunit:9

```

By default (and due to historical reasons), the `latest` version is `7`

```bash
# PHPUnit 7
docker pull ghcr.io/automattic/phpunit-docker/phpunit:latest
```

## Building

The image is automatically built by a GitHub action and published to GitHub Packages. To build it locally, clone this repository and:

```bash
cd phpunit-docker

# PHPUnit 7
docker build . -t phpunit:7 -f 7/Dockerfile

# PHPUnit 8
docker build . -t phpunit:8 -f 8/Dockerfile

# PHPUnit 9
docker build . -t phpunit:9 -f 9/Dockerfile
```
