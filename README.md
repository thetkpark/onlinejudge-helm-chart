# Onlinejudge Helm Chart
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/onlinejudge)](https://artifacthub.io/packages/search?repo=onlinejudge) ![](https://img.shields.io/github/v/tag/thetkpark/onlinejudge-helm-chart)

> A Helm Chart for [QingdaoU/OnlineJudge](https://github.com/QingdaoU/OnlineJudge)

## Installing the Chart
> Install the Chart with the release name of `my-onlinejudge`

```bash
$ helm repo add onlinejudge https://thetkpark.github.io/onlinejudge-helm-chart
$ helm install my-onlinejudge onlinejudge/onlinejudge
```

## Uninstalling the Chart

> Uninstall the Chart with the release name of `my-onlinejudge`

```bash
$ helm uninstall my-onlinejudge
```

## Paramaters

| Name               | Description                                               | Value           |
| ------------------ | --------------------------------------------------------- | --------------- |
| judge_server_token | The token that used to authorize judge-server and backend | changeThisToken |
| disk_size          | The disk size that will be provision by PVC               | 2Gi             |
| storage_class      | Name of the storage class that PV will be created on      | default         |
| postgres.db        | Database name that will be used to store data             | onlinejudge     |
| postgres.username  | Username of the Postgres database user                    | onlinejudge     |
| postgres.password  | Password of the Postgres database user                    | onlinejudge     |

