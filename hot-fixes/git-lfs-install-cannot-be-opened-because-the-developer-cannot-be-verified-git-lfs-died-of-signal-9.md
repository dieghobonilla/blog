## Git lfs install cannot be opened because the developer cannot be verified
Also seen as **git-lfs died of signal 9**

```
- run "sudo spctl --master-disable" in the terminal.
- install git-lfs as normal
- run "sudo spctl --master-enable"
```

Fix details [here](https://github.com/git-lfs/git-lfs/issues/3714) 

I found a quick workaround until a signed version is released.

Basically, you want to set "Allow apps downloaded from anywhere" in Settings/Security & Privacy. In Catalina, this option isn't available but you can do it with the terminal command "sudo spctl --master-disable".

So the basic procedure is as follows:

- run "sudo spctl --master-disable" in the terminal.
- install git-lfs as normal
- Go to settings/security and privacy and select "Allow apps downloaded from App Store and identified developers" (this is optional but probably good practice to restore things back to the default).
- run "sudo spctl --master-enable"
---------