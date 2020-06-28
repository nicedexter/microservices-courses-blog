# Log

minikube start
eval $(minikube docker-env)

k delete pod posts
k apply -f posts-depl.yaml
k get deployments
k describe deployment posts-depl
k delete deployment posts-depl

docker build -t nicedexter/posts .
k rollout restart deployment posts-depl

minikube addons enable ingress
kubectl get pods -n kube-system

k apply -f ingress-srv.yaml
sudo /etc/hosts
