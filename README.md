# Deploy the "Job" Helm Chart 
```
cd ipto-job-helm
helm install -f values.yaml .
```

# Deploy the "CronJob" Helm Chart 
```
cd ipto-cron-helm
helm install -f values.yaml .
```

# Deploy the "CronJob" Helm Chart using ArgoCD
```
kubectl apply -f argo-app.yaml
```
Caution! When the app is deployed that way, any commit to this git repo will lead to a new deployment to the cluster.
