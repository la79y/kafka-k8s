
## Setup k8s dashboard
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.2.0/aio/deploy/recommended.yaml
kubectl proxy
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/


```shell
kubectl apply -f confluent-local/00-namespace.yaml 
kubectl apply -f confluent-local/01-kafka-local.yaml
```

