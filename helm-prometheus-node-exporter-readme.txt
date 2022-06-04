run on helm prometheus node exporter with custom config
template: 

install: $ helm install [RELEASE_NAME] prometheus-community/prometheus-node-exporter
uninstall: $ helm uninstall [RELEASE_NAME]

install:
$ helm install pne prometheus-community/prometheus-node-exporter -f helm-prometheus-node-exporter.yaml

uninstall:
$ helm uninstall pne

link reference:
https://helm.sh/docs/intro/using_helm/#customizing-the-chart-before-installing
