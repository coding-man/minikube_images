minikube image for china user!
for version v0.19.1

1.start minikube with DaoCloud 
minikube start --registry-mirror=http://44d249ac.m.daocloud.io

2.pull image and tag it
docker pull dockermonster/pause-amd64:3.0
docker tag dockermonster/pause-amd64:3.0 gcr.io/google_containers/pause-amd64:3.0

docker pull dockermonster/kube-addon-manager:v6.4-beta.1
docker tag dockermonster/kube-addon-manager:v6.4-beta.1 gcr.io/google-containers/kube-addon-manager:v6.4-beta.1

docker pull dockermonster/echoserver:1.4
docker tag dockermonster/echoserver:1.4 gcr.io/google_containers/echoserver:1.4
