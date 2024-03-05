# Kafka em K8s

Recursos para um [tutorial](https://rafaelnatali.wixsite.com/rmn-technology/pt/post/executando-o-kafka-no-kubernetes-com-o-modo-kraft) que aborda a execução do [Kafka v3.5.x](https://docs.confluent.io/platform/current/installation/versions-interoperability.html) usando o protocolo [Apache Kafka Raft (KRaft)](https://developer.confluent.io/learn/kraft/) em um cluster Kubernetes baseado no Minikube.

- [Quickstart: confluent-local](./confluent-local/README-pt.md)
- [Kafka com SSL](./ssl/README-pt.md)
- [Kafka com SASL Authentication](./sasl/README-pt.md)

## Contribuindo

Fique a vontade para contribuir abrindo _issues_ ou _pull requests_.

## Licença

Este projeto está licensiado usando a MIT License - vejo o arquivo [LICENSE](../LICENSE) para detalhes.

## Setup k8s dashboard
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.2.0/aio/deploy/recommended.yaml
kubectl proxy
http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/
