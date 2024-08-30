# jenkins_training_2024_docker

master - slave architectures
master - jenkins master node
slave 1 - docker build node
slave 2 - docker test node
slave 3 - kubernetes node

master and slave nodes should have java in it..
slave 1 - docker,git should install
slave 2 - docker
slave 3 - kubectl , --> master(k8's) using admin.conf file

docker -  need to have login for the frist time manually......

vi /etc/sudoers.d/ -- privalage escalation
nopasswd
