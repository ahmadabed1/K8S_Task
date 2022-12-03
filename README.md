# **kubernetes Task**

## About
This repository represent kubernetes project, it has developed using minikube. The mean idea to publish 3 website with 3 different paths, for that i have used ingress technology to manage network connection. For each website i have used yaml file , which has:

- Deployment: build the pod under supervison(to avoid failure), every pod . . . - know the docker image to run over.
- Service: enables network access from either within the cluster or between external. processes and the service

## This images in dockerhub:
<img width="769" alt="צילום מסך 2022-11-30 210626" src="https://user-images.githubusercontent.com/73169815/205429832-b81148ff-14cb-40c7-ae9a-ddfa3ae5f905.png">

<img width="778" alt="צילום מסך 2022-11-30 210454" src="https://user-images.githubusercontent.com/73169815/205429838-a2e59f66-5115-4cb8-a770-7d2db32ba329.png">


## Run
git clone this project 

1. Start minikube:
```bash
Start minikube
```


2. Enagle ingress plugin:
```bash
  minikube addons enable ingress
```
3.Insert all deployments:
```bash
 kubectl apply -f .
```
<img width="404" alt="צילום מסך 2022-11-30 224904" src="https://user-images.githubusercontent.com/73169815/205429882-69aeca34-0955-43ee-be20-cdd6eaa78163.png">

4.Pod status:
```bash
kubctl get po
```
```bash
kubctl get deployment
```
<img width="421" alt="צילום מסך 2022-11-30 224415" src="https://user-images.githubusercontent.com/73169815/205429954-f33c692a-0bf9-4ea3-829f-99b6e1de6f6b.png">

5.Run locally:
open your browser:
. http://localhost/bitcoin

. http://localhost/ynet

6. To stop minikube run the following command:
```bash
minikube stop
```




