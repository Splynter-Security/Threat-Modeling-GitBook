# Technique: CAPEC

CAPEC is a practical technique for establishing a list of potential threats.
It revolves around cross-referencing a prexisting catalogue of known "attack patterns" and a catalogue of known "architectural weaknesses" to find potential architectural threats.
Do note that a common pitfall in this step is to focus on finding vulnerabilities instead of threats.
One of the used catalogs, CAWE, is a catalog of architectural vulnerabilities.
The end goal is not to find vulnerabilities in the system under analysis but to identify potential threats.
Potential vulnerabilities however are interesting to find potential threats that could exploit these.

## Background

Using threat catalogs to perform threat identification requires the usage of previously well established catalogs.
This means it's important to vet the resources to be used.

### MITRE
MITRE is an organization, well known for its att&ck list, a list of threats for applications with a whole database of weaknesses and more.
MITRE's catalogs are prominant reso

### CWE
Common Weakness Enumeration.
Maintained by MITRE, this enumeration focusses on vulnerabilities.
A CWE is the base unit of MITRE catalogs.

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
