- kubeadm init --config kubeadm-config.yaml --ignore-preflight-errors=NumCPU  --ignore-preflight-errors=Mem
- kubectl get pod -n kube-system
- kubectl get node

- To connect nodes to master: kubeadm join 202.182.109.171:6443 --token 8utmgl.fec9shz8dcx8jmg5 --discovery-token-ca-cert-hash sha256:b5e9c3c0849b8ce787f08f16031bc2ff52a11488ad0415e82441e63e263f333a
- kubectl create deployment hello-minikube --image=k8s.gcr.io/echoserver:1.4
- kubectl expose deployment hello-minikube --type=NodePort --port=8080

- kubectl create deployment nginx --image=nginx
- kubectl expose deployment nginx --type=NodePort --port=80

- kubeadm init --ignore-preflight-errors=all
