# helm-echoserver

echoserverのHelmチャートです。主にKubernetesやArgo CDの動作確認用。

```
$ helm repo add helm-echoserver https://VirtualTech-DevOps.github.io/helm-echoserver
$ helm repo update
$ helm upgrade -i helm-echoserver helm-echoserver/helm-echoserver --namespace echoserver --create-namespace 
```

| Chart Revision | App Version |
|----------------|-------------|
| 0.5.0          | 1.8         |
| 0.4.0          | 1.7         |
| 0.3.0          | 1.6         |
| 0.2.0          | 1.5         |
| 0.1.0          | 1.4         |
