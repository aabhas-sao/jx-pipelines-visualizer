# jx-pipelines-visualizer

![Version: 0.0.1](https://img.shields.io/badge/Version-0.0.1-informational?style=flat-square) ![AppVersion: latest](https://img.shields.io/badge/AppVersion-latest-informational?style=flat-square)

Web UI for Jenkins X, with a clear goal - visualize the pipelines - and their logs.

**Homepage:** <https://github.com/jenkins-x/jx-pipelines-visualizer>

## Source Code

* <https://github.com/jenkins-x/jx-pipelines-visualizer>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| config.archivedLogsURLTemplate | string | `nil` |  |
| config.archivedPipelineRunsURLTemplate | string | `nil` |  |
| config.archivedPipelinesURLTemplate | string | `nil` |  |
| config.logLevel | string | `"INFO"` |  |
| config.namespace | string | `"jx"` |  |
| config.pipelineTraceURLTemplate | string | `nil` |  |
| config.resyncInterval | string | `"60s"` |  |
| deployment.annotations | object | `{}` |  |
| deployment.labels | object | `{}` |  |
| deployment.replicas | int | `1` |  |
| deployment.revisionHistoryLimit | int | `2` |  |
| extraVolumeMounts | list | `[]` |  |
| extraVolumes | list | `[]` |  |
| fullnameOverride | string | `nil` |  |
| gitSecretName | string | `"tekton-git"` |  |
| image.pullPolicy | string | `nil` |  |
| image.repository | string | `"gcr.io/jenkinsxio/jx-pipelines-visualizer"` |  |
| image.tag | string | `nil` |  |
| ingress.annotations | object | `{}` |  |
| ingress.basicAuth.authData | string | `""` |  |
| ingress.basicAuth.enabled | bool | `false` |  |
| ingress.class | string | `"nginx"` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts | list | `[]` |  |
| ingress.labels | object | `{}` |  |
| ingress.tls.enabled | bool | `false` |  |
| ingress.tls.secrets | object | `{}` |  |
| istio.apiVersion | string | `"networking.istio.io/v1beta1"` |  |
| istio.enabled | bool | `false` |  |
| istio.gateway | string | `"jx-gateway"` |  |
| jx.releaseCRD | bool | `true` |  |
| nameOverride | string | `nil` |  |
| pod.activeDeadlineSeconds | string | `nil` |  |
| pod.affinity | object | `{}` |  |
| pod.annotations | object | `{}` |  |
| pod.enableServiceLinks | bool | `false` |  |
| pod.env | object | `{}` |  |
| pod.envFrom | list | `[]` |  |
| pod.hostAliases | list | `[]` |  |
| pod.labels | object | `{}` |  |
| pod.nodeSelector | object | `{}` |  |
| pod.resources.limits.cpu | string | `"1"` |  |
| pod.resources.limits.memory | string | `"512M"` |  |
| pod.resources.requests.cpu | string | `"0.2"` |  |
| pod.resources.requests.memory | string | `"128M"` |  |
| pod.schedulerName | string | `nil` |  |
| pod.securityContext.fsGroup | int | `1000` |  |
| pod.terminationGracePeriodSeconds | string | `nil` |  |
| pod.tolerations | list | `[]` |  |
| role.rules[0].apiGroups[0] | string | `"jenkins.io"` |  |
| role.rules[0].resources[0] | string | `"pipelineactivities"` |  |
| role.rules[0].resources[1] | string | `"pipelinestructures"` |  |
| role.rules[0].verbs[0] | string | `"list"` |  |
| role.rules[0].verbs[1] | string | `"watch"` |  |
| role.rules[0].verbs[2] | string | `"get"` |  |
| role.rules[1].apiGroups[0] | string | `"tekton.dev"` |  |
| role.rules[1].resources[0] | string | `"pipelineruns"` |  |
| role.rules[1].resources[1] | string | `"pipelines"` |  |
| role.rules[1].verbs[0] | string | `"list"` |  |
| role.rules[1].verbs[1] | string | `"watch"` |  |
| role.rules[1].verbs[2] | string | `"get"` |  |
| role.rules[2].apiGroups[0] | string | `""` |  |
| role.rules[2].resources[0] | string | `"pods"` |  |
| role.rules[2].verbs[0] | string | `"list"` |  |
| role.rules[2].verbs[1] | string | `"watch"` |  |
| role.rules[2].verbs[2] | string | `"get"` |  |
| role.rules[3].apiGroups[0] | string | `""` |  |
| role.rules[3].resources[0] | string | `"pods/log"` |  |
| role.rules[3].verbs[0] | string | `"get"` |  |
| service.annotations | object | `{}` |  |
| service.labels | object | `{}` |  |
| service.loadBalancerIP | string | `nil` |  |
| service.port | int | `80` |  |
| service.type | string | `nil` |  |
| serviceAccount.annotations | object | `{}` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.4.0](https://github.com/norwoodj/helm-docs/releases/v1.4.0)