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

docker commands:
------------------
sudo docker build -t veerimage:v1 .
sudo docker tag veerimage:v1 docker.io/veer18/veerimage:v1
sudo docker push  docker.io/veer18/veerimage:v1
sudo docker rm -f myos1
sudo docker pull veer18/veerimage:v1
sudo docker run --name myos1 -dit -p 80:80 veer18/veerimage:v1
sudo curl http://13.127.72.86/| grep 'welcome'
if [$? == 0]
then
  exit 0
else
  exit 1
fi
