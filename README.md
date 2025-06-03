Deploy NGINX Web Server on Kubernetes (Docker CLI + kubectl)

To run this file:
1) kubectl apply -f deployment.yaml
Verify it is running:
kubectl get pods
kubectl get deployments
2) kubectl expose deployment my-app --type=NodePort --port=80
3) kubectl get svc or minikube service my-app
