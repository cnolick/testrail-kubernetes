# Deploy Testrail to kubernetes.

Deployment [testrail](https://www.gurock.com/testrail/) to kubernetes across [kustomize](https://github.com/kubernetes-sigs/kustomize)


## Usage

just change config mysql in `mysql/config/mysql.env` and `Ingress.yaml`. 

If you wanna use ldap auth change config `testrail/config/auth.php`

and build:

```bash
kustomize build
```

or apply in your cluster

```bash
kustomize build |kubectl apply -f - 
```


## TODO

Helm