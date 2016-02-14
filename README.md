# Ethical Passive Detection of Mobile Devices (smartphones)

> This project aims at **detecting the presence/displacement of mobile devices**  from one "local station/cell" **while guaranteeing people's anonymity** and **data transparency** ([civic hacking](https://opengovdata.io/2014/civic-hacking/)).
> With a system made of several of such "local stations/cells", it could monitor the movement of people/crowd anonymously, e.g. enabling a global picture of pedestrians travelling within the city.

### Why tracking mobile devices?

Many public transportation systems today are sharing their data, e.g. bus/metro/tram/train trafic data, and even car trafic data sometimes. These datasets allow to analyze the efficiency of each system, detect chronic delays or congestions which are key informations to implement corrective actions. All together they can help improve a global transportation at the level of a city, a region, a state.

The first/last kilometer however is often left out of the analysis, simply because people either walk or ride a bike to start/finish their travel. Within cities, knowing about these path could provide valuable information about where shared-bikes, buses, trams or taxis should be more or less available.

### How to track pedestrians/bikers ethically?

In order to monitor pedestrians' travels *"ethically"*, the system **MUST guarantee the anonymity of the people** whose presence is detected. In this case **"privacy by design"** is ensured in the **open-sourced code of each tracking device**, where anyone can check that **no personal data is sent to the central/gathering unit**. Personal data might be shared among neighboring tracking devices for a short time only, in order to track the same smartphone moving along consecutive cells. This system could be seen a **swarm of ethical tracking devices** useful to improve further a global transportation system.

The tracking part can easily be done using wifi and bluetooth beacons sent by mobile phones all the time to scan for possible connections. Since we never connect to them, the information monitored is limited to their MAC address.

In order to deploy such system for civic use, for example over an entire city, the code used within those devices has to be open sourced and the results accessible to the public. The system itself must ensure anonymity and none of the information about any individual (here their MAC address) should be sent to the central/gathering unit, neither stored for too long in the tracking devices.

Practically it means we need to keep the MAC adress of a mobile device in the "local station" to track its presence within, let's say 5-30 minutes so that we avoid counting the same device as a new person every 10 seconds. However above 30 minutes or so, the same device (e.g. the same person) walking nearby again will be counted as new mobile device, and account for a new anonymous trip within the system.

### Examples of applications

As every technology, this one could be misused, but built *ethically*, the resulting applications can only benefit the community. Here is a list of a few useful insights such applications could provide:
* for transport systems in cities: by identifying users' hotspots and the displacement of pedestrians between various public transport systems,
* for shopping malls: to organize their shelves and provide a more intuitive experience to the customers,
* for any crowded indoor/outdoor event: where the congestion may critically impact the flow of people, hence their safety,
* for domotic applications: to trigger actions when the presence of people is detected moving between rooms (e.g. switch on/off lights when people are getting close/away from the tracking device.)
* ...
