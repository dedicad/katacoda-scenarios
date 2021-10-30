Let's first wait for Kubernetes to be ready.

### Step: Wait for Kubernetes to be ready

Click the below section which waits for all Kubernetes nodes to be ready.
```
watch kubectl get nodes
```{{execute T1}}


### Step: Install k9s
Click the below section to install k9s.
```
curl -sS https://webinstall.dev/k9s | bash
```{{execute T1}}
