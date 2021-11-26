# Basics

The intention of this chapter is not to give a complete introduction to ArchiMate.
It is assumed that at least some background is already present.
If this is not the case, please refer to the ArchiMate specification for more information. [[1]](#references)
Instead, this chapter will highlight the core concepts and notations used in Archimate that are of interest to be extended for threat modeling.

## Layers

One of the most distinctive elements of the Archimate notation is its clear separation into different layers that can be easily mapped onto TOGAF or Zachman layers.
There are 3 main layers: the business, application, and technology layers.
Again, one of he main goals of Archimate is a common language between different kinds of stakeholders in the business and IT systems within an organization. [[2]](#references)

![Archimate Core Framework, showing the importance of layering in ArchiMate](images/layering.jpg)

For architectural threat modelling, this is an excellent starting point.
Since the architectural layer encompasses the SABSA conceptual and logical layers, architectural threat modeling's responsibilities map quite naturally onto the business and application layers.
However, architectural threat modelling also needs some understanding of the underlying technology to understand how certain threats might manifest themselves.

Also the usefulness of layering comes back in the "why" and "who" of architectural threat modelling.
One of the "why's" being to create documentation to guide future implementation layer efforts to be more direct and efficient.
Since ArchiMate is multi-layer, there is a common language between the "who's" doing traditional threat modelling or penetration testing and the security architects.
Also in the business, the threat model can be explained to any stakeholder ranging from business architects to technical architects who have different views and responsibilities.

## Motivation Overlay

Motivation elements enable analysts to model elements related to goals, outcomes, principles and requirements.
Being able to communicate intention and current information not related to the practical modeling of components is crucial for certain use-cases.
This provides the context that allows for showing complex requirements on ArchiMate models related to the underlying components.
This will be especially relevant for risk management (and threat modeling) since this often is focused on core concepts surrounding requirements and security objectives to supplement the components.

![Motivation Example](images/motivation-example.jpg)

## Overlays and Extensions

Another important concept of Archimate is its ability to be extended with overlays and extensions.
An overlay is xyz.
An extension is xys
Overlays and extensions allow for reuse of the core Archimate specification in contexts that need a bit more refinement of its general purpose layer.

## Grouping

The final concept of interest is the idea of domains. 
A domain is xyz.
This of special interest for security modelling because it maps closely to the idea of a "security domain".
Where components are grouped with similar security requirements and permissions.
Do note that this has implications for threat modeling in zero-trust [[2]](#references) architectures. 

![Motivation Example](images/grouping.jpg)

## References

[1] : 

[2] : https://pubs.opengroup.org/architecture/archimate3-doc/chap01.html#_Toc10045267

[3]: [Motivation example image](https://pubs.opengroup.org/architecture/archimate3-doc/chap06.html)

[4]: [Layering example image](https://pubs.opengroup.org/architecture/archimate3-doc/chap03.html)
