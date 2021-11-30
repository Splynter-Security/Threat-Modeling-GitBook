# Layering

As alluded to in the previous section, the concept of treat modeling can be interpreted extremely broadly.
While this course is restricted to cyber infrastructures, even there there are a plethora of different interpretations to make use of.
It's therefore not just vital to understand how to threat model, but also to understand what kind of threat modeling is useful and when.


## Example: a Car

Cars are some of the most widely used examples in demonstrating the necessity of cyber security and it's clear to see why.
Consisting of a large attack surface which includes millions lines of code, complex networking of components, and potentially devastating real life consequences if things go wrong, cyber security (and threat modeling) is crucial in the automotive sector.
Putting on a threat modeling lens and delving into this example will show what is meant by different kinds of threat modeling.

Commonly, when vehicles are threat modeled, this is done at a component level.
Starting on the outside of the vehicle, identifying the potential entry points: bluetooth, Wi-Fi, OBD, etc. and then mapping these onto a diagram creates a Dataflow Diagram (DFD) -- a widespread modeling language for threat modeling components.

![Opengarages example of a "level 0 inputs" DFD [1]](car-example-level_0.jpg)

Next, the car is further explored, going into another level of decomposition.
This kind of decomposition is the first kind of layering, it isn't really explored in this course because it is more useful at the implementation layer then it is the architectural layer (see later).
This next view decomposes the vehicle and shows the actual components of the vehicles

![Opengarages example of a "level 1 inputs" DFD [2]](car-example-level_1.jpg)

After these DFDs are established, threats are able to start being extracted.
For example, with OBD-II access, it is possible to perform a fuzzing attack on the network to extract information about CAN IDs and their protocol schemes.
As might start to become apparent, these kinds of threats are highly technical, and while they may very well be apt for the situation, they are unable to express the breadth of threat to the overall automotive system.
For example, what about third party threats?
Tesla uses over-the-air updates (OTA) to update their vehicles, should this be included in the above diagrams?

In practice, this is where it is useful to start "layering" threat modeling abstractions.
While the car was explored at a more "component" or "implementation"-centric level in the above example,
by reducing the amount of technical specification (e.g. types of portocols), expanding the overall context (what else is the system dependent of?), and focusing on abstract applicability (what are threats to the concepts used instead of the implementations thereof) -- a new kind of view or "layer" can be achieved.
As an example, instead of seeing threats to the CAN bus (the internal networking of a vehicle between e.g. wheels and the dashboard) as specific to the protocol, redefining them into a more general fashion allows for a more hollistic view of the system.
The above fuzzing example threat could be translated to "analyzing the internal network protocol", making the threat more generally applicable and moving it to another layer of abstraction.
Now, if the internal network would change away from CAN to e.g. FireWire (as is the case in military applications), the new threat will still exist within the system because it is inherent in how automotive systems are designed.
These kinds of threats will become known as **architectural threats** whereas the former will be named **implementation threats**.


## Zachman and SABSA
Layering is not a new concept in information systems (IT) design, nor in security architecture.

Zachman
picture

