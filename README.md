# udagram-microservice

A simple image sharing AWS cloud application.


1. Frontend - Angular web application built with Ionic Framework
2. Backend RESTful API - Node-Express application
    a. Feed Service - handles image feeds 
    b. User service - handles user authentication
  
  ![Screenshot 2020-12-07 at 17 03 41](https://user-images.githubusercontent.com/17296281/101410531-66dfd000-38d7-11eb-817f-49c17c5c825a.png)
  
  
infra/k8s has the secrets and configuration for the application to work
How to configure:

# in your local machine, provided that you have configured your account using aws-cli
cat ~/.aws/credentials | head -n 3 
# this will output the first 3 lines of the file, which is the default profile
cat ~/.aws/credentials | head -n 3 | base64
# this will output the base64 encoded version of it.



similarly for POSTGRES secret environment variables, you will need to feed in encoded base64 into secret.yaml file
echo -n $POSTGRES_PASSWORD | base64 

kubectl apply -f infra/k8s will crete secret and configmap inside the cluster

  
Docker Hub images:
  
<img width="772" alt="Screenshot 2020-12-07 at 21 31 38" src="https://user-images.githubusercontent.com/17296281/101410687-9db5e600-38d7-11eb-805a-3fdcbf104011.png">

AWS EKS cluster:
<img width="1003" alt="Screenshot 2020-12-07 at 21 30 51" src="https://user-images.githubusercontent.com/17296281/101410627-8a0a7f80-38d7-11eb-8c3b-01c26a3c95e8.png">
  

'kubectl get deployments'



'kubectl get services'
<img width="1169" alt="Screenshot 2020-12-07 at 22 10 55" src="https://user-images.githubusercontent.com/17296281/101411589-25502480-38d9-11eb-905c-04bd1448914a.png">



'kubectl get hpa'







Backend service running:
<img width="940" alt="Screenshot 2020-12-07 at 14 28 02" src="https://user-images.githubusercontent.com/17296281/101410807-cccc5780-38d7-11eb-9976-84ba9efae246.png">

![Screenshot 2020-12-07 at 14 26 21](https://user-images.githubusercontent.com/17296281/101411042-3187b200-38d8-11eb-801c-7ba38bbfde26.png)


Running application:

  
