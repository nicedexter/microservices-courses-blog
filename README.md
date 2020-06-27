# Log

minikube start
eval \$(minikube docker-env)

k delete pod posts
k apply -f posts-depl.yaml
k get deployments
k describe deployment posts-depl
k delete deployment posts-depl
