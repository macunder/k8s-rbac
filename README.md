# k8s-rbac
 - create namespace (kubectl create namespace test)<br>
 - install helm chart (using lens UI to install one of chrt in the list into correct namespace)<br>
 - create service account (kubectl apply -f serviceAccount.yml)<br>
 - create user-secret (kubectl apply -f user-secret.yml)<br>
 - create role (kubectl apply -f role.yml)<br>
 - create role-binding (kubectl apply -f role-binding.yml)<br>
 - copy serviceAccount kubeconfig file into local kubecfg file (get it from lens UI)<br>
 - test access to list to the specifics namespace (kubectl get deployments -n test --kubeconfig=kubecfg)<br>
