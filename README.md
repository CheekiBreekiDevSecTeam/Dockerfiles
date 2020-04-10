# Docker installation

```sh
 sudo apt install docker docker.io -y
```
### To run the docker service./* Ubuntu run the service when booting */
```sh
sudo service docker start
```

### To see the images on your system
```sh
sudo docker images
```

### List all containers
```sh
sudo docker ps -a
```

### Copy files from host to container
```sh
sudo docker cp file container:/path/to/copy/file
```
### Remove all stopped containers
```sh
sudo docker rm $(docker ps -a -q)
```
