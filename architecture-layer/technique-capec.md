# Technique: CAPEC

CAPEC is a practical technique for establishing a list of potential threats.
It revolves around cross-referencing a preexisting catalogue of known "attack patterns" and a catalogue of known "architectural weaknesses" to find potential architectural threats.
Do note that a common pitfall in this step is to focus on finding vulnerabilities instead of threats.
One of the used catalogs, CAWE, is a catalog of architectural vulnerabilities.
The end goal is not to find vulnerabilities in the system under analysis but to identify potential threats.
Potential vulnerabilities however are interesting to find potential threats that could exploit these.

## Background

Using threat catalogs to perform threat identification requires the usage of previously well established catalogs.
This means it's important to vet the resources to be used.

### MITRE
MITRE is an organization, well known for its att&ck list, a list of threats for applications with a whole database of weaknesses and more.
MITRE's well maintained catalogs are prominent resources for threat modeling and several of them will be very useful for architectural threat modeling.

### CWE
The first MITRE catalog that's important for architectural modeling is the CWE also known as the Common Weakness Enumeration.
This community maintained catalog lists common weaknesses found in software and hardware.
Note, as mentioned before the end goal of threat identification is not to find weakness but to identify threats.
CWE makes use of "views" to provide different viewpoints of approaching the catalog.
The views select and organize CWEs into different hierarchical catagories.

### CAWE
Out of growing interest in architectural threats, a new specialized "view" of the CWE was made.
This catalog, known as CAWE (Common Architectural Weakness Enumeration) focusses specifically on architectural weaknesses.
It identifies which CWE can occur at an architectural instead of simply an implementation level.
Developed as research for the US department of homeland security, it is well peer reviewed and is a cornerstone of this threat identification technique.

### CAPEC
CAPEC stands for "Common Attack pattern Enumeration and Classification". 
According to the CAPEC website it "provides a comprehensive dictionary of known patterns of attack employed by adversaries...". 
In essence, it's a huge catalog of threats -- exactly what's necessary for threat identification.
It can be used as a sort of shopping list of threats that can be cross-referenced with the system under analysis to determine whether it is or isn't a potential threat.
An important shortcoming of CAPEC is that it lists all software and hardware threats, not just architectural threats.
This means it's important to use other tools in combination with CAPEC to determine architectural threats to the system.

## How to use it
Recall, threat catalogs are part of the threat identification phase.
At this point, you already have a model.

The workflow of using the CAPEC threat catalog to perform
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
