# pi-zero-minimalist-clock

![example blink](https://raw.githubusercontent.com/Crysknife007/pi-zero-minimalist-clock/main/sSo3rFh.gif)

Save the script in your home directory as minimalistClock.sh and make it executable with the command chmod +x minimalClock.sh. Then run it under its own screen with the command screen ./minimalClock.sh since it can be somewhat distracting if running on your main session due to all the echo commands. 

* Use the command sudo apt-get install screen if you don't already have it. 

After getting the clock up and running in screen you can press ctrl+a then ctrl+d to detach the screen and have it keep running in the background.

The clock is read by counting the number of long blinks to get the hours, and then the number of short blinks to get the tenth place of minutes. For example, 4 longer blinks followed by 3 shorter blinks indicates that the current time is about 4:30. 

This script can be included in /etc/rc.local so that it will begin running when the Pi Zero starts up.
