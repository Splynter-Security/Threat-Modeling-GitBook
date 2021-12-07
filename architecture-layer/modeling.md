# Modeling

```
Input: Documentation, implementations, other model views
Output: Context model focused on risk
Tools: Modeling notations
```

Modeling denotes the activity of creating a suitable context model that allows viewing at the system being threat modeled through a risk & security lens.
A model is a visual representation of the overall system under analysis.
With "context" model, there is simply more emphasis on the overall context than just individual components.
The idea of (context) model used in this course maps closely to the concept of a "conceptual model" [[1]](#references)
This model will be used in the later activities to provide a systematic declarative approach to managing security risks.
Of course, before we can use the model, it has to first be drafted - meaning a suitable notation must be chosen.
Architectural modeling as a discipline has a wealth of literature to probe from with new modeling notations being a constant point of development.
Also the field of risk management has influenced these efforts providing a good base for security management threat modeling to build upon.


## Ideal Notation
A natural starting point to find the right modeling language is thus to look at modeling notations specialized in the architectural layer.
A good architectural system model needs to be able to show multi-layer concepts, ideally providing a common abstract language for business and technical analysts to communicate with.
Ideally it's technology independent and able to integrate with lower layer diagrams.


### Risk & Security expressiveness
Amongst these, the ideal notation would preferably also have pre-existing security components that could be  leveraged for threat modeling.
After all, the goal of modeling is to create a suitable context model for managing security risks.
Do note -- we need to be able to find threats in an architectural sense: design flaws, not simply implementation failures or inter-connectivity issues.

### ArchiMate
ArchiMate [[2]](#references) is a notation that ticks all the above boxes -- an open standard modeling notation specialized in cross-layer modeling.
Built upon a strong theoretical foundation of TOGAF [[3]](#references), Zachman [[4]](#references), and SABSA [[5]](#references), it provides a multi-view modeling technique that leverages inter-layer concepts.
Also, a risk and security overlay has already been proposed, providing a toolbox of a diverse array of elements needed for threat modeling activities.
It is widely used in practice, easing adoption as a threat modeling standard is simplified providing business.

## References

1: [Conceptual Model](https://en.wikipedia.org/wiki/Conceptual_model)

2: [Archimate Standard](https://pubs.opengroup.org/architecture/archimate3-doc/)

3: [TOGAF](https://www.opengroup.org/togaf)

4: [Zachman](https://www.zachman.com/images/ZI_PIcs/ZF3.0.jpg)

5: [SABSA](https://sabsa.org/)
