## ☸️ kubernetes prometheus Setup

mv promethus directory

kubectl create namespace monitoring  
kubectl create -f clusterRole.yaml  
kubectl create -f config-map.yaml  
kubectl create  -f prometheus-deployment.yaml   
kubectl get deployments --namespace=monitoring   
kubectl get pods --namespace=monitoring   
kubectl port-forward prometheus-monitoring-3331088907-hm5n1 8080:9090 -n monitoring  
kubectl create -f prometheus-service.yaml --namespace=monitoring  
 
