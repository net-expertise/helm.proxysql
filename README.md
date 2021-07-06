# Proxysql Helm Chart

Proxysql cluster to install on Kubernetes

Inspired by https://github.com/ProxySQL/kubernetes

More details at https://www.netexpertise.eu/en/database/mysql/proxysql-helm-chart-load-rules-from-sql-query-set.html

## Chart Details

This chart will do the following:

* ProxySQL exposed on an external LoadBalancer
* Admin port 6032 on LoadBalancer with annotations
* Stat web server reachable through ingress
* SQL config injected from Values file

## Installing the Chart

To install the chart with the release name `my-release`:

```bash
$ helm install my-release -f example.yaml ./proxysql
```

