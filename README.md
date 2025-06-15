# kube-demo-argo-cd

handson:

- Create a git repo // sample repo: https://github.com/aryanm12/demo-argocd

- Add Argo Application Configuration like: application.yaml

- Place K8S manifest files in it like: k8s-manifest/sample.yaml

- Apply the Argo Application file:

    - kubectl apply -f application.yaml

- Check if sync is working:

    - kubectl get application -n argocd // Status should update to Healthy

- Change replica settings at the runtime // Observe that there is no change in the cluster

- Change the replicas in the git repo // Observe auto update