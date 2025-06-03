Deploy NGINX Web Server on Kubernetes (Docker CLI + kubectl)
(Without a Service, you have no stable way to access the app — either from your machine or from another app in the cluster.
It will run with just deployment but it is poor practice and not ideal in a real world situation.)

To run:
1) kubectl apply -f deployment.yaml
2) kubectl apply -f service.yaml
Verify it is running:
kubectl get pods
kubectl get deployments
3) kubectl expose deployment my-app --type=NodePort --port=80
4) kubectl get svc or minikube service my-app
