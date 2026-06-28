# apisix-ui-charts

Helm charts for [apisix-ui](https://github.com/Kamoliddinxoji/apisix-ui).

## Add repo

```bash
helm repo add apisix-ui https://kamoliddinxoji.github.io/apisix-ui-charts
helm repo update
```

## Install

```bash
helm install apisix-ui apisix-ui/apisix-ui \
  --set config.databaseUrl="postgres://user:pass@postgres:5432/apisix_ui?sslmode=disable" \
  --set config.jwtSecret="your-secret-32chars" \
  --set config.adminPassword="your-admin-password"
```
