Ok ok last step was really cool, but how do I debug my application 🛠️ ?


## Visualizing logs
As we saw before, you can access list of pods on a given namespace with a command like this one : 
```
pods falco
```{{execute T1}}
Then you have a in front of you a list of pod, just press "l" to acess logs of the pods. 

🖐️ Well nice, try but I can't see a single line ?
Oh ok, easy, there is some time window option, by default you only see the last 5 minutes of logs. Just press "0" to see all logs 🤙️ ! 

🖐️ Well nice, but I have to do this each time I open a pod logs ? 
Rhaa you're moving too fast 🏃️🏃️🏃️ ! Of course not ! k9s allows you to config most parameters such as this one, but we will only discuss this in Step 12 😫️ !

## An event you said ?
When kube pieces perform an action relatively to a pod (or any ressource) they store an event with this action and the result. 
🖐️ Oh great ! That means I can view previous events and investigate why a pod is nos ready and running ?
Exactly !

You can vizualise this directly on the give pod by **describing** it. The key "d" allows you to describe the pod current configuration and if you roll down to the bottom of the page you will see a list of events.


>>Which element of kubernetes emits the first event ?<<
=== default-scheduler

>>What was the message for one of the running falco pod ?<<
=~= Successfully assigned falco/falco


Well I thought a little schema would be cool now so there it is: 
![Kube Architecture](./assets/components-of-kubernetes.svg)


### Alright, but let's say I want an event overview ?
Well, easy, just use ```events falco```{{execute T1}} for you overview ! 

🖐️ So cool, but I would like to focus only on errors ! I don't care about success (not in general but only there 😁️)
Just type ctrl + z and you will only see errors !

## Wanna do more debugging ?
I believe french people say something like this : Patience est mère de sûreté ! We'll see more invasive methods in Step 11 ⚔️😄️


