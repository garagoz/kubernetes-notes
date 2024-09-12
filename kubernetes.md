# Kubernetes commands both imperative and declarative way

## Pods

#### creating a pod imperative way
k run nginx --image=nginx

#### creating with maifest file -> nginx.yaml
apiVersion: v1
kind: Pod
metadata:
  name: mypod
spec:
  containers:
    - name: nginx
      image: nginx

