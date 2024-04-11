Step1: kubectl create ns ingress-nginx
Step2:Clone the repo (cmd: git clone https://github.com/techiescamp/nginx-ingress-controller.git)
Step3: cd nginx-ingress-controller/manifests/
Step4: kubectl apply -f .
Step5: Check the pods and svc in the ingress-nginx namespace
Step6: Check Loadbalancer svc created
