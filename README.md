# helm-echoserver

echoserverのHelmチャートです。主にKubernetesやArgo CDの動作確認用。

```
$ helm repo add helm-echoserver https://VirtualTech-DevOps.github.io/helm-echoserver
$ helm repo update
```

```
$ domain=test.devops.virtualtech.jp

$ helm upgrade -i helm-echoserver \
    helm-echoserver/helm-echoserver \
    --namespace echoserver \
    --create-namespace \
    --set "ingress.hosts[0].host=$domain" \
    --set 'ingress.hosts[0].paths[0].path=/' \
    --set 'ingress.hosts[0].paths[0].pathType=Prefix' \
    --set "ingress.annotations.external-dns\.alpha\.kubernetes\.io/hostname=$domain"
```

| Chart Revision | App Version |
|----------------|-------------|
| 0.7.0          | 1.10         |
| 0.6.0          | 1.9         |
| 0.5.0          | 1.8         |
| 0.4.0          | 1.7         |
| 0.3.0          | 1.6         |
| 0.2.0          | 1.5         |
| 0.1.0          | 1.4         |
