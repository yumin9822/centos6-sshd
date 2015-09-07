# centos6-sshd
Dockerized SSH service, built on top of official centos6 images.

## Installed packages

openssh-server

## Config:

PermitRootLogin yes

UsePAM no

exposed port 22

default command: /usr/sbin/sshd -D

root password: p@ssw0rd99

## Run example
```
$ sudo docker run -d -P --name my_sshd yumin9822/centos6-sshd:latest
$ sudo docker port my_sshd
  0.0.0.0:49181
```
