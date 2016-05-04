# qdisc
simple script for network queuing for linux


cribbed from https://wiki.gentoo.org/wiki/Traffic_shaping

Slowly adding some features and tweaks.

You can put some defaults either in /etc/qdisc.conf or /etc/default/qdisc, and the script will
read the file and override the defaults.

It should be *mostly* automagic between 1kb/s and 1gb/s, but no testing has been done below 256kb or above 1gb/s

usage:  
qdisc [start|stop]{_ingress|_egress} | restart | flush | status

   start	- enables bidirectional queuing  
   stop		- disables queuing  
   flush	- stops, then unloads modules  
   restart	- stops, then starts bidirectional queuing  

  start_ingress - one-sided queuing (downloads)  
   start_egress	- one-sided queuing (uploads)  

   status	- displays queue information

