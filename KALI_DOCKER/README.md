# Kali Docker

## Build and run image 
```sh
sudo docker build -t kali_image .
sudo docker run -it  kali_image /bin/bash
```
## Create Image
When exiting the container you can save the container as your image with
```sh
sudo docker commit container-id or image_tag Image_name_you_want_to_give
```

Example: 
```sh
sudo docker commit {a3f41572ce6f || kali_image} kali/kalimage
```

To start a container when booting again run:
```sh
sudo docker start image_name
sudo docker attach image_name
```
