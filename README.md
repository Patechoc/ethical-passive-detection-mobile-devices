# Ethical Passive Detection of Mobile Devices (smartphones)

This project simply aims at detecting the presence/displacement of mobile devices from one "local station": [civic hacking](https://opengovdata.io/2014/civic-hacking/) if guaranteeing people anonymity and data transparency.
With a system made of several "local stations", it could allow to monitor displacement within a limited time frame.

In order to monitor *"ethically"*, the system **must guarantee the anonymity of the people** whose presence is detected.

The tracking can easily be done using wifi and bluetooth beacons sent by mobile phones all the time to scan for possible connections. Since we never connect to them, the information monitored is limited to their MAC address.

In order to deploy such system for civic use, for example over an entire city, the code used within those devices has to be open sourced and the results made public. The system itself must be ensure anonymity and none of the information about any individual (here their MAC address) should be sent to the central/gathering unit, neither stored for too many hours.

Practically it means we need to keep the MAC adress  of a mobile device in the "local station" to track its presence within, let's say 5-30 minutes so that we don't count the same device as a new person every 10 seconds. However above 30 minutes or so, the same device (e.g. the same person) walking nearby again will be counted as new.

As every technology, this one could be misused, but if built *ethically*, such applications can only benefit the community, as for example:
* tranport systems in cities: by identifying users' hotspots and the displacement of pedestrians between various public transport systems,
* shopping malls to organize their shelves and provide a more intuitive experience to the customers,
* any crowded events where the congestion critically impacts the flow of people (hence their safety),
* domotic applications: to trigger actions when the presence of people is detected (e.g. swith on/off lights when people close/away from the tracking device.)
* ...



## LINKS

* https://www.raspberrypi.org/forums/viewtopic.php?f=37&t=47466

## ToDo list

* Trouver un moyen de ne pas demander systematiquement au telephone d'accepter la connection. Essayer autre chose dans le script qu'une demande de connexion, ca doit exister.