
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

## Ingress

```bash
kubectl apply -f ingress-gogs.yaml
```
Add domain gogs.com to file hosts:

1. go C:\Windows\System32\drivers\etc
2. open hosts file with notepad 
3. add a line with :  youripaddress  gogs.com
4. save and close
5. in navigator click :  http://<youripaddress>/gogs.com