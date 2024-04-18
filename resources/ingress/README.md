kubectl create ns ingress-nginx

git clone https://github.com/techiescamp/nginx-ingress-controller.git

cd nginx-ingress-controller/manifests/

kubectl apply -f .

Check the pods and svc in the ingress-nginx namespace

Check Loadbalancer svc created
