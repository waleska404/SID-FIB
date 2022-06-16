# Ontologies and Knowledge Representation

[//]: # (Poner aqui link al pdf/quizas no es muy legal colgar las transpas de otros)

###### tags: `SID-teo`

[ToC]

---

* In Distributed AI, ontologies are the basis of knowledge exchange.
* But are Ontologies a Knowledge Representation?
* Knowledge representation is a multidisciplinary subject that applies theories and techniques from three other fields:
    1. **Logic** provides the formal structure and rules of inference.
    2. **Ontology** defines the kinds of things that exist in the application domain.
    3. **Computation** supports the applications that distinguish knowledge representation from pure philosophy…

> […] Without logic, a knowledge representation is vague, with no criteria for determining whether statements are redundant or contradictory. Without ontology, the terms and symbols are ill-defined, confused, and confusing. And without computable models, the logic and ontology cannot be implemented in computer programs. Knowledge representation is the application of logic and ontology to the task of constructing computable models for some domain.
*(Sowa (2000), Knowledge Representation: Logical, Philosophical, and Computational Foundations, Brooks Cole Publishing Co., Pacific Grove, CA.)*


---

## The Role of Ontologies in Agent Communication

* Used by agents when trying to make sense of each other.
* Case of FIPA: Ontology is denoted by one parameter in an ACL message (along with other parameters: sender, receiver, content, reply-with, reply-by, in-replyto, envelope, language, protocol, and conversation-id).
* Example:
![](https://i.imgur.com/gZyePL8.png)
http://www.fipa.org/specs/fipa00061/
http://www.fipa.org/specs/fipa00037/
* Ontology is referenced from within an ACL message and it determines the semantics of the concepts used in the content language:
    * However, ontologies themselves might concern whatever topics.
    * One interesting case would be to ontologize agent communication.
    * For example interaction protocols (Conversation layer) might be described in an ontology external to the agents.
    * The agents could download the interaction protocol descriptions and modify their behaviour accordingly.
        * Ontology of actions or tasks vs. ontology of facts.
        * **Know-how** vs. **know-that**.

![](https://i.imgur.com/Z9iwGCo.png)
![](https://i.imgur.com/Sf76jhU.png)

---

## Some Ontology Tools

* Protégé (Ontology editor)
    * Lots of plugins: OKBC, RDF(S), OWL, UML, Prolog, Jess, OWL-S, etc. http://protege.stanford.edu/, http://protege.stanford.edu/plugins/owl/
* Jena
    * Java API for manipulating RDF, RDF(S), and OWL. http://www.hpl.hp.com/semweb/jena.htm, http://jena.sourceforge.net/
* Pellet
    * Open-source Java-based OWL DL reasoner. http://www.mindswap.org/2003/pellet/
* RDF Validator
    * For testing ontology code on RDF level: http://www.w3.org/RDF/Validator/
* Ontolingua
    * Collaborative environment to browse, create, edit, modify, and use ontologies. http://www.ksl.stanford.edu/software/ontolingua/

---