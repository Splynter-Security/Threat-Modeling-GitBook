# Basics

The intention of this chapter is not to give a complete introduction to ArchiMate.
It is assumed that at least some background is already present.
If this is not the case, please refer to the ArchiMate specification for more information. [[1]](#references)
Instead, this chapter will highlight the core concepts and notations used in Archimate that are of interest to be extended for threat modeling.

## Layers

One of the most distinctive elements of the Archimate notation is its clear separation into different layers that can be easily mapped on TOGAF or Zachman layers.
There are 3 main layers: the business, application, and technology layers.

As stated before, archimate is

![Archimate Core Framework, showing how the types of elements exist on multiple layer](images/layering.jpg)


## Motivation OVerlay

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

[2] : 

[3]: [Motivation example image](https://pubs.opengroup.org/architecture/archimate3-doc/chap06.html)

[4]: [Layering example image](https://pubs.opengroup.org/architecture/archimate3-doc/chap03.html)
