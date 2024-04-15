https://helm.sh/docs/intro/install/


helm create jenkins


helm template jenkins ./jenkins



helm install jenkins ./jenkins --dry-run




helm install jenkins ./jenkins 

or

helm install --create-namespace jenkins ./jenkins --namespace jenkins





helm uninstall jenkins


helm update jenkins ./jenkins --set replicas=4
