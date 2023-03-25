### To add a helm repo
```sh
helm repo add my-repo https://charts.bitnami.com/bitnami
```

### To install from added repo
```sh
helm install my-release my-repo/mysql
```

### To list helm charts
```sh
helm list
```

### To uninstall charts
```sh
helm uninstall mysql
```

### To list all registered repo
```sh
helm repo list
```

### To update helm repo
```sh
helm repo update
```
### To edit running service
```sh
kubectl edit svc monitoring-grafana
```

### To print the values of repo
```sh
helm show values prom-repo/kube-prometheus-stack
```

### To update the running helm chart data
```sh
helm upgrade monitoring prom-repo/kube-prometheus-stack --set grafana.adminPassword=admin
```

#### To update running helm chart with values
```sh
helm upgrade monitoring prom-repo/kube-prometheus-stack --values=values.yml
```

### To download charts from artifact hub
```sh
helm pull prom-repo/kube-prometheus-stack --untar=true
```

### To run downloaded charts
```sh
helm install monitoring ./kube-prometheus-stack
```

### To upgrade cluster with override values
```sh
helm upgrade monitoring --values=myvalues.yaml .
```

### To Generate kubernetes yml from charts
```sh
helm template monitoring ./kube-prometheus-stack --values=./kube-prometheus-stack/myvalues.yml > monitoring-stack.yaml
```

### To create a own helm chart
```sh
helm create fleetman-helm-chart
```

