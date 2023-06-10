```plaintext
 .d8888b. 8888888 8888888888 88888888888                                               
d88P  Y88b  888   888            888                                                   
Y88b.       888   888            888                                                   
 "Y888b.    888   8888888        888           .d88888  .d88b.  88888b.d88b.  888  888 
    "Y88b.  888   888            888          d88" 888 d8P  Y8b 888 "888 "88b 888  888 
      "888  888   888            888   888888 888  888 88888888 888  888  888 888  888 
Y88b  d88P  888   888            888          Y88b 888 Y8b.     888  888  888 Y88b 888 
 "Y8888P" 8888888 888            888           "Y88888  "Y8888  888  888  888  "Y88888 
                                                   888                                 
                                                   888                                 
                                                   888
[*] Forensic toolkit of SANS
[*] Running on qemu-kvm... 
```
## Intro

This project help you to deploy the VM **`SIFT-SANS`** (forensic-toolkit) on qemu-kvm!

## Instructions

1. Download the **.ova** from *https://www.sans.org/tools/sift-workstation/*
2. Extract file **SIFT-Workstation.ova** with this command:

```bash
tar -xvf SIFT-Workstation.ova
```

3. Now is necesary convert file **.vmdk** to **.qcow2**(disk image of qemu) with this command:

```bash
qemu-img convert -O qcow2 SIFT-Workstation.vmdk SIFT-Workstation.qcow2
```

4. Create a qemu VM with this image, and run it!

5. If you have problems with the graphical interface:

+ Run TTY with **Alt+F2** or another F-key
+ Login with this credentials: sansforensics | forensics
+ Install a display manager (I prefer **lightdm**)
```bash
sudo apt-get update
sudo apt install lightdm
```
+ Configure **lightdm** as default display manager
```bash
sudo dpkg-reconfigure lightdm
```
+ Reboot if is necesary and after you can run graphical interface for SIFT!

## Credits

<a href="https://www.linkedin.com/in/edgardhq29">Edgard Huanca (a.k.a. v1c4r10us)</a> 
