I prefer **sddm** than **kdm**.  

Install **sddm** and **sddm-themes** from **epel** repository and use the following instructions to switch to **sddm** display manager.  
```  
systemctl enable sddm
```  

Edit **/etc/sddm.conf** and delete the **#** before **MinimumUid=1000** under **\[Users]** and modify the **1000** to **0** to allow root login.  
```  
    ...
[Users]
    ...
MinimumUid=0
    ...
```  
