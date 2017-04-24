# Docker Study
### Mounting a folder from host to boot2docker
1. in docker-machine VM, create a shared file mapping of local folder to guest(VM) folder. E.g. D:/projects/docker to docker-projects
2. `docker-machine ssh`
3. `sudo -i` to get root access
4. `vi /var/lib/boot2docker/profile`
5. add in `sudo mkdir -p /docker-projects && mount -t -vboxsf docker-projects /docker-projects`
6. exit docker-machine
7. `docker-machine restart` to take effect

### Install docker-compose in boot2docker
1. docker-compose does not come by default
2. `docker-machine ssh <machine-name> < install-docker-compose.sh`