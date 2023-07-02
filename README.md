# jupyterhub

to install:
helm upgrade --cleanup-on-fail --install my-jupyter jupyterhub/jupyterhub --namespace jhub2 --create-namespace --values values.yaml

dependecies:
values.yaml -> for custom install
storage-class-immediate.yaml -> for auto create pvc


other commands:
kubectl cluster-info
kubectl get all --all-namespaces


chmod o-r ~/.kube/config
chmod g-r ~/.kube/config

helm repo add jupyterhub https://jupyterhub.github.io/helm-chart/
helm repo add jupyterhub https://github.com/irwannafly13/jupyterhub/blob/main/jupyterhub-2.0.tgz


helm repo update
helm version
helm show values jupyterhub/jupyterhub > values.yaml

helm init --upgrade --force-upgrade

helm repo list 

helm upgrade --cleanup-on-fail --install jupyter jupyterhub/jupyterhub --namespace jhub --create-namespace --values values.yaml

cd to custom chart, then helm install . --generate name

kubectl get pod --namespace test-irwan

kubectl get services -n jhub

kubectl --namespace irwan-dev get service proxy-public

kubectl config set-context $(kubectl config current-context) --namespace test-irwan

helm upgrade chart-1684117419 /root/.kube/jupyterhub
