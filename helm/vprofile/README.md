# VProfile Helm Chart

Install the chart with:

```sh
helm install vprofile ./helm/vprofile
```

Configure workloads and credentials in `values.yaml`. Override `secrets.dbPassword` and `secrets.rabbitmqPassword` for non-local environments. To use a private image registry, set `dockerregistry.enabled` to `true` and provide its server, username, password, and email; the generated Secret is attached to workload pods as an image pull secret.
