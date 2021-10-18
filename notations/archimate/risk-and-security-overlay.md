<!-- TODO: Remove the <br/> breakpoints within the table if gitbook does this modelling themselves-->
# Risk and Security Overlay

The Archimate standard explicitly defined itself to be extensible.
One of the main building blocks to support this goal is the ability for individuals to develop archimate "overlays" these are extended specifications of archimate using basic archimate building blocks to allow for more expressiveness.
An example of such an overlay is specifically important for threat modeling: the Archimate risk and security overlay.
This overlay has become part of ...
The white paper updated for Archimate 3.1 can be found here. This chapter will outline the theoretical foundation, main building blocks as well as practical examples of the overlay.

In what follows we will introduce each individual risk management concept and how it is mapped to the archimate standard.

## Mapping Risk and Security concepts to Archimate

### Risk
Risk, as defined by .
It can be represented as

### Loss Event

### Vulnerability

### Threat

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

