# ghostfolio-k8s

[Ghostfolio](https://github.com/ghostfolio/ghostfolio/) is an open source wealth management software built with web technology. This project enables potential users to deploy the entire app on Kubernetes with [Helm](https://helm.sh/) 

## Why
With rising popularity of Kubernetes, this project will provide an alternative way to deploy the application on Kubernetes using Helm

## Dependencies

* `Kubernetes`
* `Helm`

## Deployment Guide 

Create new namespace
```
kubectl create namespace ghostfolio
```

Deploy Ghostfolio using Helm

```
helm install ghostfolio . --namespace ghostfolio
```

Check if services are ready

```
kubectl get svc --namespace ghostfolio
```

Go to your browser and enter the following URL:

```
localhost:32333
```

## Roadmap
- [x] Create Manifests file
- [x] Helm Integration Guide
- [ ] Implement Secrets 

## Contributing

Pull requests are welcome. The premise of this script is to provide basic information, so keep that in mind. If you have a major feature idea, let's discuss it through the issues page first.

Of course, feel free to fork and create a more interactive experience!

## License

GPL v3
