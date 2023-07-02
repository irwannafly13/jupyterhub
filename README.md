# jupyterhub


to install:
helm upgrade --cleanup-on-fail --install my-jupyter jupyterhub/jupyterhub --namespace jhub2 --create-namespace --values values.yaml

dependecies:
values.yaml -> for custom install
storage-class-immediate.yaml -> for auto create pvc
