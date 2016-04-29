# qdisc
simple script for network queuing for linux


cribbed from https://wiki.gentoo.org/wiki/Traffic_shaping

Slowly adding some features and tweaks.

usage:  
qdisc [start|stop]{_ingress|_egress} | restart | flush | status

   start	- enables bidirectional queuing  
   stop		- disables queuing  
   flush	- stops, then unloads modules  
   restart	- stops, then starts bidirectional queuing  

  start_ingress - one-sided queuing (downloads)  
   start_egress	- one-sided queuing (uploads)  

   status	- displays queue information

