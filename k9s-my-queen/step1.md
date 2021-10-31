Let's first wait for Kubernetes to be ready.

### Step: Wait for Kubernetes to be ready

Click the below section which waits for all Kubernetes nodes to be ready.
```
kubectl get nodes
```{{execute T1}}


### Step: Install k9s
Click the below section to install k9s.
```
curl -fsSL https://github.com/derailed/k9s/releases/download/v0.24.15/k9s_Linux_x86_64.tar.gz --output k9s_Linux_x86_64.tar.gz && tar -xzf k9s_Linux_x86_64.tar.gz --directory /usr/bin k9s
```{{execute T1}}

### Add 
```
echo "alias secure-k9s='k9s --readonly'" > .bash_aliases && source .bashrc
```{{execute T1}}
