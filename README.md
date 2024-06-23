Thanks to the main creator ive forked his project to run on a specific console.
A lot of users who own MAC OS Laptop or computer don't have access to windows or an ethernet port.

This is a fork of PPPwn (-> PPLGPwn) which works on LG tvs which uses the RJ45 port to communicate over PPPoE
If you have an LG tv, great. 
If you DONT have an LG tv, Go back to google for your situation, this is for LG WEB OS.

Using Mac OS SSH to your television isn't the wisest option, if you keep getting WAITING FOR STAGE 2 shut off PS4 every time, 
this fork may help via ssh. 

Credits
To creator of goldHEN
and the original author of this branch.

Credits 
FinalCionide for helping Mac users with this updated CURL for the original project for PS4 users with consoles model: 2016A.


# PPLGPwn
A method of executing PPPwn through rooted LGTV's.
This method is using the C++ version of PPPwn, made by xfangfang, the link to the repo it's this one:
https://github.com/xfangfang/PPPwn_cpp

It provides a new way of jailbreaking your PS4, using a rooted LGTV.
For more information of which firmwares are supported, visit the link above.

![image](https://github.com/zauceee/PPLGPwn/assets/37784801/068d16b5-051e-4f22-bdf7-b0e3b46e6590)

## Changelog v1.2 -- 16/05/2024
- Added Support for aarch64 TV's
- New option to select if you want PPLGPwn to start when you turn your TV on (Thanks llbranco for the help!)

## Requirements
- Rooted LGTV
- Ethernet cable
- Device to connect to the TV thru ssh (You can use a phone)

## How can I do it?

Firstly you'll need to root your LGTV, the root itself it supported by a couple of models, check both exploits to see if your TV is capable of doing so, more steps on how to root it and activate SSH aswell are available there:
### Root my TV: https://rootmy.tv/
### Dejavuln: https://github.com/throwaway96/dejavuln-autoroot

Secondly, after you jailbreak your own TV (ironic on how we use a jailbroken TV to jailbreak another device lol), you will need to run the ```install.sh``` present in the releases tab on your TV, do it thru this command:

```
FOR THIS FORK BY FinalCionide use: 
wget https://github.com/FinalCionide/PPLGPwn_PS42016A-s/releases/download/Release/install.sh && source ./install.sh
```

**Connect your PS4 to your TV through the Ethernet port, and go in your PS4 set up LAN > PPPoE, and the exploit should be working!**

## How can I execute this with just a click of a button?
1. Head to the [Homebrew Store](https://www.webosbrew.org/) app and download [LG Input Hook](https://repo.webosbrew.org/apps/org.webosbrew.inputhook/)

2. Open the LG Input Hook and head to the link the app gives you in a device that has a web browser (you can also do this in your TV, but it will take more time)

3. Setup this custom **Execute** action to any button you'd like:

```
cd /media/internal/downloads/PPLGPwn && chmod +x ./run.sh && ./run.sh
```   

4. Save your changes

**And done!** The button you setup with the custom action will know execute the exploit everytime you press it!

# NOTES
!! This exploit is made for TV's with the armv7 or aarch64 architectures, I'm unsure if it works on any other different arch, to know your TV chip architecture run ```uname -m``` !!

!! This exploit stage2 runs LightningMod's load from usb payload !!

Proudly **🇵🇹** <3

Thanks to the OpenLGTV and the RootMyTV communities that gave us this TV Jailbreak
Also a thanks to everyone in the PS4 jailbreaking community that gave us the exploits!
And also thanks to all the contributors!
