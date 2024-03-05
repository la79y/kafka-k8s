```shell
kubectl --kubeconfig=/Users/bander/Downloads/k8s-1-29-1-do-0-fra1-1709583608918-kubeconfig.yaml apply -f confluent-local/00-namespace.yaml 
kubectl --kubeconfig=/Users/bander/Downloads/k8s-1-29-1-do-0-fra1-1709583608918-kubeconfig.yaml apply -f confluent-local/01-kafka-local.yaml

```


## Setup k8s dashboard
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.2.0/aio/deploy/recommended.yaml
kubectl proxy
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/
