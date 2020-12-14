# Grouparoo Helm Chart

## Running

Ensure that you have both docker and Kubernetes running locally. If you are using Docker Desktop, you can do this from the Prefrences pane:

> TODO: IMAGE

You can run the generated Helm Chart locally with the helm command - https://helm.sh/docs/intro/install/

Assuming you have Docker and Kubernetes running locally: `

```bash
cd helm
helm install grouparoo-app-example .
```

From there you can use the normal kubectl commands to check on the deployments:

```bash
# see that the chart deployed a db, redis, grouparoo-web, and grouparoo-worker deployment
kubectl get deployments

## kubectl cheatsheet -https://kubernetes.io/docs/reference/kubectl/cheatsheet/
```

And you can uninstall the chart with

```bash
helm uninstall grouparoo-app-example
```

## Notes

If you have a 'stale' PVC (persistent value column) in your Kubernetes cluster, you may end up with an old value for the Postgres password. https://github.com/helm/charts/issues/10918#issuecomment-458044163. Totally blowing away all the data in your cluster is one way to fix it...
