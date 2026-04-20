# Guard_Dog
Readme file for University of Helsinki AI course ideas
Final project for the Building AI course

## Summary

My project would be to create an AI version of my Guard Dogs. I have two dogs who give excellent warnings when something or someone is not where they are allowed to be. I am proposing an AI guard dog who performs the same task for those people who are unable, for whatever reason, to have a living dog of their own.


## Background

Conventional alarm systems tend to be boolean. Either there is an intrusion to my property or there isn’t. It doesn’t matter if the intrusion is permissible i.e  someone delivering the post or collecting the recycling a perimeter based alarm system will register them. My dogs know when the postman arrives and when the recycle truck is around; and they know that these ‘intruders’ are part of the normal permissible environment and so they don’t make a fuss. On the other hand, if someone disturbs the recycling, human or animal, and it’s dark, they make a lot of noise. The topic is interesting because it involves a problem peculiar to individual circumstances that requires a high level of learned response. (The postman doesn’t always deliver the mail at exactly the same time each day and sometimes there’s no mail at all.)
## How is it used?

My idea  acts as a warning mechanism and a deterrent to unwanted visitors to my home.
It depends upon four main data sources;
The position, number and direction of movement of anything moving within the property
	: postman arrives via garden path, delivers letters into the mailbox, postman departs down garden path
The regularity and repeatability of these patterns of movement.
	: post arrives regularly on weekdays, not at weekends 
The timing of such movements.
	: post arrives during daylight hours, usually in the morning, never at night.
Other behaviour modifying factors.
	:Are the guard dog’s owners on the property? This modifies probability of giving warning.
It gathers data from sensors located around the property and weights these factors appropriately; e.g. movement on the patio behind the house when the owners are not present increases probability of giving warning.
Sensors may be cameras but also could be simple PIR or ultrasound detectors or microphones. Status of owners being present may be strategically evaluated by door lock sensors e.g. majority of exterior doors locked, no interior doors locked, cars parked in their usual places ……owners are probably present. Whereas, all exterior doors locked, all interior doors locked, one or more cars absent……. Owners are probably absent. Timing/calendar data can be from RTC’s or similar.solution needed (environment, time, etc.)? Who are the users, what kinds of needs should be taken into account?

## Data sources and AI methods
Data comes from active sensors and by feedback from the system user in the form of the approval of output; similar to training a live dog.
The AI techniques used will probably be neural networks which can be trained to give responses given certain combinations of input conditions. A certain basic pre-processing would use majority or gated logic and could be implemented in hardware.
## Challenges

The system would be used continuously. It will act as a deterrent to unwanted intruders; the presence of a dog deters burglars, and it will alert neighbours and householders to any unexpected intruders. However there is a problem when the owners are away for any prolonged period. Having used a very basic microphone triggered barking alarm when I have been on vacation once prompted a visit from the humane society: Someone had reported that I had left a dog alone in the house whilst I was away.
The AI would not solve this latter problem and it would also not solve the problem of unexpected circumstances e.g. when animals enter the perimeter at night. However, live dogs also detect this type of intruder and give the same response.  It also does not solve the problem of mimicry; where an intruder pretends to be legitimate by mimicking the behaviour of a regular visitor. In addition, the system relies on the majority of its inputs operating correctly; hardware failures occur or spurious electromagnetic noise may cause false triggering. On a more human level the system will not give the companionship, health benefits or personality of a real, living, dog.
## What next?

The system is meant as an audible deterrent, but it may be extrapolated to more sophisticated intruder detection with more active response scenarios e.g. informing police or other monitoring services.

## Acknowledgments
No external resources have been used in the creation of this idea.
