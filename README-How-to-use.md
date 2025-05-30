minikube start
eval $(minikube docker-env)
docker build -t fastapi-app:latest .
kubectl apply -f k8s-deployment.yaml