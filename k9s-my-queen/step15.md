## Pulse view
When you have kubernetes metrics collected on your cluster, you can visualize them with Pulse view ! 

Try on review cluster 
```
pulse
```{{execute T1}}

## Introducing Popeye
Try on review cluster 
```
pop api
```{{execute T1}}

[Popeye](https://popeyecli.io/) is an open-source tool that helps you sanitize your cluster 🤗️
At the top, you can notice a global score (58 - Category E for api namespace in review cluster).

For example, Popeye allows you to see : 
- Unused Service accounts
- Unhealthy ReplicatSets


Popeye does not do any actions on your behalf on the cluster, it just lists you the problematic ressources.
Try 
```
pop all
```{{execute T1}} 
to get a full overview of review cluster 💯️