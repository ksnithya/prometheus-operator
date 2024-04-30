# prometheus installation
First we install Prometheus using helm.
Add Prometheus helm chart repository
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
------------------------------------
Update the helm chart repository
helm repo update
helm repo list
-----------------------------------------
Create prometheus namespace
kubectl create namespace prometheus
-----------------------------------------
Install Prometheus
helm install prometheus prometheus-community/kube-prometheus-stack -n Prometheus
----------------------------------------------
