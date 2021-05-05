# How to deploy dotnet 5 app kubernetes

## Create dockerfile

    docker build -t hello-k8s-image:v1 .

## Check docker image

    docker images

## Apply K8S deployment

    kubectl apply -f .\deployments.yaml

## Check deployment

    kubectl get deployment

## Check Pod

    kubectl get pod

## Get Container log

    kubectl logs <podName> (Example : hello-k8s-deployment-7bf75dd54c-wxbgl)

## Apply K8S service

    kubectl apply -f .\service.yaml

## Check service

    kubectl get service

## Check application endpoint

    http://localhost:8080/WeatherForecast

