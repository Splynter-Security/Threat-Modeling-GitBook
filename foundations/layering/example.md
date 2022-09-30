
## Example: a car

Cars are some of the most widely used examples in demonstrating the necessity of cyber security and it's clear to see why.
Consisting of a large attack surface which includes millions lines of code, complex networking of components, and potentially devastating real life consequences if things go wrong, cyber security (and threat modeling) is crucial in the automotive sector.
It is expected that the connected cars sector will double in the next 5 years [[1]](#references), nearly every new car rolling off the factory line has at least some kinds of smart sensors and functionality embedded within it.
Putting on a threat modeling lens and delving into this example will show what is meant by different kinds of threat modeling.


## Decomposition
Commonly, when vehicles are threat modeled, this is done at a component level.
Starting on the outside of the vehicle, identifying the potential entry points: bluetooth, Wi-Fi, OBD, etc. and then mapping these onto a diagram creates a Dataflow Diagram (DFD) -- a widespread modeling language for threat modeling components. Don't get hung up on the details of the examples. Most things are just abbreviations not necessary for the rest of the course.

![Opengarages example of a "level 0 inputs" DFD [2]](car-example-level_0.jpg)

Next, the car is further explored, going into another level of decomposition.
This kind of decomposition is a simple first kind of layering, it isn't strictly speaking the same as what is meant by "layering" but it is useful for illustrative purposes.
This next view decomposes the vehicle and shows the actual components of the vehicles

![Opengarages example of a "level 1 inputs" DFD [2]](car-example-level_1.jpg)

After these DFDs are established, threats are able to start being extracted.
For example, with OBD-II (On-Board Diagnostics) access, it is possible to perform a fuzzing attack on the network to extract information about CAN (Controller Area Network) identifiers and their protocol schemes. [3](#references)
As might start to become apparent, these kinds of threats are highly technical, and while they may very well be apt for the situation, they are unable to express the breadth of threat to the overall automotive system.
For example, what about third party threats?
Tesla uses over-the-air updates (OTA) to update their vehicles, should this be included in the above diagrams?
What is the subject of the threat modeling activity, an actual physical vehicle or the design and infrastructure it is derived from?
Do threats need to be elicited on the vehicle as it rolls out off the factory floor or on the broader architecture of the vehicle -- how it was designed to work.

## Logical Layering
In practice, this is where it is useful to start "layering" threat modeling abstractions.
While the car was explored at a more "component" or "implementation"-centric level in the above example,
by reducing the amount of technical specification (e.g. types of portocols), expanding the overall context (what else is the system dependent of?), and focusing on abstract applicability (what are threats to the concepts used instead of the implementations thereof) -- a new kind of view or "layer" can be achieved.
As an example, instead of seeing threats to the CAN bus (the internal networking of a vehicle between e.g. wheels and the dashboard) as specific to the protocol, redefining them into a more general fashion allows for a more hollistic view of the system.
The above "fuzzing" example threat could be translated to "analyzing the internal network protocol", making the threat more generally applicable and moving it to another layer of abstraction.
Now, if the internal network would change away from CAN to e.g. FireWire (as is the case in military applications), the new threat will still exist within the system because it is inherent in how automotive systems are designed.
These kinds of threats will become known as **architectural threats** whereas the former will be named **implementation threats**.
Architectural threats also inherently focus more on the overall picture where the component is situated in, this includes its broader OTA infrastructure and V2X and other connectivity.

## References

1: [Connected cars industry growth](https://www.mordorintelligence.com/industry-reports/europe-connected-cars-market)

1: [The Car Hacker's Handbook](http://opengarages.org/handbook/ebook/)

2: *Timothy Werquin, Mathijs Hubrechtsen, Ashok Thangarajan, Frank Piessens, Jan Tobias Mühlberg. "Automated Fuzzing of Automotive Control Units." International Workshop on Attacks and Defenses for Internet-of-Things (ADIoT) / International Workshop on the Secure Internet of Things (SIoT), 2019*

