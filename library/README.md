# common

![Version: 0.0.1](https://img.shields.io/badge/Version-0.0.1-informational?style=flat-square) ![Type: library](https://img.shields.io/badge/Type-library-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

Gitlab Helm Chart Library

**Homepage:** <https://github.com/lpmatos/helm-library>

## Maintainers

| Name    | Email                   | Url |
|---------|-------------------------|-----|
| CI Monk | lpsm-dev@protonmail.com |     |

## Source Code

* <https://github.com/lpmatos/helm-library>

## Requirements

Kubernetes: `>=1.16.0-0`

## Values

| Key                                                           | Type   | Default               | Description |
|---------------------------------------------------------------|--------|-----------------------|-------------|
| application.owner                                             | string | `"team-xpto"`         |             |
| application.product                                           | string | `"xpto"`              |             |
| applications[0].affinity                                      | object | `{}`                  |             |
| applications[0].autoscaling.enabled                           | bool   | `true`                |             |
| applications[0].autoscaling.maxReplicas                       | int    | `3`                   |             |
| applications[0].autoscaling.minReplicas                       | int    | `1`                   |             |
| applications[0].autoscaling.targetCPUUtilizationPercentage    | int    | `80`                  |             |
| applications[0].autoscaling.targetMemoryUtilizationPercentage | int    | `80`                  |             |
| applications[0].containerSecurityContext                      | object | `{}`                  |             |
| applications[0].deploymentAnnotations                         | object | `{}`                  |             |
| applications[0].extraEnv                                      | object | `{}`                  |             |
| applications[0].extraEnvSecret                                | object | `{}`                  |             |
| applications[0].gitlab.project                                | string | `"api/auth"`          |             |
| applications[0].gitlab.tag                                    | string | `"1.0.0-rc.1"`        |             |
| applications[0].livenessProbe.enabled                         | bool   | `true`                |             |
| applications[0].name                                          | string | `"auth"`              |             |
| applications[0].nodeSelector                                  | object | `{}`                  |             |
| applications[0].pdb.enabled                                   | bool   | `true`                |             |
| applications[0].podAnnotations                                | object | `{}`                  |             |
| applications[0].podSecurityContext                            | object | `{}`                  |             |
| applications[0].priorityClassName                             | string | `""`                  |             |
| applications[0].readinessProbe.enabled                        | bool   | `true`                |             |
| applications[0].replicaCount                                  | int    | `1`                   |             |
| applications[0].resources.limits.cpu                          | string | `"100m"`              |             |
| applications[0].resources.limits.memory                       | string | `"252Mi"`             |             |
| applications[0].resources.requests.cpu                        | string | `"100m"`              |             |
| applications[0].resources.requests.memory                     | string | `"252Mi"`             |             |
| applications[0].rollingUpdate.surge                           | string | `nil`                 |             |
| applications[0].rollingUpdate.unavailable                     | string | `nil`                 |             |
| applications[0].service.externalPort                          | int    | `80`                  |             |
| applications[0].service.internalPort                          | int    | `3000`                |             |
| applications[0].strategy                                      | string | `nil`                 |             |
| applications[0].tolerations                                   | list   | `[]`                  |             |
| domain                                                        | string | `"xpto.com.br"`       |             |
| environment                                                   | string | `"develop"`           |             |
| gitlab.branch                                                 | string | `"sandbox"`           |             |
| gitlab.group                                                  | string | `"xpto/beta"`         |             |
| global.sharedEnv                                              | object | `{}`                  |             |
| global.sharedEnvSecret                                        | object | `{}`                  |             |
| image.pullPolicy                                              | string | `"Always"`            |             |
| image.registry                                                | string | `"registry.xpto.com"` |             |
| serviceAccount.create                                         | bool   | `true`                |             |
| serviceAccount.imagePullSecrets[0].name                       | string | `"image-pull-secret"` |             |
| serviceAccount.name                                           | string | `"xpto-registry"`     |             |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
