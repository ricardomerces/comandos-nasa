# Listagem com comandos úteis da NASA

Exibe os detalhes de um certificado

`openssl x509 -in nome_certificado.crt -text -noout`

Lista as contas configuradas no Gcloud

`gcloud config configurations list`

Alterna entre as contas configuradas no Gcloud

`gcloud config configurations activate <name>`

Lista e contabiliza o número de pods por node (Kubernetes)

`kubectl get pods -A -o jsonpath='{range .items[*]}{.spec.nodeName}{"\n"}{end}' | sort | uniq -c | sort -rn`
