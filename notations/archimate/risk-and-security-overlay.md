<!-- TODO: Remove the <br/> breakpoints within the table if gitbook does this modelling themselves-->
# Risk and Security Overlay

The ArchiMate standard explicitly defined itself to be extensible.
One of the main building blocks to support this goal is the ability for individuals to develop ArchiMate "overlays" these are extended specifications of ArchiMate using basic ArchiMate building blocks to allow for more expressiveness.
An example of such an overlay is specifically important for threat modeling: the ArchiMate risk and security overlay.
This overlay has become part of ...
The white paper updated for ArchiMate 3.1 can be found here. This chapter will outline the theoretical foundation, main building blocks as well as practical examples of the overlay.

In what follows we will introduce each individual risk management concept and how it is mapped to the ArchiMate standard.
Note: this entire sub-chapter includes definitions and concepts directly from the risk and security overlay whitepaper.
However, this white paper was written about risk management at a higher level, not specifically cyber security threat modelling.
We will therefore focus more on the relevant components.

## Mapping Risk and Security concepts to ArchiMate
The definitions and mapping are near identical copies of those found in the whitepaper.
Sometimes slightly adjusted to focus more on threat modelling instead of risk management.

### Risk
**Risk** can be defined as the probably frequency and probable magnitude of future loss.
Risk also includes the potential of a potentially undesirable outcome (loss) resulting from a given action, activity, and/or inaction foreseen and unforeseen. Mapping the concept of risk in ArchiMate can be done with the assessment concept. In a threat model however, risk itself is not commonly modelled. What is far more useful is to model individual threats, control measures, etc.

**Risk metrics** are metrics used to quantify risk. These should be included as attributes to the risk concept.

### Loss Event
A **loss event** is 

### Threat
**Threats** are possible dangers that could exploit a vulnerability. It can refer to a threatening circumstance, an entity capable of causing harm, or the actual event that may cause harm. The general notion of a threat can be modelled as an ArchiMate driver, however since threat is an ambiguous term, more specific notions of threat are also used to more precisely model threats.

The term **Threat Agent** refers to the above entity capable of causing harm. Note, this can be both intentional; a hacker with malicious intent, or accidental; an employee accidentally types the wrong bash command. There exist various active structure ArchiMate elements that could be used to model threat agents. In practice, business actor elements are commonly used.

In contrast to threat agent, a **Threat Event** refers to the actual event that may cause harm. Similar to threat agents, threat events can be naturally mapped to the business event element.

***Note:*** When we talk about an *attack* this is a specific type of threat event that is the result of an *attacker's*, a specific kind of threat agent, intentional malicious activity.

***TODO: Add picture of the various kinds of threats***

### Vulnerability
A **vulnerability** within cyber security contexts can be defined as a weakness that allows an attacker to threaten the value of an asset. An assessment can be used to model these, however one does not typically want to model vulnerabilities themselves. In an architectural model, known vulnerabilities should be scarce. The focus should lie on threats.

### Domain




## Concept Mapping Table
This table has been made with terminology as found in the security overlay.
Refer to page for more specific terminology.

| Concept | Summary | Mapping |
| --- | --- | --- |
| Risk | The potential of loss -- probable frequency and probable magnitude<br/> of future loss |Assessment  |
| Risk Metrics | TODO | |
| Loss Event | Circumstance that causes loss or damage to an asset | business event |
| Threat | Possible danger that might exploit a vulnerability | driver |
| Threat Agent | Anything capable of acting against an asset in a harmful manner | various active structure elements |
| Threat Event | Event with the potential to adversely impact an asset | |
| Vulnerability | Weakness that allows an attacker to threaten the value of an asset | |
| Domain | A set related entities that share characteristics and define a specific field | |
| Security Domain | Group of assets with the same security level under the same <br/> security policy's jurisdiction | |
| Risk Management <br/> Domain | A domain with shared risk management or security characteristics| |
| Mitigation Domain | A group of assets and actions that together mitigate risk in <br/>one or more risk management domains| |
| Risk Control, <br/> Treatment, Mitigation | Deployment of a set of services to protect against a threat | |
| Control Requirement | Formal need that must be fulfilled by a control to face a known threat| |
| Asset at Risk | Anything that is capable of being owned or controlled to produce value| |
| Policy | A set of rules which governs the behavior of a system | |

