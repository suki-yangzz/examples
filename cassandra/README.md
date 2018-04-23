# Example: Cassandra with StatefulSets on Kubernetes


This directory contains the source code and Kubernetes manifests for Cassandra
deployment with StatefulSets tutorial.

Follow this tutorial at https://kubernetes.io/docs/tutorials/stateful-application/cassandra/.


kubectl create -f cassandra-service.yaml
kubectl get services
kubectl create -f cassandra-statefulset.yaml
kubectl describe pod cassandra-0

kubectl delete statefulset -l app=cassandra
kubectl delete pvc -l app=cassandra
kubectl delete storageclass fast
