## Prerequisites
### #Step 1 Install docker
ref: [install docker](https://docs.docker.com/engine/installation/)

### #Step 2 Install composer
ref: [install composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

### #Step 3 Setting up docker
1. create docker machine via 
   run ```"docker-machine create --driver virtualbox default"``` and then
   run ```"eval $(docker-machine env default)"``` for activate machine and then
   run ```"docker-machine ip default"``` for check machine ip we will use this ip to access others services

2. 