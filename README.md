# To run containers:

- Install Helm
  - https://helm.sh
  - or `brew install helm`
- Install `nginx-ingress` via Helm
  - `helm repo add nginx-stable https://helm.nginx.com/stable`
  - `helm repo update`
- Verify nginx is running
  - `kubectl get services nginx-ingress-controller`
- Build docker image on local
  - `docker build -t k8s-fast-api .`
- Run all yaml files
  - `cd kubernetes`
  - `kubectl apply -f .`
