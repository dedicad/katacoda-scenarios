Let's first wait for Kubernetes to be ready.

### Install zsh and Oh-my-zsh for nice coloring
Say yes to zsh as default shell 😉️
```
sudo apt install -qqy zsh && sudo apt install -qqy git-core curl fonts-powerline && sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)" 
```{{execute interrupt T1}}

### Install k9s
Click the below section to install k9s.
```
clear && curl -fsSL https://github.com/derailed/k9s/releases/download/v0.24.15/k9s_Linux_x86_64.tar.gz --output k9s_Linux_x86_64.tar.gz && tar -xzf k9s_Linux_x86_64.tar.gz --directory /usr/bin k9s
```{{execute T1}}

### Add secure alias for k9s
```
echo "alias secure-k9s='k9s --readonly'" >> .zshrc && source .zshrc
```{{execute T1}}

### Check if Kubernetes nodes are ready

Wait for all nodes to be ready.
```
watch kubectl get nodes
```{{execute T1}}
Then hit ```clear```{{execute interrupt T1}} to ctrl + c and cler the screen.