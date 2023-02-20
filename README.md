# keycloak-gitops
oc apply -k bootstrap/argocd
oc apply -k bootstrap/deploy/00_rhsso-operator
oc apply -k bootstrap/deploy/01_rhsso-dev
oc apply -k bootstrap/deploy/02_rhsso-test
oc apply -k bootstrap/deploy/03_rhsso-prod 