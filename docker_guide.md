


### List all docker containers
> docker ps -a

### List all docker images 
> docker image ls

### Pull down an OS interactivly via a terminal (example)
### This example pulls down the latest tag of arch linux and start a bash terminal
> docker run -it --name archenv archlinux /bin/bash

#### Following example does the same but for a nodejs image
> docker run -it --name node16 node:16 /bin/bash

### Starting simple container and binding a port (indiefold-frontend is an image)
#### docker run -p [hostport:engineport] [image_name] 
> docker run -p 3000:3000 indiefold-frontend


#### Run a container in detached mode (indiefold-frontend is an image)
> docker run -p 3000:3000 -d indiefold-frontend

### Attache to a running container <em> Can also use container id instead of name</em>
> docker attach [container_name]

### Can also attach and follow to see logs
> docker log -f [container_name]

### or start in attached mode
docker start -a [container_name]

### starting a type of docker container that takes input
> docker run -it [image_name]

### restarting an existing container in interactive mode w/ user input
> docker start -a -i [container_name]


### flag to automatically remove containers when they exit (--rm)
> docker run -p 3000:80 -d --rm [image_id]

### look into images metadata
> docker image inspect [image_id]

### Copy a file into a container
> docker cp [host_file_or_dir_path] [container_name]:[container_path]

### Copy a file/dir from container to host
> docker cp [container_name]:[container_file_or_dir] [host_file_or_dir_path]
