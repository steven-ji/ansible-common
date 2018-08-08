## Install kubernetes master
```
# Pre Install Docker(Default Docker version set in group_vars/docker).
# Could cover docker version by use --extra-vars(or -e) point version.
$ ansible-playbook -i hosts -t docker -e "docker_version=docker-ce-18.06.1.ce" site.yml
# Install kubeadm
$ ansible-playbook -i hosts -t master site.yml
```
