# Identification

```
Input: Context threat models
Output: Concrete threat lists/overviews
Tools: Brainstorming techniques, generic threat catalogs/libraries
```
Threat identification in the architectural layer enjoys a poorer historic research background as modeling.
Mostly due to modeling's relative importance in the field of risk management.
Putting threats front-and-center comes more out of the cyber security industry and the discipline of "red teaming" which tends to focus more on the systems layer.
Luckily there is still extensive literature to fall back on especially from the field of software architecture as well as the widespread standardization and cataloging efforts in cyber security.

Architectural threat identification is largely a brainstorming phase and similar techniques to systems layer threat identification can be applied. This section's following paragraphs will explore the concept of threats and provide and overview of brainstorming techniques -- these techniques will then be explored more in-depth in the next sections.

## Concept of "Threats"
As touched upon in the modeling step, threats are central to threat modeling, it is in the name after all.
Threat - Threat Event - Threat Actors.
Recall, the main goal of threat identification is to use the results of the modeling efforts to generate a list of threats likely to impact the architecture being developed.
Threat actors are more used to inform these threats and refine the context model.

## Threat Actors
...

## Architectural Threats
This does lead to an important question: what is an architectural threat?
As stated before, currently threat modeling in practice is mostly applied at the system layer meaning existing threat definitions mostly focus solely on the system layer, a clear definition of architectural threats is vital to continue.

Am architectural threat is...
**INSERT DEFINITION OF ARCHITECTURAL THREAT AND EXAMPLES**

Some architectural threat examples (from capec.mitre.org):
* Adversary in the Middle (AiTM)
* Exploitation of Trusted Identifiers
* Software Integrity Attack


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

