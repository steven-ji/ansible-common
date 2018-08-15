## ansible-common
一些通用的ansible playbook剧本.
## Describe all file
+ docker
docker.yml: Install docker-ce.Could specific docker-ce version use variable docker_version.
docker_login.yml: Use to docker login credential.Should explicit point username by "registry_username" and password by "registry_password".
+ kubernetes


## Usage
### Install docker
```
# Install docker(default docker version is set in docker.yml)
# Could special version by use --extra-args(or -e)
$ ansible-playbook -i hosts -e "docker_version=docker-ce-18.06.0.ce" docker/docker.yml
```
### Set of credential
```
$ ansible-playbook -i hosts -e "registry_username=yourname registry_password=passwd" docker/docker_login.yml
```
### Install shadowsocks+privoxy
``` 
$ ansible-playbook -i hosts shadowsocks/shadowsocks.yml
```
