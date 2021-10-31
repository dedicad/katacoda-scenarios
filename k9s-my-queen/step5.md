As you may know Kubernetes ressources are organized thanks to namespace.

At Gojob, one namespace regroups all ressources of 1 micro-services. Therefore we have namespaces like "hris", "mission-followup" and so on.


To visualize ressources based on a given namespace you just need to add the namespace name after the command. 
For exemple try 

```
pod falco
```{{execute T1}}

```
deployments falco
```{{execute T1}}


❓️🤔️ Great, but  what if I don't know the exact namespace ?
k9s got your back ! Just type ```ns```{{execute T1}} to have a list of all namespace. Then you can use the magic key "/" followed by a regex to directly find your namespace. 

<details>
    <summary>Heuuu okay but concrete example ? 👇️</summary>
    Just do ```ns```{{execute T1}} and see "/" and ```fal``` and the only namespace you should see is "falco" !
</details>

💡️ Whaou this / command looks amazing, can I use it somewhere else 🤩️ ? 

Actually, yes ! Everywhere k9s let you use this command to filter pods, secrets, namespace, etc. Enjoy using it ! 

And you might also leverage its evil twin : "/" + "!". For example try typing "/" then ```!fal```{{execute T1}} you should see only namespace without fal inside !



