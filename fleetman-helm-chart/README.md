# Steps to create own helm chart

### To initialize the helm chart
```sh
helm create fleetman-helm-chart
```

### To Test own helm chart
```sh
helm template . --set webapp.numberOfWebAppReplicas=4
```


