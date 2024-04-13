# Install

[Setup gitlab helm repo](https://docs.gitlab.com/runner/install/kubernetes.html#installing-gitlab-runner-using-the-helm-chart)

Create a namespace for your runners:
```bash
kubectl apply -f runner-namespace.yaml
```
(version v1.29.0 at the time)

Install the runner:
```bash
helm install --namespace runners runner-name -f values.yaml gitlab/gitlab-runner
```
(version v3.13.1 at the time)