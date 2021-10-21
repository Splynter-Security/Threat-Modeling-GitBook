# Methodology
"Threat Modeling" isn't just a one-and-done activity.
It's more a discipline consisting of several different steps and techniques to get a holistic overview of risk to a system and controls to manage these threats.
Threat modelling should actually be seen as a constant cyclic refinement of understanding.

While there isn't one set agreed upon methodology for threat modeling, most literature [[1]](#references)[[2]](#references) describe similar phases in the overall lifecycle of a threat model. 
Making this a bit more concrete results in the following approach:
```
Context Modeling -> Threat Identification -> Managing Controls
```

The ideas behind this methodology are cross-layer, being both applicable at the architectural as well as the system layer.

## Modeling
The first step in threat modeling is to establish a context model of the system.
This model needs to be a specialized view able to express security concepts relevant to threat modeling such as threats (events, actors), risks, controls, and more.

Due to the wide variety of pre-existing modeling languages, there's plenty of choice in notation.
However there are several standard notations such as Archimate or Dataflow Diagrams (DFD) that are particularly interesting for creating these context models.
They will be explored further in later sections.


## Identification
After having establish an initial architectural system mode, the phase of threat identification begins.
Note, this does not mean your model will remain static from this point on, in fact the opposite is true;
once threats (and later controls) start being identified, the model should be updated to express these concepts as well.

The main goal of threat identification is the creation of a list of threats to the modeled system.
Threat identification is very much a brainstorming phase, threats are after all different for every system.
Threat catalogs, mnemonics such as STRIDE or LINDDUN, or brainstorm schemas are commonly used to aid in keeping this phase structured and methodical.

## Controls
Finally with the refined context model and an overview of threats in hand, it's possible to start identifying controls to manage these threats.


# References

1: Threat Modeling - designing for security by Adam Shostack

2: "Threat modeling: from infancy to maturity"