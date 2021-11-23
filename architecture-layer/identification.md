# Identification

```
Input: Context threat models
Output: Concrete threat lists/overviews
Tools: Brainstorming techniques, generic threat catalogs/libraries
```

After having made a context model with a solid security dimension, it is time to start identifying actual concrete threats.
This phase is known as threat identification.

Unfortunately, threat identification in the architectural layer lacks the same rich historic research background as modeling.
This is mostly due to modeling's relative importance in the field of risk management.
Putting threats front-and-center is a trend that came more out of the cyber security industry and the discipline of "red teaming" which tends to focus more on the systems layer.
Luckily there is still extensive literature to fall back on, especially in software architecture, as well as the widespread standardization and cataloging efforts in cyber security.

Architectural threat identification is largely a brainstorming effort and similar techniques to systems layer threat identification can be applied. 
This section's following paragraphs will explore the concept of threats and provide and overview of brainstorming techniques -- those techniques will then be explored more in-depth in the next sections.

## Concept of "Threats"
As touched upon in the modeling step and the name implies, threats are central to threat modeling.
Reviewing the distinction between the kinds of threats: a threat is a possible danger to the system, a threat actor is anything capable of acting against an asset in a harmful manner, and a threat event is an event with the potential to adversely impact an asset.
Recall, the main goal of threat identification is to use the results of the modeling efforts to generate a list of threats likely to impact the architecture being developed.
Out of these 3 concepts, threats and threat agents are particularly interesting for architectural threat identification.

### Threat Actors
Threat actors are useful for several reasons.
First of all, they aid in refining the context model, using more specifically defined threat actors, a more applicable model can be created.
They are also useful as brainstorming tools to identify more threats.

### Architectural Threats
Since threat modeling in practice is mostly applied at the system layer, most concrete threat definitions focus mostly on that layer.
This leads to the important question: what is an architectural threat?
A clear definition of architectural threats is vital to continue.

First a couple of examples of architectural threats (from capec.mitre.org):
* Adversary in the Middle (AiTM)
* Exploitation of Trusted Identifiers
* Software Integrity Attack

It is evident that these kinds of threats are very abstract and do not describe any technology or even pre-existing assumptions of how a component should function.

An architectural threat is...
**INSERT DEFINITION OF ARCHITECTURAL THREAT**

## Brainstorming
Returning to the original question, how to build such a threat overview.
How does one go about finding the above defined architectural threats in practice?
The rest of this chapter will focus on some brainstorming techniques you can use to identify threats.
Some of these techniques might sound familiar to the attentive reader for they have been explored previously in the methodology section.

To start of with, one of the best ways to do architectural threat modeling is the use of an architectural threat catalog.
Of course in order to be able to use such a practical approach to threat identification there would need to exist threat catalogs that focus more on the architectural dimension.
While there are famous threat catalogs for the system layer (MITRE ATT&CK), it is not entirely evident those would exist at the architectural layer as well.
Luckily there is a currently well supported architectural view to MITRE's CWE named CAWE.
Combining this with MITRE's CAPEC -- a clear methodology for using threat catalogs for architectural threat identification can be made.

In case a more loose approach is desired, for example when there is an explicit desire for more custom threat modeling, a different approach would need to be followed.
Ideally there'd be existing mnemonics to be used as is the common practice in system layer threat modeling where STRIDE, LINDDUN, and DREAD are particularly notable.
Unfortunately this is not the case for architectural threat modeling.
An older technique of performing threat identification in the past, attack trees, however is quite transferable to the architectural layer.
Setting the initial concept front and center and then adding basic categories (such as those found in CAWE "security techniques") provides a good loose bottom up approach to architectural threat identification.
Lastly, it's also possible to use the threat agent refinement during the identification phase as not just an extension of the context model but also as a bottom up brainstorming starting point.
