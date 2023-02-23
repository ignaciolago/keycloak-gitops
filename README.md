# keycloak-gitops
## First we install the argocd operator:
```
oc apply -k bootstrap/argocd
```
## Second we install the Red Hat Single Sign Dev Environment using Red Hat Single Sign On Operator
```
oc apply -k bootstrap/deploy/application/01_rhsso-dev
```

# Install Database for prod
## add values to secret for DB
```
oc apply -k bootstrap/deploy/application/03_rhsso-prod
```
