# Jinja2-Linter

[![Container Release (j2lint)](https://github.com/leberkaslabs/docker-image-j2lint/actions/workflows/build-push-action.yml/badge.svg)](https://github.com/leberkaslabs/docker-image-j2lint/actions/workflows/build-push-action.yml)

This repository is designed to build Docker images for [j2lint](https://github.com/aristanetworks/j2lint).

```bash
docker pull dudecalledbro/j2lint:latest
```

## Usage

You can easily run `j2lint` using Docker, which provides cross-platform solution for linting your Jinja2 files. Simply pipe your Jinja2 file into the Docker container with the following command:

```bash
docker run --rm -i dudecalledbro/j2lint:latest < $JINJA_FILE
```

This will run `j2lint` on your Jinja2 fle without needing to install anything locally.

## Build

This image build is scheduled with GitHub Actions and will be pushed to DockerHub. The image will also be rebuilt, if the `main` branch is updated. If you need to build the image locally, ensure [Docker](https://docs.docker.com/engine/installation/) is installed and execute the following:

```bash
docker build -t j2lint:latest .
```

## License

Copyright © 2025 Niclas Spreng

Licensed under the [MIT license](LICENSE).
