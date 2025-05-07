# Listagem com comandos úteis da NASA

Exibe os detalhes de um certificado

`openssl x509 -in nome_certificado.crt -text -noout`

Lista e contabiliza o número de pods por node (Kubernetes)

`kubectl get pods -A -o jsonpath='{range .items[*]}{.spec.nodeName}{"\n"}{end}' | sort | uniq -c | sort -rn`

GCP - Lista as contas configuradas no Gcloud

`gcloud config configurations list`

GCP - Alterna entre as contas configuradas no Gcloud

`gcloud config configurations activate <name>`

GCP - Usar o impersonate como default

`gcloud config set auth/impersonate_service_account SERVICE_ACCT_EMAIL`
