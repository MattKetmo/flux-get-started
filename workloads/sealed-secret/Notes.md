https://github.com/bitnami-labs/sealed-secrets#installation

kubectl -n kube-system port-forward deployment/sealed-secrets-controller 8080:8080

curl localhost:8080/v1/cert.pem > cert.pem


See: https://github.com/bitnami-labs/sealed-secrets#usage
use version v0.5.1 of kubeseal cli since later version are broken
See: https://github.com/bitnami-labs/sealed-secrets/issues/86

