# Identification

```
Input: Models, Threat Catalogs/Libraries
Output: Threat Lists/Overviews
```
Threat identification in the architectural layer enjoys less of the rich historic research background as modeling did due to risk management.
The central importance of threats in this step is an evolution specific to cyber security and the discipline of "red teaming".
However, there is still extensive literature to fall back on especially coming from the software architecture industry as well as the widespread standardization efforts in cyber security.
Identification is largely a brainstorming step.
In this section the links between traditional... SABSA... will made more clear.


## Architectural Threats
Recall, the main goal of threat identification is to use the results of the modeling efforts to generate a list of threats likely to impact the architecture being developed.
In a sense building an overview of "architectural threats".
This does lead to an important question: what is an architectural threat?
As stated before, currently threat modeling in practice is mostly applied at the system layer meaning existing threat definitions mostly focus solely dimension, a clear definition of architectural threats is vital to continue.

**INSERT DEFINITION OF ARCHITECTURAL THREAT AND EXAMPLES**
encryption as an example?

## Brainstorming
The rest of this chapter will focus on some brainstorming techniques you can use to identify threats.
Returning to the original question, how to build such a threat overview.
How to go about finding the above defined architectural threats in practice?
Earlier (in chapter methodology) several techniques were touched upon as aides...

A more practical approach to this brainstorming step is using existing threat catalogs.
There is current support for this with MITRE's CAPEC and CAWE.

In case a more loose approach is desired, this more often the case if there is an explicit desire for more custom threat modeling, however.
Ideally there'd be existing mnemonics to be used as is the common practice in system layer threat modeling where STRIDE, LINDUN, and DREAD are particularly common.
An older technique of performing threat identification in the past, attack trees, however is quite transferable to the architectural layer.
Setting the initial concept front and center and then adding basic categories (such as those found in CAWE "security techniques").


A practical technique for generating a list of threats.
Explain it with tactics and weaknesses. Weaknesses are vulnerabilities but not threats.
Threats need to be acted upon however they can used to inform your thinking.
https://cwe.mitre.org/data/definitions/1000.html
Making such a list can look as follows:
One often pitfall in building architectural catalogs is confusing threats with vulnerabilities.

