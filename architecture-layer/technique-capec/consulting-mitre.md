# CAPEC CAWE CWE

## Traversing CAPEC
The first step to using this methodology consists of going to the CAPEC website found at [capec.mitre.org](https://capec.mitre.org/). The starting page should look something look the following:

![CAPEC Website](capec-website.png)

On the website, there are currently 2 main "views" within CAPEC: mechanisms of attack or domains of attack (see left side, "CAPEC List Quick Access").
Linking this to the context model background, mechanisms focus more on threats in interaction between components whereas domains focus more on threats within entities themselves.
Clicking through to the desired view a collection of high level categories will be presented.
Expanding these show individual threats.
These individual threats are of interest in this step.

**adjust this to expand access control**
![CAPEC mechanisms of attack](capec-mechanisms-of-attack.png)

Clicking one will result in the following image.
**image capec example**
it lists a description, relationships, prerequisites, execution flows, mitigations and occasionally weaknesses.

![CAPEC exploitation of trusted identifiers](capec-exploitation-of-trusted-identifiers.png)

There's a lot of information here to go through, but initially the most important section to focus on is actually found at the bottom, under relevant weaknesses.
What this section actually does is it links the current CAPEC -- a threat, to potential weaknesses -- vulnerabilities.
Recall from the previous section where this technique was explained at a higher level that there exists a catalogue of architectural weaknesses (CAWE).
Unfortunately, MITRE does not provide its own catalog of of architectural threats, the threats found through CAPEC are cross-level and include system threats that are not relevant for the architectural level.
However, because MITRE does have an architectural view at the weakness level (CAWE), this weakness catalog can be used to cross-reference the threat catalog to determine whether or not a threat is an architectural threat.
Simply, a threat is an architectural threat if it has relevant architectural weaknesses.
So after identifying a CAPEC, inspect the listed CWEs to determine whether any are architectural weaknesses.



## Interpreting C(A)WEs
Pictures: CAPEC website
