# K8S Postgres Nest App

### Instalar minikube (Mac)

```bash
brew install minikube
minikube version
minikube start
```

### Levantar cluster

#### Postgres

```bash
kubectl apply -f postgres-config.yml
kubectl apply -f postgres-secrets.yml
kubectl apply -f postgres.yml
```

#### PgAdmin

```bash
kubectl apply -f pgadmin-secrets.yml
kubectl apply -f pgadmin.yml
```

#### Teslo App (Nest.js)

```bash
kubectl apply -f backend-secrets.yml
kubectl apply -f backend.yml
```

#### Levantar servicios

```bash
kubectl get all

minikube service pgadmin-service
minikube service backend-service
```

##### Made with ❤️ by Leandro Arturi

### Comandos utiles

```bash
minikube pause
minikube unpause
minikube stop
minikube delete --all
minikube service <nombre del deployment>
```

```bash
kubectl get pod
kubectl rollout restart deployment
```

---

##### Made with ❤️ by Leandro Arturi
