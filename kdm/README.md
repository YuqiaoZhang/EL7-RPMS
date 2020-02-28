I prefer **lightdm** than **kdm**.  

Install **lightdm** from **epel** repository and use the following instructions to switch to **lightdm** display manager.  
```  
systemctl enable lightdm
```  

Edit **/etc/lightdm/lightdm.conf** and add the following lines to allow manual login.  
```  
[SeatDefaults]
greeter-show-manual-login=true
```  
