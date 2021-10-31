Dangerous manipulation !! Understand them well in sandboxes before replicating them on review cluster (don't start me on production cluster !!! 👿️)
**From now on and on future steps, we will use k9s to break everything** so quit readonly mode ! Just click here : 
```
k9s
```{{execute interrupt T1}}


### Delete a pod
Alright my pod is going crazy, I want to delete it and let kube respawn a new fresh one :
- Access the given pod
```
pods falco
```{{execute T1}}
- use ctrl+d to delete one of the falco pod. you should see the scheduler respawn a new one ! 

🖐️ Okok! But what if I need to delete multiple pods
Hmmm not sure of your use case, but in this situation, you can use the mark feature of k9s. Just press the space bar and the pod should be in green, it's **marked**. You can mark a few pods and then delete all of them in one shot. (Careful of the heart attack in the same time 🤐️)

Oh by the way, you've got trouble viewing what you need ? 
Feel free to use **k9s sorting feature** : 
- shift + a : sorts by age
- shift + n : sorts by name
- shift + s : sorts by status

and many more, see shift + l to see the help screen !

