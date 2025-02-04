# peregrine

![Version: 0.1.1](https://img.shields.io/badge/Version-0.1.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 2022.10](https://img.shields.io/badge/AppVersion-2022.10-informational?style=flat-square)

A Helm chart for gen3 Peregrine service

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| file://../common | common | 0.1.1 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| arboristUrl | string | `nil` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| env | string | `nil` |  |
| fullnameOverride | string | `""` |  |
| global.ddEnabled | bool | `false` |  |
| global.dev | bool | `true` |  |
| global.dictionaryUrl | string | `"https://s3.amazonaws.com/dictionary-artifacts/datadictionary/develop/schema.json"` |  |
| global.dispatcherJobNum | int | `10` |  |
| global.environment | string | `"default"` |  |
| global.hostname | string | `"localhost"` |  |
| global.kubeBucket | string | `"kube-gen3"` |  |
| global.logsBucket | string | `"logs-gen3"` |  |
| global.netPolicy | bool | `true` |  |
| global.portalApp | string | `"gitops"` |  |
| global.postgres.dbCreate | bool | `true` |  |
| global.postgres.master.host | string | `nil` |  |
| global.postgres.master.password | string | `nil` |  |
| global.postgres.master.port | string | `"5432"` |  |
| global.postgres.master.username | string | `"postgres"` |  |
| global.publicDataSets | bool | `true` |  |
| global.revproxyArn | string | `"arn:aws:acm:us-east-1:123456:certificate"` |  |
| global.syncFromDbgap | bool | `false` |  |
| global.tierAccessLevel | string | `"libre"` |  |
| global.userYamlS3Path | string | `"s3://cdis-gen3-users/test/user.yaml"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"quay.io/cdis/peregrine"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| postgres.database | string | `"peregrine"` |  |
| postgres.dbCreate | string | `nil` |  |
| postgres.host | string | `nil` |  |
| postgres.password | string | `nil` |  |
| postgres.port | string | `"5432"` |  |
| postgres.username | string | `"peregrine"` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | float | `1` |  |
| resources.limits.memory | string | `"512Mi"` |  |
| resources.requests.cpu | float | `0.1` |  |
| resources.requests.memory | string | `"12Mi"` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| volumeMounts | string | `nil` |  |
| volumes[0].emptyDir | object | `{}` |  |
| volumes[0].name | string | `"shared-data"` |  |
| volumes[1].name | string | `"config-volume"` |  |
| volumes[1].secret.secretName | string | `"peregrine-secret"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
