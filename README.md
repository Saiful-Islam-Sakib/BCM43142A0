# BCM43142A0
bluetooth firmware for hp 850 g3 i5 6th gen for linux

the steps are :
- run this command (dmesg | grep -i blue; rfkill list) in terminal and see which file is missing
- then download the missing file from internet
- and paste the file in the specified folder(/lib/firmware/ or /lib/firmware/brcm/) showed in the first step.
in my case, the desired file is given....

# run the commands for wifi not found problem
- sudo apt-get update
- sudo apt-get install linux-image-$(uname -r|sed 's,[^-]*-[^-]*-,,') linux-headers-$(uname -r|sed 's,[^-]*-[^-]*-,,') broadcom-sta-dkms
- sudo modprobe -r b44 b43 b43legacy ssb brcmsmac bcma
- sudo modprobe wl 
