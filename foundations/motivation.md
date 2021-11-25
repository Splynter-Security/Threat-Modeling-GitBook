# Motivation

## Why
One morning an engineer wakes up to to messages alerting them that their company infrastructure has been compromised.
Not because of flaws in their software or operational practices however, but due to a critical dependency on a different company.
The news quickly finds it way to the executives of the company who ask themselves how such an issue couldn't be identified earlier.
Is there any way to prevent this from happening?
Perhaps a consistent methodology to chart the security landscape of their company, identifying dangers not just on singular servers but also in the supply chain and beyond.
This is the story of many companies involved in the 2019-2020 Solarwinds attacks [[1]](#references).

![](motivation-cover.jpg)

## What

Identifying dangers to operational infrastructure is far from a recent desire.
Even before the field of cyber security and a company such as Solarwinds even existed it was necessary to chart dangers to physical systems to understand weaknesses to for example theft, war, or even natural disasters.
This domain is known as threat modelling.
In a broad sense, threat modelling is something all of us do every day to understand the dangers (or "threats") in our day-to-day life.
As shown in the earlier example, today, this kind of process should also be done by companies to protect and gain a deeper understanding of their own cyber infrastructure.

## How

In essence, threat modelling should be seen as a process of iteratively refining a defined security model.
Identifying new threats when new components are added, then modelling these threats -- thus maintaining a consistent view of a system's risk profile in its broader environment.
Threat modeling builds a continuous risk analysis documentation that assists future security initiatives in identifying what threats to focus on.

Lots of work has already been done on threat modelling for cyber security.
Microsoft especially has been a big contributor with innovations such as STRIDE and the Secure Development Lifecycle (see Shostack [[3]](#References)).
Also OWASP [[4]](#References), SABSA [[5]](#References), MITRE [[6]](#References) and more are all well respected international organizations that have aided in building the threat modelling movement. 
This course uses many of these entities as references.

## References
1: [SolarWinds Supply Chain Attacks on Wikipedia](https://en.wikipedia.org/wiki/SolarWinds#2019%E2%80%932020_supply_chain_attacks)

2: [Cover image source](https://www.dw.com/en/threat-modeling-guide-how-to-identify-digital-risks-in-international-development-projects/a-55092469)

3: *Adam Shostack. 2014. Threat Modeling: Designing for Security (1st. ed.). Wiley Publishing.*

4: [Open Web Application Security Project (OWASP)](owasp.org)

5: [SABSA Enterprise Security Architecture](sabsa.org/)

6: [MITRE](mitre.org)
