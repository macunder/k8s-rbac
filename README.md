# k8s-rbac
create namespace (kubectl create namespace test)
install helm chart (using lens UI to install one of chrt in the list into correct namespace)
create service account (kubectl apply -f serviceAccount.yml)
create user-secret (kubectl apply -f user-secret.yml)
create role (kubectl apply -f role.yml)
create role-binding (kubectl apply -f role-binding.yml)
copy serviceAccount kubeconfig file into local kubecfg file (get it from lens UI)()
test access to list to the specifics namespace (kubectl get deployments -n test --kubeconfig=kubecfg)
