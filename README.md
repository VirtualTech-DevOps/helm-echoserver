# helm-echoserver

Setup Helm Repo

```
$ helm repo add helm-echoserver https://VirtualTech-DevOps.github.io/helm-echoserver
$ helm repo update
```

Install EchoServer

```
$ helm upgrade -i helm-echoserver helm-echoserver/helm-echoserver --namespace echoserver --create-namespace
```
