# BCM43142A0
bluetooth firmware for hp 850 g3 i5 6th gen for linux

the steps are :
- run this command (dmesg | grep -i blue; rfkill list) in terminal and see which file is missing
- then download the missing file from internet
- and paste the file in the specified folder(/lib/firmware/ or /lib/firmware/brcm/) showed in the first step.
in my case, the desired file is given....
