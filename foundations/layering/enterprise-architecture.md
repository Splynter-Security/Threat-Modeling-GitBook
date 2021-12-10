## Zachman and SABSA
Layering is not a new concept in information systems (IT) design, nor in security architecture.
The discipline of enterpreise architecture has long seperated business, logical, technological, etc. responsibilities into separate distinct layers with their own properties.

One of the most popular frameworks for layering Enterprise Architecture systems is the Zachman framework.

![The Zachman framework [1]](zachman.jpg)

Of most interest for threat modeling is the leftmost column which seperates the activities (topmost row) into separate layers.
Starting from high abstraction level and decomposing into more concrete IT components as the table is descended.
While the Zachman framework itself is more of a theoretical foundation (and won't be futher explored in this course), it did become part of another more practical framework centered on security architecture: SABSA.

![The SABSA framework [2]](sabsa.jpg)

SABSA (Sherwood Applied Business Security Architecture)[3] uses similar layers as Zachman but redefines them in a security context.
SABSA also includes different models and processes spanning the layers as well as a service management view.
One could view threat modeling as a continuous modeling process in the service management view which models threats on the other layers.

This framework allows for what is truly of interest: defining layers where threat modeling is sensible.
A short overview of the layers:
* Contextual layer: The context of the infrastructure, the broader business vision within it is situated.
* Conceptual layer: The business concepts underlying the infrastructure -- the governance, policies and people involved within it.
* Logical layer: Focusses on the logical responsibilities of things such as services and applications. 
* Physical layer: A more concrete definition of how the former layer is deployed, the kinds of abstract technologies used such as "azure cloud server"
* Component: The actual component itself, how it is implemented and maintained.


This course makes a synthesis of SABSA, identifying 2 dedicated layers on which to perform threat modeling: combining the conceptual and logical layer and calling it architectural and combining the physical and component and calling it system.
This synthesis was used because of its practical usability: eventually layering becomes less useful and more bothersome.
By focusing on the 2 synthesized layers, this can somewhat be avoided.
Of course, these 2 new synthesized layers still have some understanding of the existence of the other layers.
The scope layer as a 3rd layer is of theoretical interest for threat modeling by allowing for threat modeling laws, regulations, visions, mission statements, etc. however it is not practically crucial and will thus not be further explored.

## Piecing it all together

Returning to the original question: "what are we modeling"?
With layering, there are now 2 main "layers" to investigate -- the architectural and implementation layers.
In essence, by investigating the architectural layer, this will give us the roadmap to further investigate the implementation layer.
What components to decompose, what security activities to perform (such as penetration testing), etc.
Implementation layer threat modeling will then aid implementing those activities.
Now it is time to explore threat modeling as a methodology.

## References

1: [Zachman Framework](https://www.zachman.com/)

2: [Zachman Framework Image](https://www.researchgate.net/figure/Zachman-Framework-for-Enterprise-Architecture-the-enterprise-For-example-the-answers_fig3_267300493)

3: [SABSA](https://sabsa.org/sabsa-executive-summary/)
