#Docker installation

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
docker ps -a
```

### Copy files from host to container
```sh
docker cp file container:/path/to/copy/file
```
