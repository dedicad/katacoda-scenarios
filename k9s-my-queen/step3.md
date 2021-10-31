Ok let's go ! We are going to use k9s now !

Small tip, to use a command in k9s you may use ':' and then click on the left panel to execute the command 😉️

### Start k9s in readonly mode
```
secure-k9s
```{{execute T1}}

### Visualize nodes with k9s
```
nodes
```{{execute T1}}
You should see exactly the same output as before with
```
kubectl get nodes
```{{execute T2}}



### Tips 
k9s commands works with singular, plural and short-names (e.g. :pods will work but :pod too, :ns will do the same as :namespace )
