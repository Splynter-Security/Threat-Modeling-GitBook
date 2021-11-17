# Synthesizing CAPEC Threats

## Consider CAPEC with Context Model
After having arrived at a CAPEC with an architectural link, the next step is to extract an actual threat from the CAPEC.
Recall, a CAPEC is an attack pattern which is an abstraction of how an attacker would exploit a vulnerability.
Such a pattern is a kind of threat but note: attack patterns are not the only threats to an architecture.
A CAPEC is used to brainstorm threats in combination with the context model.

For example, take CAPEC-122: Privilege Abuse.
**Take an archimate example and do a consideration.**

## Common Pitfalls

### Overlapping Threats
CAPEC attack patterns will sometimes lead to identifying the same kind of threat in multiple different CAPECs.
As an example CAPEC

### Missing generalizations


### Bad Prioritization

The main goal of threat catalogs is to provide an as exhaustive as possible catalog of threats in certain contexts.
CAPEC attempts to do this for cyber-attack patterns.
However, CAPEC does no work in prioritizing certain attack patterns over others, this means that in a brainstorming exercise with threat catalogs it's easy to get stuck in a loop of continually identifying new threats that might not be as relevant.
Here it's important to separate first and second order threats.
A first order threat is a threat that assumes very little or no previously established power in the system under analysis.
Basically a threat where a complete outsider could cause harm -- someone breaking in through the front or back door.
A second order threat is a threat that assumes the attacker has at least some kind of previously established position within the system.
For example, a thief broke into a home and is now waiting until the owners return to kidnap them.
For the most part, try to keep the analysis focused on first order threats.
Do note that some second order threats can sometimes be as or more important than certain first order threats.
A good example of this could be important privilege escalation threats.
Additional analysis like OSA help and proper documentation help reduce this issue.

## Document the Threat

image: making a list of threats

## Common Pitfalls

## Tips & Tricks
