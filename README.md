# Fedora 37 Ansible Test Image

[![GitHub Actions](https://github.com/MonolithProjects/docker-systemd-fedora37/workflows/Dockerfile%20test/badge.svg?branch=master)](https://github.com/MonolithProjects/docker-systemd-fedora37/actions)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-fedora37)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora37)
[![DockerHub-pulls](https://img.shields.io/docker/pulls/monolithprojects/systemd-fedora37)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora37)
[![DockerHub](https://img.shields.io/docker/image-size/monolithprojects/systemd-fedora37?sort=date)](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora37)

Docker image with Fedora 37 and enabled systemd. Image is updated with the latest software updates on the 1st day in the month. Image contains also `ansible` user (UID/GID 1000) with NOPASSWD:ALL sudo rights.  

**Note:** This docker image is ment to be used for Molecule Ansible tests and development purpose. I do not recomend to use it in production.

## Tags

- `latest`  
- `<monthly build timestamp>` for the list of the tags see the [Docker Hub](https://hub.docker.com/repository/docker/monolithprojects/systemd-fedora37/tags?page=1)

## How-to

  1. Pull image with command `docker pull monolithprojects/systemd-fedora37:latest`  
  2. Run the container from the image: `docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro monolithprojects/systemd-fedora37:latest`  

## License

MIT
