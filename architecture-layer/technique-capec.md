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
MITRE [[1]](#references) is an organization, well known for its att&ck list, a list of threats for applications with a whole database of weaknesses and more.
MITRE's well maintained catalogs are prominent resources for threat modeling and several of them will be very useful for architectural threat modeling.

### CWE
The first MITRE catalog that's important for architectural modeling is CWE [[2]](#references) also known as the Common Weakness Enumeration.
This community maintained catalog lists common weaknesses found in software and hardware.
Note, as mentioned before the end goal of threat identification is not to find weakness but to identify threats.
CWE makes use of "views" to provide different viewpoints of approaching the catalog.
The views select and organize CWEs into different hierarchical catagories.

### CAWE
Out of growing interest in architectural threats, a new specialized "view" of the CWE was made.
This catalog, known as CAWE (Common Architectural Weakness Enumeration) [[3]](#references) focusses specifically on architectural weaknesses.
It identifies which CWE can occur at an architectural instead of simply an implementation level.
Developed as research for the US department of homeland security, it is well peer reviewed and is a cornerstone of this threat identification technique.

### CAPEC
CAPEC [[4]](#references) stands for "Common Attack pattern Enumeration and Classification". 
According to the CAPEC website it "provides a comprehensive dictionary of known patterns of attack employed by adversaries...". 
In essence, it's a huge catalog of threats -- exactly what's necessary for threat identification.
It can be used as a sort of shopping list of threats that can be cross-referenced with the system under analysis to determine whether it is or isn't a potential threat.
An important shortcoming of CAPEC is that it lists all software and hardware threats, not just architectural threats.
This means it's important to use other tools in combination with CAPEC to determine architectural threats to the system.

## How to use it
In the next sections, the topic of using these catalogues will be further explored.
Recall, threat catalogs are part of the threat identification phase, there will be a rudimentary context model already in place and now there is a desire to generate a list of potential threats to the system architecture and to further refine said model.

In brief, the workflow of using the CAPEC threat catalog to perform is as follows:
1) go to CAPEC website and start browsing threats one-by-one
2) determine whether the current threat is an architectural threat or not by cross-referencing with the CAWE catalog through a forward link
3) analyze the threat in relation to the context model
4) document the threat and refine the context model

## References

1: [MITRE](mitre.org)

2: [Common Weakness Enumeration (CWE)](cwe.mitre.org)

3: [Common Architectural Weakness Enumeration (CAWE)](https://www.researchgate.net/publication/317929320_A_Catalog_of_Security_Architecture_Weaknesses)

4: [Common Attack Pattern Enumeration and Classification (CAPEC)](capec.mitre.org)
