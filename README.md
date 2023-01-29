# K8S Postgres Nest App


### Comandos utiles

```bash
minikube pause
minikube unpause
minikube stop
minikube delete --all
minikube service <nombre del deployment>

kubectl get pod
kubectl rollout restart deployment

kubectl apply -f postgres-config.yml
kubectl apply -f postgres-secrets.yml
kubectl apply -f postgres.yml
kubectl get all

kubectl logs <nombre del deployment>
kubectl get events
minikube ip 

minikube ssh -- docker images
```

---

##### Made with ❤️ by Leandro Arturi
