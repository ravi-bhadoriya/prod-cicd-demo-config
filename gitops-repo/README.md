# prod-cicd-demo-config

This is the GitOps repository.

It represents desired production state.

ArgoCD watches this repository and reconciles the Kubernetes cluster to match these manifests.

Before first sync, replace `REPLACE_ECR_REPOSITORY` in `apps/prod-cicd-demo/deployment.yaml` with the ECR repository URL from Terraform output.
