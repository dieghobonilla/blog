## Add Android PATH mac zsh after changing from shell

Good explanation [here](https://youtu.be/yGmN7F4Gfos?t=171) 

```
// Create .zprofile and add
eval $(/usr/libexec/path_helper -s)
export ANDROID_HOME=/Users/$USER/Library/Android/sdk
export PATH=${PATH}:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools
````
---------

<!--stackedit_data:
eyJoaXN0b3J5IjpbODI2MTI0NDI3XX0=
-->