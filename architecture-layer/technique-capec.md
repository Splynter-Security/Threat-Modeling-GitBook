# Technique: CAPEC

A practical technique for generating a list of threats. Explain it with tactics and weaknesses. Weaknesses are vulnerabilities but not threats. Threats need to be acted upon however they can used to inform your thinking. https://cwe.mitre.org/data/definitions/1000.html Making such a list can look as follows: One often pitfall in building architectural catalogs is confusing threats with vulnerabilities.


## Background

### MITRE
MITRE is an organization, well known for its att&ck list, a list of threats for applications with a whole database of weaknesses and more.

### CAWE
Was developed for the department of homeland security. It is well peer reviewed and became part of the 

### CAPEC
CAPEC stands for "Common Attack pattern Enumeration and Classification". According to the CAPEC website it "provides a comprehensive dictionary of known patterns of attack employed by adversaries...". 
Basically -- it's a huge catalog of threats.
Instead of shopping through amazon, you shop through threats.
These threats are of course of extreme importance in identifying threats in the architecture under development.

## How to use it
As a company, you have your model, cool now what.
Workflow: 1) go to CAPEC, look through threats 2) check if architectural CWE 3) link to model 4) write down the threat 5) add classifiers
Going through this list one by one and considering how a certain threat could apply to your current architecture, if it does 

### Traversing CAPEC
CAPEC website
There are currently 2 main views within CAPEC: mechanisms of attack or domains of attack.
Lining this to your model, mechanisms focus more on interaction between components whereas domains focus more on entities themselves.
Clicking through to the desired view a collection of high level categories will be presented.
Expanding these show individual threats.
These individual threats are of interest in this step.
Clicking one will result in the following image.
**image capec example**
it lists a description, relationships, prerequisites, mitigation and occasionally weaknesses.



### Interpreting C(A)WEs
Pictures: CAPEC website

### Consider CAPEC with Context Model

take an archimate example and do a consideration

### Document the Threat

image: making a list of threats
