Waouh k9s is pretty neat ! But I I feel there's a little bit too much on my screen I'am lost !


No problem ! k9s is fully configurable, actually I just added a config file in ~/.config/k9s/views.yml so now restart ```
k9s
```{{execute interrupt T1}} 
and then try to do 
```
pods all
```{{execute T1}}
Have a look : 
```
vim ~/.config/k9s/config.yml
```{{execute T2}}

More info [in the official docs](https://k9scli.io/topics/columns/)

### Config

You can also see the file ~/.config/k9s/config.yml to see lot of parameters you can adjust, for example : 
- Toggle timestamp on logs by default
- sinceSeconds to choose the default past logs to see (default 5 minutes)

## Optionnal : if you have time

### Custom Shortcuts
🖐️ Ok ok, but this is a bit long to access the screen I want to see. 

Yes so you can a hotkey file in ~/.config/k9s/hotkey.yml ! I've added one for you, try to press the touch "m"

This should get you directly to containers of namespace falco ! 
Have a look at the config file : 
```
vim ~/.config/k9s/hotkey.yml
```{{execute T2}}

### Custom commands
You can add your own shortcuts ! For example if you want to see the logs of a pod with a different command, let's say ctrl+l. I've added a ~/.config/k9s/plugin.yml file to do so. Give it a look !
```
vim ~/.config/k9s/plugin.yml
```{{execute T2}}

### Skins
Oh you don't like the colors ? 😖️

You can use personnalized skins 🌈️ ! And the most useful : **One skin per Cluster !** What do you say ? so that you know when you use production or review in one blink 😉️
Click to update the default skin !

```
cp /tmp/skins.yml ~/.config/k9s/
```{{execute T2}}

More info [in the official docs](https://k9scli.io/topics/skins/)

[More skins here](https://github.com/derailed/k9s/tree/master/skins)