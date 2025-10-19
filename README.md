# Keycloak Operator Helm Chart

Huge shout out to https://github.com/KyriosGN0 as this repo is based entirely on his work.

## Installation

```bash
helm repo add keycloak-operator https://binary64.github.io/keycloak/
helm --kube-context k3d-mycluster upgrade --install \
  keycloak-operator keycloak-operator/keycloak-operator \
  --namespace keycloak-operator \
  --create-namespace
```
