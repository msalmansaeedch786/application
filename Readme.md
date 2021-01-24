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

6. Access Application

```bash
minikube service easynotes-service
```

## Tutorial
You can find the tutorial for this application at [The CalliCoder Blog](https://www.callicoder.com) - 

<https://www.callicoder.com/node-js-express-mongodb-restful-crud-api-tutorial/>