# Risk and Security Overlay

The ArchiMate standard explicitly defined itself to be extensible. 
One of the main building blocks to support this goal is the ability for individuals to develop ArchiMate "overlays"; 
extended specifications of ArchiMate using basic ArchiMate building blocks to allow for more expressiveness.
An example of such an overlay is especially important for threat modeling: the ArchiMate risk and security overlay. [[1]](#references) [2](#references)

This chapter will outline the theoretical foundation, main building blocks as well as practical examples of the overlay. In what follows we will introduce each individual risk management concept and how it is mapped to the ArchiMate standard. In the next sections an overview table of all these components can be found, use this as reference for any definitions that might be unclear.

## Mapping Risk and Security concepts to ArchiMate

### Risk

Mapping the concept of **risk** in ArchiMate can be done with the _assessment_ concept, for example through specialization. 
In a threat model however, risk itself is not commonly modelled. What is far more useful is to model individual threats, control measures, etc.
**Risk metrics** should be included as _attributes_ to the risk concept.
Finally, a **loss event** (the event that the risk considers) can be mapped to the _business event_ concept.

![Modelling a Risk and Loss event](images/risk-and-loss-event.jpg)

### Threat
The general notion of a **threat** can be modelled as an ArchiMate _driver_, however since threat is an ambiguous term, more specific notions of threat are used to more precisely model threats.
The term **Threat Agent** refers to the above entity capable of causing harm. There exist _various active structure_ ArchiMate elements that could be used to model threat agents. In practice, _business actor_ elements are commonly used. In contrast to threat agent, a **Threat Event** refers to the actual event that may cause harm. 
Similar to threat agents, threat events can be naturally mapped as a specialization to the _business event_ element. 
"Threat Event" in the overlay is what is most commonly referred to as an actual "threat", both terms can be used in modelling for describing this concept. 

_**Note:**_ When we talk about an _attack_ this is a specific type of threat event that is the result of an _attacker's_ (a specific kind of threat agent) intentional malicious activity.

![Example showing the relationships between components, threats and loss events](images/threats-example.jpg)

#### Asset at risk

Anything (tangible or intangible) capable of being owned or controlled to produce value can be referred to as an **asset at risk**. In cyber security contexts, this can an data, device, or other component of the environment that supports information-related activities. Mapping assets can be done with _most or a combination of core elements_ in the ArchiMate specification. A specific "asset" profile could be assigned to the elements, this profile could then have attributes important to to the asset such as its value. In the last example, the database server could be an asset at risk.

#### Vulnerability

A **vulnerability** within cyber security contexts can be defined as a weakness that allows an attacker to threaten the value of an asset. An _assessment_ can be used to model these, either by seeing a vulnerability as a specialization of an assessment or as a specific attribute. However typically vulnerabilities aren't modelled themselves. In an architectural model, known vulnerabilities should be scarce. The focus should lie on threats.
See the example above for an example of how to model a vulnerability.

### Domain

**Domains** can be mapped to the ArchiMate grouping element.
**Security domain**, **risk management domain**, and **mitigation domain** are all examples of specific security domains that could be modelled.
Often, domains are initially copied from the business before becoming more specialized in later threat modeling iterations.
_**Note:**_ In practice defining a security domain is tricky. Recently trends such as zero-trust and defense-in-depth have only made it even more important to be very careful in going about this.

### Controls

**Risk Control**, **Treatment**, **Mitigation** can nearly all, depending on the kind of action, be modelled with  _any core element or combination_ thereof. A grouping can also be used to form a control of several different sub-components.

![Example showing the relationships between risk and controls](images/controls-example.jpg)

#### Control Requirement

**Control Requirements** can be modelled wih _a wide variety of core elements as long as these core elements are complementary_ to those used in modelling risk controls/treatments/mitigations.
In the example above, the control objective is as an example of a control requirement and the control measure is a kind of risk control.

#### Policy


## References