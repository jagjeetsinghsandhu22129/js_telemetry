# INFO8995-telemetry
run open telemetry demo in codespace

TLDR;

```
ansible-playbook toaster.yml
kubectl port-forward svc/my-otel-demo-frontendproxy 8080:8080
```

If you need to delete a cluster and start over you can run:

```
k3d cluster delete local-k8s
rm -rf ~/.kube
```

Then you can take it from the top.

Note: This also works (faster) in vscode local with docker desktop installed. 

1. From the command palette `Dev Containers: Clone Repository in Container Volume`. 

2. Choose this repository `https://github.com/rhildred/INFO8985-telemetry.git`. 

3. Follow the steps from TLDR;

The deliverable for the lab is to create a deployment diagram using [https://www.umletino.com/umletino.html](https://www.umletino.com/umletino.html). This can be done by dragging and dropping pods you see with the `kubectl get pods` command. A starting place would be something like this:

![deployment diagram](READMEImages/deployment.png)

Hopefully this is a gentle introduction to ansible and kubernetes.