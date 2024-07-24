
# Steps to follow :

these are steps to follow in order to install gogs in kubernetes cluster

## Namespace

```bash
kubectl apply -f namespace.yaml
```

## Persistent Volume

```bash
kubectl apply -f pv.yaml
```
## Persistant Volume Claim

```bash
kubectl apply -f pvc.yaml
```
## Deployment

```bash
kubectl apply -f deployment.yaml
```

## Service

```bash
kubectl apply -f gogs-service.yaml
```
