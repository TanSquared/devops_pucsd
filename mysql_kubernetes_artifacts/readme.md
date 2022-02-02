## Task : Create MYSQL database on kubernetes using kubernetes artifact files

### Steps Followed:
1. Create a namespace 
2. Set the current namesapce to the one you created
3. Create db-secret
4. Create configmap
5. Create deployment
6. Create service

Code for the steps:
```
kubectl create namespace demo
kubectl config set-context --current --namespace=demo
kubectl create -f secret.yaml
kubectl create -f configmap.yaml
kubectl create -f db-deployment.yaml
kubectl get pods --watch
```

![](./'mysql_artifacts 1.png')
