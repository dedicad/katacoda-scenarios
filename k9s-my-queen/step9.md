Can you see the cronjob I installed on the cluster ?

<details>
    <summary>Need help ? Toggle me ! 👇️</summary>
    Cronjobs are a kube ressource like any others, just use ```cronjobs```{{execute T1}} to view all cronjobs running on the cluster 💪️
</details>

Ok, no you should be able to enter the pods, see what this cronjob is doing. 

>>Tell me, what is the last log line of the last run ?<<
=== Hello from the Kubernetes cluster

### Trigger me
Alright, now let's suppose something went wrong on the last run and you want to run it now ? 
Just press "t" to trigger this cronjob, check that you have a new pod who ran to execute it !

### Suspend me
Ok let's say (no realistic example) that you're relying on an external service for your cronjob succesfull completion. Let's call this external service "Arhia". 
If Arhia is down, you probably want to stop your cronjobs, so that you're not losing events and generating useless errors. 
k9s helps you again ! 

- Just press "s" to suspend the cronjob and to resume it later on.