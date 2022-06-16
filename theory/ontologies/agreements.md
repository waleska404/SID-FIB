# Ontologies: Agreements, Types and Examples

[//]: # (Poner aqui link al pdf/quizas no es muy legal colgar las transpas de otros)

###### tags: `SID-teo`

[ToC]


---


## Ontological Agreements

Agreements to use the vocabulary in a coherent and consistent way.

![](https://i.imgur.com/q3OcuGD.png)

### Man-machine communication
![](https://i.imgur.com/3hbEbG0.png)


---

## Ontology Types

![](https://i.imgur.com/9O0kaga.png)

* **Ask & Tell ontologies** : limited subset of what can be queried and answered **Meta-Ontologies**.

---

## Hierarchy

![](https://i.imgur.com/t2D3NyU.png)

---

## Predicate Calculus Representations

"***Parents love their children***" can be represented as:

![](https://i.imgur.com/oknnP9h.png)

* `For all P, For all C, P is a person AND C is a child of P implies P loves C.`


---


## Reasoning Using Logic

* *Simple Example:*
![](https://i.imgur.com/0Le4eHJ.png)

* *Harder Example:*
![](https://i.imgur.com/FeCu7pA.png)

---

## Fundamental Design Questions

**Syntagmatic** vs **Paradigmatic**
* Syntagmatic –when words appear together in a unit.
* Paradigmatic –if words are linked in a lexical resource.

When we hear a word, many words come to our mind through association.
*Example For cat:*
animal , mammal –Paradigmatic
mew , purr , furry –Syntagmatic

---

## Major Lexical Relations

* Synonymy
* Polysemy
* Metonymy
* Hyponymy/ Hypernymy
* Meronymy/ Holonymy
* Antonymy

### Hyponymy

==**ISA relation**==
* Related to Super ordinate and Subordinate level.
* Categories:
    * hyponym(robin , bird)
    * hyponym(emu, bird)
    * hyponym(bird, animal)
    * hypernym(animal , bird)
* A is a hypernym of B if B is a type of A.
* A is a hyponym of B if A is a type of B.

### Hyponymy vs Synonymy

![](https://i.imgur.com/84kop4g.png)



---

## Examples

### From Simple to Complex

![](https://i.imgur.com/PmBaSB3.png)
![](https://i.imgur.com/pTLw12f.png)
![](https://i.imgur.com/MJgatYS.png)
![](https://i.imgur.com/QwYkR7L.png)


### Cyc (1985)

* Cycorp: "It's just common sense". 
* In CycL over 1 000 000 hand-entered assertions (or "**rules**") designed to capture a large portion of what we normally consider consensus knowledge about the world ("river flows downhill" etc.).
    * Sometimes so called **microtheories** are however necessary difference with domain ontologies?
    * Nevertheless exemplifies the "One large ontology" approach!
* **Opencyc (2003)**: an open source subset of Cyc: 
    * 6 000 concepts: an upper ontology for all of human consensus reality.
    * 60 000 assertions about the 6 000 concepts, interrelating them, constraining them, in effect (partially) defining them.
    * Opencyc has OWL serialization. Note however that Cyc is not a Semantic Web phenomenon but been under development since 1984.
* There also exists CycL-to-Lisp, CycL-to-C, etc. translators.
* It uses Google as the search engine in the background.

![](https://i.imgur.com/wEomxWf.png)

* **CycL** is Cyc’s **language** (tongue).
    * Bill Clinton belongs to the collection of U.S. presidents".
    ![](https://i.imgur.com/9UewLu0.png)
    * "All trees are plants".
    ![](https://i.imgur.com/Rsdk0dS.png)
    * "Paris is the capital of France".
    ![](https://i.imgur.com/8MWLb8h.png)
    * "a fact about sets"
    ![](https://i.imgur.com/jsqK8Ps.png)


### WordNet (1990)

![](https://i.imgur.com/7M6tcy2.png)

* Can canary sing? – pretty fast response.
* Can canary fly ? – a bit slower response.
* Does canary have skin? – a slow response.

![](https://i.imgur.com/vuyNzCW.png)

* WordNet Sub-Graph (English)

![](https://i.imgur.com/TmyRYGE.png)


### Generalized Upper Model (1994)

![](https://i.imgur.com/esJJfHp.png)


---

## Examples of Domain-specific Ontologies

### Ontology of GOD

![](https://i.imgur.com/R3t8weF.png)

### Unified Medical Language System (1993)

![](https://i.imgur.com/ZShbgCP.png)

### TOVE (1995) – Enterprise ontology

![](https://i.imgur.com/9XPdOLh.png)

---

## More Examples

* Traffic & mobility
    * DATEX II (https://datex2.eu/)
* Healthcare
    * Semantic DICOM (https://bioportal.bioontology.org/ontologies/SEDI)
    * Disease Ontology (http://disease-ontology.org/)
    * HL7 RDF (http://build.fhir.org/rdf)
* Music
    * The Music Ontology (http://musicontology.com/)
* Encyclopedic information
    * DBPedia (https://wiki.dbpedia.org/)
* Generic metadata
    * Dublin Core (http://dublincore.org/)