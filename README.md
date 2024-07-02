# promtail-k8s-helm
For install promtail replace <your-ip> in the file monitoring/values.yaml with your own ip and enter commands:
```
git clone https://github.com/bonanzza-web/promtail-k8s-helm.git
kubectl create ns monitoring
cd promtail-k8s-helm
helm install -n monitoring --values monitoring/values.yaml loki-stack grafana/loki-stack
```
