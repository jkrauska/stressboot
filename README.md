# stressboot
A pxebootable live image that runs stress-ng 


Goal:

You've got 100 machines that just got racked.

You have DHCP and DNS ready to go, but you want to run your own stress test based on stress-ng on the boxes to make sure you didn't get any lemons.

(Yes, there are some other things that kinda do this..)

Step 1: Leave Debian Live Systems (live-boot, live-config, live-build).
https://debian-live.alioth.debian.org/live-manual/unstable/manual/html/live-manual.en.html

Step 2: Build a docker container as your build env.

Step 3: Choose what packages and bits you want in your image.

Step 4: Make stress-ng in to a systemd service

Step 5: Copy kernel, initrd and squashfs to a tftp and http server in your boot farm.

Step 6: NetBoot

Step 7: Stress!
