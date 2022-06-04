kubernetes metrics-server 
url: https://github.com/kubernetes-sigs/metrics-server
install: kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml

note: 
- namespace bisa menggunakan namespace "kube-system" atau "default"
- metrics-server tidak bisa langsung di scrape oleh prometheus, harus menggunakan exporter

alternative installation: 
https://bitnami.com/stack/metrics-server/helm
https://cloud.digitalocean.com/marketplace/5d83d4f9cc248c518b58a38c?i=561432

https://github.com/grupozap/metrics-server-exporter
install: kubectl apply -f deploy/

ganti service metrics-server-exporter dengan service NodePort atau LoadBalancer agar bisa discrape oleh prometheus


alternative: https://github.com/ghouscht/metrics-server-exporter
