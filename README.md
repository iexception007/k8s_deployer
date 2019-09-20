#  install kubernetes and components
## compoents or module
* base env.
* yum-repo
* pip-repo
* harbor
* etcd
* k8s
* helm
* jenkins
* nats
* mysql
* redis

## execute setp. 
excute <install.sh>  in my mac. with only one <config.yaml> file. 
### setp 1. reset the hosts. 
### setp 2. download the docker images.
### setp 3. install docker, setting the network. time sync close.swap.
jq, yq ansible ansibe-playbook.
run yum-repo  
run pip-repo  
run harbor  
### setp 4. Push image to the harbor
### setp 5. install k8s
### setp 6. install helm
### setp 7. install other compnents.

## usage.
```
./install.sh reset     | esxi snapshot
./install.sh pull      | download the docker images.
./install.sh prev      | install docker, setting the network...
                       | run yum-repo and pip-repo
                       | run harbor
./install.sh push      | push the docker images to the harbor
./install.sh -c k8s    |
./install.sh -c mysql  | install one specail compoent
./install.sh -c redis
./install.sh           
```