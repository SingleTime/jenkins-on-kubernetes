## Get Start



## build jenkins master

```shell
kubectl create -f jenkins.yaml -n kube-ops
```



## build setting.xml

```shell
kubectl create configmap maven-settings --from-file=settings.xml -n kube-ops
```



## build jenkins agnet

```shell
kubectl create -f jenkins-agent.yaml -n kube-ops
```

 备注：jenkins-agent:1.0。镜像的构建脚本 jenkins-agent/Dockerfile

