# before you run kubeconfig you should have service account created
$ kubectl create serviceaccount k8s-dash-sa
# otherwise ca=.. token=.. & namespace=.. will fail if the secret is not present in default namespace

# get the cluster url, cluster certificate and account token from cluster file, stored under: ~/.kube/config
$ kubectl --context=k8s get pods -n test-namespace

# add below flag if you are using self signed certificate
$  --insecure-skip-tls-verify




