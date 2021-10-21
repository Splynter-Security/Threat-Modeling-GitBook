# Identification

```
Input: System threat models
Output: Concrete threat lists/overviews
Tools: Brainstorming techniques, generic threat catalogs/libraries
```
Threat identification in the architectural layer enjoys less of the rich historic research background as modeling did due to modeling's relative importance in the field of risk management.
Putting threats in a central position is a more recent evolution specific to cyber security and the discipline of "red teaming".
However, there is still extensive literature to fall back on especially coming from the software architecture industry as well as the widespread standardization and cataloging efforts in cyber security.
Identification is largely a brainstorming step and similar techniques to systems layer threat identification can be applied.

In the following paragraphs the concept of threats will be further explored and an overview of brainstorming techniques will be given.

## Threat Concept
As touched upon in the modeling step, threats are central to threat modeling, it is in the name after all.
Threat - Threat Event - Threat Actors.
Recall, the main goal of threat identification is to use the results of the modeling efforts to generate a list of threats likely to impact the architecture being developed.

## Architectural Threats
In a sense building an overview of "architectural threats".
This does lead to an important question: what is an architectural threat?
As stated before, currently threat modeling in practice is mostly applied at the system layer meaning existing threat definitions mostly focus solely on the system layer, a clear definition of architectural threats is vital to continue.

**INSERT DEFINITION OF ARCHITECTURAL THREAT AND EXAMPLES**

Some architectural threat examples:
* Adversary in the Middle (AiTM)
* Exploitation of Trusted Identifiers
* Software Integrity Attack

from capec.mitre.org


## Threat Actors

## Brainstorming
The rest of this chapter will focus on some brainstorming techniques you can use to identify threats.
Returning to the original question, how to build such a threat overview.
How to go about finding the above defined architectural threats in practice?
Earlier (in chapter methodology) several techniques were touched upon as aides...

A more practical approach to this brainstorming step is using existing threat catalogs.
There is current support for this with MITRE's CAPEC and CAWE.

In case a more loose approach is desired, this more often the case if there is an explicit desire for more custom threat modeling, however.
Ideally there'd be existing mnemonics to be used as is the common practice in system layer threat modeling where STRIDE, LINDUNN, and DREAD are particularly common.
An older technique of performing threat identification in the past, attack trees, however is quite transferable to the architectural layer.
Setting the initial concept front and center and then adding basic categories (such as those found in CAWE "security techniques").

