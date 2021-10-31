In this step we are going to play a little bit with kube and visualize results with built-in api and kubectl cli.

(Be patient, k9s will come right after ! 💪️)

## Spawn some applications : 

```
helm repo add falcosecurity https://falcosecurity.github.io/charts
helm repo update
kubectl create ns falco
helm install falco -n falco falcosecurity/falco
```{{execute interrupt T1}}

## Use kubectl to see your apps and their status : 
```
kubectl get pods -n falco
```{{execute T1}}

## Create nginx deployment
```
kubectl create deployment nginx --image=nginx -n falco
```{{execute T1}}

## Look at my deployment
```
kubectl get deployments -n falco
```{{execute T1}}

## Look at my pod with nginx image, created by this deployment:
```
kubectl get pods -n falco
```{{execute T1}}