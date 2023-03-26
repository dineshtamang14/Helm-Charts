# Steps to create own helm chart

### To initialize the helm chart
```sh
helm create fleetman-helm-chart
```

### To Test own helm chart
```sh
helm template . --set webapp.numberOfWebAppReplicas=4
```

### To Run our own local charts
```sh
helm install my-fleetman-release . --set development=true
```

### To update running charts
```sh
helm upgrade my-fleetman-release . --set development=false
```

