# Docker Study
### Mounting a folder from host to boot2docker
1. in docker-machine VM, create a shared file mapping of local folder to guest(VM) folder. E.g. D:/projects/docker to docker-projects
2. `docker-machine restart` to take effect

### Install docker-compose in boot2docker
1. from the mount folder, git checkout this repository
2. go to https://github.com/docker/compose/releases and look for the latest release
3. change sh/install-docker-compose.sh DOCKER_COMPOSE_VERSION to latest release
4. ssh into the docker-machine
5. go to the sh folder, `cd ${mount_folder}/docker-study/sh`
6. then `chmod +x install-docker-compose.sh` to make it executable
6. to run the shell `sh install-docker-compose.sh`s

