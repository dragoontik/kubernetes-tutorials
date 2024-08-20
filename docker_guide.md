


### List all docker containers
> docker ps -a

### List all docker images 
> docker image ls

### Pull down an OS interactivly via a terminal (example)
### This example pulls down the latest tag of arch linux and start a bash terminal
> docker run -it --name archenv archlinux /bin/bash

#### Following example does the same but for a nodejs image
> docker run -it --name node16 node:16 /bin/bash