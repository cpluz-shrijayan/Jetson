### Check
    free -m
    
### Disable ZRAM:
    sudo systemctl disable nvzramconfig

### Create 4GB swap file
    sudo fallocate -l 4G /mnt/4GB.swap
    sudo chmod 600 /mnt/4GB.swap
    sudo mkswap /mnt/4GB.swap

# Append the following line to /etc/fstab
    sudo su
    echo "/mnt/4GB.swap swap swap defaults 0 0" >> /etc/fstab
    exit

OR

    sudo vi /etc/fstab
    
Press insert key on keybord

    /mnt/4g.swap swap swap defaults 0 0
    
Press ESC and press Shift + : and press wq

# REBOOT!
    
    free -m
