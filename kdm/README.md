I prefer **lightdm** than **kdm**.  

Install **lightdm** from **epel** repository and use the following instructions to switch to **lightdm** display manager.  
```  
systemctl enable lightdm
```  

Edit **/etc/lightdm/lightdm.conf** and delete the **#** before **greeter-show-manual-login=false** under **\[Seat:\*\]** and modify the **false** to **true** to allow manual login.  
```  
    ...
[Seat:*]
    ...
greeter-show-manual-login=true
    ...
```  
