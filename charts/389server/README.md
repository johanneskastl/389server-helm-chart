# 389server

![Version: 0.2.1](https://img.shields.io/badge/Version-0.2.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2.0](https://img.shields.io/badge/AppVersion-2.0-informational?style=flat-square)

Helm chart for the 389ds server

## TL;DR
```console
$ helm repo add johanneskastl-389server https://johanneskastl.github.io/389server-helm-chart/
$ helm repo update
$ helm install 389server johanneskastl-389server/389server
```

## Installing the Chart
To install the chart with the release name `389server`:
```console
helm install 389server johanneskastl-389server/389server
```

## Uninstalling the Chart
To uninstall the `389server` deployment:
```console
helm uninstall 389server
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install 389server \
  --namespace 389server \
    johanneskastl-389server/389server
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install 389server johanneskastl-389server/389server -f values.yaml
```

