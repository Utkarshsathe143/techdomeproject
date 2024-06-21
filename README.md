

Architecture

Frontend: React application served on port 3000.
Backend: Express server on port 5000.
Database: MongoDB instance on port 27017.

Deployment Strategy

 Docker Compose : Define the multi-container setup locally.
 Kubernetes : Deploy each container with its dependencies in a Minikube cluster.


Docker Compose
Run docker-compose up

Kubernetes

type minikube start
Apply the Kubernetes files:

   kubectl apply -f backend-deployment.yaml
    kubectl apply -f frontend-deployment.yaml
   kubectl apply -f database-deployment.yaml
   kubectl apply -f mongo-pvc.yaml
