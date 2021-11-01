Ooookkk, let's dig into debugging now. 

## Yaml defining a ressource
In Kube each ressource is defined by a yaml. Therefore, if you want to see how a ressource (like a pod) was created you just need to access the yaml by using the key **y**. 

## Describe current state of the pod
To describe the current state of one pod, you can press **d** this will give you informations like env variables, events (as we saw before), etc. That can help you understand the current state of your pod.

## See all pods in error in a namespace
Actually you already have all the tools for this, can you see what pod in error I've introduced in namespace falco ?

>>Give me its name !<<
=~= hello-node

<details>
    <summary>Need help ? Toggle me ! 👇️</summary>
    Just use ```pods falco```{{execute T1}} to see pods associated to namespace falco

    Then you can leverage the "ctrl+z" combination to show only pods in error !
</details>

## Toggle wide
Hum, you would like to see in one glance what's going on with this pod ?

**Aie next step doesn't work in browser 😁️** but well you can read it at least to try later on your computer.

Try using "ctrl+w" to toggle wide view and you might have a more precise idea of the error.

## Error
And by the way, did you understand this error ? 

>>Could you spell the first faulty event message for me ?<<
=~= Failed to pull image "registry.gitlab.com/gojob/hris/master"
