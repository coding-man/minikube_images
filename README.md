minikube image for china user!
for version v0.19.1

~~~start minikube with DaoCloud 

minikube start --registry-mirror=http://44d249ac.m.daocloud.io

~~~pull image and tag it

docker pull dockermonster/pause-amd64:3.0
docker tag dockermonster/pause-amd64:3.0 gcr.io/google_containers/pause-amd64:3.0

docker pull dockermonster/kube-addon-manager:v6.4-beta.1
docker tag dockermonster/kube-addon-manager:v6.4-beta.1 gcr.io/google-containers/kube-addon-manager:v6.4-beta.1

docker pull dockermonster/echoserver:1.4
docker tag dockermonster/echoserver:1.4 gcr.io/google_containers/echoserver:1.4

docker pull dockermonster/kubernetes-dashboard-amd64:v1.6.1
docker tag dockermonster/kubernetes-dashboard-amd64:v1.6.1 gcr.io/google_containers/kubernetes-dashboard-amd64:v1.6.1

docker pull dockermonster/k8s-dns-kube-dns-amd64:1.14.2
docker tag dockermonster/k8s-dns-kube-dns-amd64:1.14.2 gcr.io/google_containers/k8s-dns-kube-dns-amd64:1.14.2

docker pull dockermonster/k8s-dns-dnsmasq-nanny-amd64:1.14.2
docker tag dockermonster/k8s-dns-dnsmasq-nanny-amd64:1.14.2 gcr.io/google_containers/k8s-dns-dnsmasq-nanny-amd64:1.14.2

docker pull dockermonster/k8s-dns-sidecar-amd64:1.14.2
docker tag dockermonster/k8s-dns-sidecar-amd64:1.14.2 gcr.io/google_containers/k8s-dns-sidecar-amd64:1.14.2
