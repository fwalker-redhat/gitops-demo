# Very Basic GitOps Demo

## Instructions

1. Clone the repository
2. In order to bootstrap the correct ArgoCD Application Projects (`appproject`) resources need to be created first. This can be achieved by running the following command: `oc project openshift-gitops; oc apply -f argocds/kustomize/overlays/cluster/projects`
3. Apply the bootstrap Argo CD Application. This can be achieved by running the following command: `oc project openshift-gitops; oc apply -f bootstrap/bootstrap-app-of-apps.yaml`