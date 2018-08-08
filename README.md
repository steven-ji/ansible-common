# ansible-common
一些通用的ansible playbook剧本.
# Usage
```
# Install docker(default docker version is set in docker.yml)
# Could special version by use --extra-args(or -e)
$ ansible-playbook -i hosts -e "docker_version=docker-ce-18.06.0.ce" docker/docker.yml
```
