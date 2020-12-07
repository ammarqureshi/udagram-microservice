# udagram-microservice

A simple image sharing AWS cloud application.


* Frontend - Angular web application built with Ionic Framework
* Backend RESTful API - Node-Express application
    * Feed Service - handles image feeds 
    * User service - handles user authentication
  
![arch](images/architecture.png)
  
  
infra/k8s has the secrets and configuration for the application to work

How to configure:

in your local machine, provided that you have configured your account using aws-cli
```cat ~/.aws/credentials | head -n 3``` 
this will output the first 3 lines of the file, which is the default profile
```cat ~/.aws/credentials | head -n 3 | base64```
this will output the base64 encoded version of it.

similarly for POSTGRES secret environment variables, you will need to feed in encoded base64 into your secret yaml file
```echo -n $POSTGRES_PASSWORD | base64``` 

kubectl apply -f infra/k8s will create secret and configmap inside the cluster

```kubectl get secrets```
![secrets](images/kubectl-secrets.png)

```kubectl get configmaps```
![configmaps](images/kubectl-configmaps.png)

  
Docker Hub images:
![DockerHub](images/docker-hub.png)

AWS EKS cluster:
![EKS](images/eks-cluster.png)

  
```kubectl get deployments```
![deployments](images/kubectl-deployments.png)


```kubectl get services```
![services](images/kubectl-services.png)


```kubectl get hpa```
![hpa](images/kubectl-hpa.png)


Backend service functioning properly:
![feed-logs](images/kubectl-feed-logs.png)
![feed-ui](images/feed-api-aws-logs.png)

Running application:
![client](images/udagram-ui.png)

  
