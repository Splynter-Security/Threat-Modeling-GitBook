# Technique: OSA

Typically, identifying threat actors is an overlooked element in threat modeling. It doesn't tend to be an explicit step in threat identification and at best is implicitly done during context modeling. However, taking time to do more explicit identification of threats definitely can have a positive effect on providing a more holistic overview of threats. They help to refine the context model as well as can be used when judging impact and feasibility of specific threats.

In this section OSA's (Open Security Architecture) threat actor model will be explored. OSA is a world-wide recognized open source community which publishes security controls and patterns.

## The OSA Threat Catalogue

![OSA Model](OSA.jpg)

The OSA threat catalogue is made up of sub-spaces in 3 orthogonal dimensions which are modeled as seen on the diagram Threat actors fit into a point on this 3-dimensional space. The motivation vector defines 2 spaces: accidental and deliberate actors. The localization vector also defines 2: the external and internal actors. The agent vector defines 3 sub-spaces: human actor, technological actor and force majeur actors.

### Motivation dimension

The motivation dimension defines the dimension that defines the intentions of the the threat actor. It is somewhat straight-forward and since the only options are "accidental and "deliberate",

### Localization dimension

Localization in the OSA context is tied to the origin of the threat being exploited. Either this origin is from within or outside the system under analysis. The answer to this question leads to the position on the axis being either internal or external.

### Force Majeur dimension

The force majeur dimension defines what kind of agent the actor is. In a way, in what kind of universe it's understood to exist, the sub-spaces make this a bit more clear. The human agent is as one would expect any kind of human actor such as users, attackers, APTs, etc. A technological agent creates threats that are tied to physical or chemical processes. OSA uses as an example aging processes. Finally, a force majeur actors are predominately environment-like such as tropical storms, earthquakes, water, etc.

## Shortcomings

OSA does have shortcomings however. While any threat actor can be mapped onto the OSA model, it is sometimes lacking as a tool for brainstorming threat actors. There are after all, for example, many kinds of deliberate internal human actors such as disgruntled employees, malicious suppliers. cloud platforms that process data in an undesired fashion, thieves, APTs... In order to provide a bit more guidance in identifying these actors, it can be useful to supplement the OSA threat catalogue with another dimension. For example, by introducing a "relational" dimension which defines actors in accordance to their relation to the system under analysis. The spaces are then defined on an additional axis of internal (within the system itself), supplier, and unknown. Note, this is different from localization which focuses on the origin of the threat actor, not the relation of the threat actor to the system.

## Example Table

A good way to document OSA threat actors is to map them into a table, below an example of such a table for a simple architecture.

| **Relation →**<br/>**Motivation-Localization ↓** | **Internal** | **Supplier** | **Unknown** |
| --- | --- | --- | --- |
| **Internal-Deliberate** | <mark style="color:yellow;">Employee</mark> | <mark style="color:yellow;">Software Contractor</mark>, <mark style="color:yellow;">Cloud Provider</mark>, <mark style="color:yellow;">Library Developer</mark> | <mark style="color:yellow;">Thief</mark>, <mark style="color:yellow;">APT</mark> |
| **Internal-Accidental** | <mark style="color:yellow;">Employee</mark>, <mark style="color:green;">Server Hardware</mark>, <mark style="color:green;">Employee Hardware</mark> | <mark style="color:yellow;">Software Contractor</mark>, <mark style="color:yellow;">Cloud Provider</mark>, <mark style="color:yellow;">Library Developer</mark> | |
| **External-Deliberate** | <mark style="color:yellow;">Remote Employee</mark> | <mark style="color:yellow;">ISP</mark> | <mark style="color:yellow;">Hacker</mark>, <mark style="color:blue;">Alien Invasion</mark> |
| **External-Accidental** | <mark style="color:yellow;">Remote Employee</mark> | <mark style="color:yellow;">ISP</mark>, <mark style="color:green;">The Internet</mark> | <mark style="color:blue;">Natural Disaster</mark> |

<mark style="color:yellow;">*Human Actor*</mark>, 
<mark style="color:green;">*Technology Actor*</mark>, 
<mark style="color:blue;">*Force Majeur Actor*</mark>

## Conclusion

As seen, threat actors are important tools for model refinement. This will be of particular use later when judging impact and feasibility of threats in threat identification. On another note, threat actors could also be used on their own as starting points for a more freestyle technique of threat identification "what could a deliberate external actor do to the system architecture?"
