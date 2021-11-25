# Synthesizing CAPEC Threats

## Consider CAPEC with Context Model
After having arrived at a CAPEC with an architectural link, the next step is to extract an actual threat from the CAPEC.
Recall, a CAPEC is an attack pattern which is an abstraction of how an attacker would exploit a vulnerability.
Such a pattern is a kind of threat but note: attack patterns are not the only threats to an architecture.
A CAPEC is used to brainstorm threats in combination with the context model.

For example, take **CAPEC-122: Privilege Abuse** in a context with a shared PC connected to a database.
This could lead to identifying of the architectural threat "an employee abuses their access to a shared PC to gain access to the confidential database server".

## Document the Threat
The final step in the technique is to document the actual threat.
Of course, you want to write down the threat in a numbered list somewhere, maybe link it with the explicit CAPEC.
But also important to consider is what meta-information to add.
A small overview of interesting meta-information:

| Meta-Data  | |
| --- | --- |
| Scenario | A scenario that describes how the threat could be exploited in the wild |
| DREAD [[1]](#references)| Damage-Reproducibility-Exploitability-Affected Users-Damage analysis |
| Impact/Feasibility | Simple way of gauging the importance of the threat |
| Related threats | link other threats together showing alternative ways of interpreting a threat |
| Components | Instead of documenting an explicit threat for each and every potential issue, write a generic threat and link the potentially affected components separately |
| Sub/Super-Threats | What does this threat look in a different enterprise layer


## Common Pitfalls
Of course, there are several potential pitfalls when trying to analyze a potential threat.
Here already a couple to consider when applying the CAPEC threat catalog.

### Overlapping Threats

CAPEC attack patterns will sometimes lead to identifying the same kind of threat or very similar ones in multiple different CAPECs.
As an example take **CAPEC-151: Identity Spoofing** and **CAPEC-21: Privilege Abuse**.
Both of these threats are quite similar in an architecture even if the attack patterns are different.
Think about a malevolent employee that abuses their privileges as an employee to impersonate another employee with more rights to a specific document or drive.
It's possible to arrive at this threat when considering both CAPECs individually however it's not practical to create a list of threats with many duplicates.
One way to help diminish this issue is by tracking "related threats", by doing this each new threat needs a reason to exist and if it's similar to another threat, it's easy to navigate between them.
In a way, creating a broader threat by virtually combining smaller ones.

### Missing generalizations

Due to the way cross-referencing works it's sometimes tricky to stay at the same conceptual layer.
If examining **CAPEC-28 Fuzzing**, as an example, this is an architectural threat but the reason why is the CAWE **CWE-20 Improper input Validation**.
While this CAWE does lead to various architectural threats, someone fuzzing a badly validated input field is a kind of architectural threat.
It doesn't really fit neatly in the architectural layer, there is a sense of it being too implementation based.
When such a threat is found, it's useful to think about how to generalize this threat.
In the end, the goal again, is to find a list of threats -- CAPEC is simply a tool.
For example, fuzzing can be generalized as ... **NOT SURE YET HOW TO GENERALIZE IT MYSELF**

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

### CAPEC has an engineering background

CAPEC as a tool was initially made for security developers or engineers -- it has a rich background in the implementation layer.
This does make it less natural to be used for the architectural layer.
Sometimes attack patterns might have clunky names or there are a few kinds of architectural threats that are not able to captured using CAPEC.
This is why it's important to complement CAPEC with other tools like OSA.

## References

1: [DREAD](https://en.wikipedia.org/wiki/DREAD_(risk_assessment_model))
