Let's first wait for Kubernetes to be ready.


### Install k9s
Click the below section to install k9s.
```
curl -fsSL https://github.com/derailed/k9s/releases/download/v0.24.15/k9s_Linux_x86_64.tar.gz --output k9s_Linux_x86_64.tar.gz && tar -xzf k9s_Linux_x86_64.tar.gz --directory /usr/bin k9s
```{{execute interrupt T1}}

### Add secure alias for k9s
```
echo "alias secure-k9s='k9s --readonly'" > .bash_aliases && source .bashrc
```{{execute T1}}

### Check if Kubernetes nodes are ready

Wait for all nodes to be ready.
```
watch kubectl get nodes
```{{execute T1}}
Then hit ```clear```{{execute interrupt T1}} to ctrl + c and cler the screen.