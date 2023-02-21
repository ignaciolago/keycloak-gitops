# keycloak-gitops
## First we install the argocd operator:
```
oc apply -k bootstrap/argocd
```
##
```
oc apply -k bootstrap/deploy/00_rhsso-operator
oc apply -k bootstrap/deploy/01_rhsso-dev
```
# Install Database for test
# add values to secret for DB
```
oc apply -k bootstrap/deploy/02_rhsso-test
```
# Install Database for prod
# add values to secret for DB
```
oc apply -k bootstrap/deploy/03_rhsso-prod
```
