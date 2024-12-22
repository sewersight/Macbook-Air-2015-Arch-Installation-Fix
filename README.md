# Macbook-Air-2015-Arch-Installation-Fix
If for some odd reason your using a 2015 MacBook Air (or anything with broadcom wifi drivers) to install arch linux, here is the fix for you.

Run iwctl device list to make sure nothing appears. If something does, safely ignore this fix.

Inside of the terminal, run rmmod b43, rmmod bcma, rmmod wl, and modprobe wl.
Now do iwctl device list. You should now see something along the lines of wlan0 in the device list.

Enjoy arch installing.
