Oh you're pretty damn fast ! This is an optionnal step, depending on your time, you can move on to the next one directly !
**From now on and on future steps, we will use k9s to break everything** so quit readonly mode ! Just click here : 
```
k9s
```{{execute interrupt T1}}

### Cordon a node, heuu What ?
kube allows us to say "hey, I don't want this node to have new pods scheduled on it". This is particularly usefull to update nodes, decommission them, etc. 

In this step I am lead you through this type of operation without entering into necessary details to conduct it in real life.

Alright, we've seen it before but by doing 
```
nodes
```{{execute T1}}
we see all nodes for our cluster. 

>>Our cluster is composed of 2 nodes, what's the name of the essential one ?<<
=== controlplane

Right, just to be sure you won't kill this one 🎚️🎚️! 

Alright let's do the work now, from the node view, you can press the "c" key and cordon the **master node**. 

### Drain a node
Good, good, Now my master is not able to gain new pods, but what if I want to empty it ? 
This is the role of "r" key, it will "drain" the node, therefore removing all pods (except daemonsets and k8s core pods). You might need to tick the "ignore-daemonsets" option. 


**Press it !**

Wow nice, isn't it ? You should see the other node "node01" getting more and more pods coming from the master node. 



For the sake of the exercice, you can uncordon ("u" key) the master node and come back to a normal situation 😊️
