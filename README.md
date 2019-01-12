# Anisble Docker Example
----
Instead testing playbooks in VM , testing can be done in docker container in local before we move it to any target environment.


## To Run Container
```sh
$ git clone https://github.com/jrsaravanan/ansible-docker.git
$ cd ansible-docker
$ sudo docker build -t ubuntu-ssh .
$ ./start.sh
```

## To Execute 
```sh
$ ansible-playbook -i inventory/local playbooks/echo.yml
```

## To Stop and Remove
```sh
$ sudo docker stop ansible_test_host
$ sudo docker rm ansible_test_host
```
