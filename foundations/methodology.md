# Methodology

"Threat Modeling" isn't just a one-and-done activity.
It's more a discipline consisting of several different steps and techniques to get a holistic overview of risk to a system and controls to manage these threats.
Threat modeling should actually be seen as a constant cyclic refinement of understanding.

While there isn't one set agreed upon methodology for threat modeling, most literature [[1]](#references)[[2]](#references) describe similar phases in the overall lifecycle of a threat model.
Making this a bit more concrete results in the following approach:

```
Context Modeling -> Threat Identification -> Managing Controls
```
The results of each phase are used as the inputs of the next phase and refine the previous phases.

The ideas behind this methodology are cross-layer, being both applicable at the architectural as well as the implementation layer.

## Modeling

Threat modeling cannot be done without first having an idea of the overall context the analysis is situated in.
While this phase is referred to as the "modeling" phase, do not confuse this with "threat modeling" as a whole.
The goal at this point is to end up with a preliminary "risk & security view" of the system under analysis,
initially this might not include any security concepts and looks more like a classic architectural model.
Eventually however, this model will be expanded to become a specialized view able to express security concepts relevant to threat modeling such as threats (events, actors), risks, controls, and more.

Due to the wide variety of pre-existing modeling languages, there's plenty of choice in notation.
Oftentimes pre-existing context models can be used as a preliminary 
However there are several standard notations such as Archimate [[3]](#references) or Dataflow Diagrams (DFD) that are particularly interesting for creating these context models.
They will be explored further in later sections.

## Identification

After having established an initial architectural system model, the threat identification phase begins.
Note, this does not mean your model will remain static from this point on, in fact the opposite is true;
once threats (and later controls) start being identified, the model should be updated to express these concepts as well.
Also of importance in this phase is the identification of threat actors which guides this process and helps refine the context model.

The main goal of threat identification is the creation of a list of threats to the modeled system.
Threat identification is very much a brainstorming phase, threats are after all different for every system.
Threat catalogs, mnemonics, or brainstorm schemas are commonly used to aid in keeping this phase structured and methodical.

## Controls

Finally with the refined context model and an overview of threats in hand, it's possible to start identifying controls to manage these threats.
*This step is not further explored in this version of the course, instead the focus lies on threat identification and how to iteratively model threats themselves.*

# References

1: *Adam Shostack. 2014. Threat Modeling: Designing for Security (1st. ed.). Wiley Publishing.*

2: *K. Yskout, T. Heyman, D. Van Landuyt, L. Sion, K. Wuyts and W. Joosen, "Threat modeling: from infancy to maturity," 2020 IEEE/ACM 42nd International Conference on Software Engineering: New Ideas and Emerging Results (ICSE-NIER), 2020, pp. 9-12.*

3: [Archimate Standard](https://pubs.opengroup.org/architecture/archimate3-doc/)
