# ArchiMate Concept Mapping Table
The ArchiMate standard explicitly defined itself to be extensible. 
One of the main building blocks to support this goal is the ability for individuals to develop ArchiMate "overlays"; 
extended specifications of ArchiMate using basic ArchiMate building blocks to allow for more expressiveness.
An example of such an overlay is especially important for threat modeling: the ArchiMate risk and security overlay. [[1]](#references) [[2]](#references)

This section introduces a table mapping the used concepts to their definitions and how they are mapped in the overlay.
Note, in the section after this one we will expand upon the mappings.
Instead, use this as section more as a reference for definitions and a quick overview for the overlay.

## Risk & Security concepts mapped to ArchiMate
| Concept | Summary | Mapping |
| --- | --- | --- |
| Risk | The potential of loss -- probable frequency and probable magnitude of future loss | Assessment  |
| Risk Metrics | Metrics used to quantify risk | Attributes |
| Loss Event | Circumstance that causes loss or damage to an asset | Business Event |
| Threat | Possible danger that might exploit a vulnerability | Driver |
| Threat Agent | Anything capable of acting against an asset in a harmful manner | Active Structures (Business Actor) |
| Threat Event | Event with the potential to adversely impact an asset | Business Event |
| Asset at Risk | Anything that is capable of being owned or controlled to produce value | Core Elements |
| Vulnerability | Weakness that allows an attacker to threaten the value of an asset | Assessment |
| Domain | A set related entities that share characteristics and define a specific field | Group |
| Security Domain | Group of assets with the same security level under the same security policy's jurisdiction | Group |
| Risk Management Domain | A domain with shared risk management or security characteristics | Group |
| Mitigation Domain | A group of assets and actions that together mitigate risk in one or more risk management domains | Group |
| Risk Control, Treatment, Mitigation | Deployment of a set of services to protect against a threat | Core Elements |
| Control Requirement | Formal need that must be fulfilled by a control to face a known threat | Core Elements complementary to risk controls |
| Policy | A set of rules which governs the behavior of a system | principle |

## References
1: [Modeling Enterprise Risk Management and Security with the ArchiMate® Language](https://researchportal.unamur.be/en/publications/modeling-enterprise-risk-management-and-security-with-the-archima)

2: [Evaluation of the Risk and Security Overlay of ArchiMate to model Information System Security Risks](https://ieeexplore.ieee.org/document/8089840)
