# Passive device detection

This project simply aims at detecting the presence and maybe the distance of mobile devices from our device, probably made of a Rasberry Pi.  This is done using wifi and bluetooth beacons sent by mobile phones all the time to scan for possible connections. Since we never connect to them, the information monitored is limited to their MAC address and guaranties the anonymity of the people whose presence is detected.

This module could be used for many other appplications, hopefully ethical ones:

* monitor car traffic to detect congestion in cities
* monitor presence of people in rooms to trigger actions (e.g. swith on/off lights when people close/away from the tracking device.)



## LINKS

* https://www.raspberrypi.org/forums/viewtopic.php?f=37&t=47466

## ToDo list

* Trouver un moyen de ne pas demander systematiquement au telephone d'accepter la connection. Essayer autre chose dans le script qu'une demande de connexion, ca doit exister.