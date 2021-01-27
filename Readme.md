# EasyNotes Application

Build a Restful CRUD API for a simple Note-Taking application using Node.js, Express and MongoDB.

## Steps to Setup

1. Install dependencies

```bash
npm install
```

2. Run Server

```bash
node server.js
```
You can browse the apis at <http://localhost:3000>

3. Compose Deploymennt

```bash
docker-compose up

docker-compose down
```

4. Minikube Cluster

```bash
minikube start --network-plugin=cni --cni=calico
```
Start minikube using above command to enable calico

5. Kubernetes Deploymennt

```bash
kubectl apply -f ./Deployments

kubectl delete -f ./Deployments
```

6. Helm Deployment

```bash
helm install mongodb-chart ./helm-chart/charts/mongodb/ -f ./helm-chart/values.yaml

helm install easynotes-chart ./helm-chart/charts/easynotes/ -f ./helm-chart/values.yaml



helm uninstall mongodb-chart easynotes-chart
```

7. Access Application

```bash
kubectl get services

minikube service <service_name>
```

## Tutorial
You can find the tutorial for this application at [The CalliCoder Blog](https://www.callicoder.com) - 

<https://www.callicoder.com/node-js-express-mongodb-restful-crud-api-tutorial/>