# Kubernetes-Tutor
## Kubernetes Training for Beginners

### Description
This is a simple Demo Project for running and deploying web app(MongoDB+MongoExpress) from TechWorld with Nana (https://www.youtube.com/watch?v=X48VuDVv0do&t=3414s)


### Implementation
Below are the terminal commands that are needed to run the app.
Also it is running with docker desktop (instead of minikube)

- Create deployments/services and other components

1. kubectl apply -f mongo-secret.yaml
2. kubectl apply -f mongo-configmap.yaml
3. kubectl apply -f mongo.yaml
4. kubectl apply -f mongo-express.yaml

- Check all deployments/services/pods with

kubectl get pods | deployment | service | secret | configmap

kubectl describe pods | service

kubectl logs <pod_name>


- Delete components

1. kubectl delete -f mongo-secret.yaml
2. kubectl delete -f mongo-configmap.yaml
3. kubectl delete -f mongo.yaml
4. kubectl delete -f mongo-express.yaml

### - Run the App
open in browser the url http://localhost:8081
