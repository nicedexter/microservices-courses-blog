# Log

minikube start
eval \$(minikube docker-env)
kubectl apply -f posts.yaml
kubectl get pods
kubectl describe pod posts
