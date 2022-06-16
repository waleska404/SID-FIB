# Formal Foundations and Languages

[//]: # (Poner aqui link al pdf/quizas no es muy legal colgar las transpas de otros)

###### tags: `SID-teo`

[ToC]

---

## Formal Foundations

### Mereology

:::warning
:bulb: En filosofía, la **mereología** es el estudio de las relaciones entre partes, tanto de las partes con el todo, como de las partes con otras partes.
:::

* **Mereology** is a collection of axiomatic first-order theories dealing with parts and their respective wholes.
* Its core notion is **meronomic**, which means based on part–whole relationships.
* It has been the formal basis of ontologies since Plato until beginning of 20th century.
* The creator of mereology: polish logician and mathematician Stanisław Lesniewski (1886-1939).
* **Ground mereology**: parthood is a reflexive partial order.
    * x is_a part_of x (**irreflexivity** - nothing is a part of itself).
    * If x is_a part_of y and y is_a part_of x then x=y.
    * If x is_a part_of y then y is_not_a part_of x (**asymmetry**).
    * If x is_a part_of y and y is_a part_of z then x is_a part_of z.(**transitivity**)

There are two basic definitions - of mereological sum and mereological fusion. Suppose that we have some set Z of objects.
* An object x is a **mereological sum** of all elements of Z iff every element of Z is an ingrediens of x and every ingrediens of x overlaps some element z from Z.
* An object x is a **fusion** of all elements of Z iff for every object y, y overlaps x iff y overlaps some element z from Z. 
* x is **proper part** of y: x is part of y and y is not part of x.
* x **overlaps** y: there is a part of x that is also a part of y.
* x and y are **disjoint**: x and y do not overlap.
* **Binary Product:** x . y: individual that is part of both x and y and any common part of x and y is a part of the product.
* **Binary Sum:** x + y: individual that overlaps something iff it overlaps at least x or y.
* **Difference:** x – y: largest individual contained in x that has no part in common with y.


### member-of ≠ instance-of

==In other words, set ≠ class.==
A set which does not have its **intensional description** cannot be a class.

*Examples:*
* {car, 3, set, sushi} is not a concept, and hence not a class.
* {human-1, human-2, …(all humans)} can have two interpretations:
    * A **class** Human when human-i is interpreted as an instance of Human.
    * An **instance** of a class “human-set” whose members are human-i.
* {tree-1, tree-2, …, tree-n} → a forest(*member-of*).
* {tree-1, tree-2, …, tree-i, …(all trees)} → a class Tree(*instance-of*).

**The ontological definition of a class and instance**
A thing which is a conceptualization of a set X can be a class if and only if each element x of X belongs to the class X if and only if the “**intrinsic property**” of x satisfies the intensional condition of X. And, then and only then, `<x instance-of X>` holds.


**Is-a vs. part-of**
The major difference between is-a and part-of: when making an instance of a class:
* **is-a case**: Only one instance of one of the subclasses are generated.
* **part-of case**: Instances from each of its subclasses are generated.

![](https://i.imgur.com/TU8af9p.png)


Cat part-of mammal? dog part-of mammal? If we interpret them as **species**, it is correct.

### Description Logics

* Need to find a computable representation.
* First Order Logic (FOL) is too expressive and computationally expensive.
* Description Logics is a valid option:
    * It allows to reason about classes, subclasses, instances and definitions.
    * Is a restriction from FOL based on **Set Theory**.
    * Is also the foundation of Object Oriented formal semantics.
    * There are efficient algorithms based on **analytic tableaux**.
* FOL + new operators and symbols:
    ![](https://i.imgur.com/ZSwk9yH.png)
* Distinction between two kinds of predicates:
    * Concepts (*C*).
    * Relations (*R*).
* Quantified formulae are rewritten:
![](https://i.imgur.com/qZYd9Wf.png)


---

## Languages

* Need to express ontologies in a machine-computable language (usable by computational entities in their messages and in their reasoning).
    * A language simple enough to make ontology development easier.
    * A language with formal semantics.
        * Formal semantics are needed in order to obtain deductions from the information in the ontology.
    * A language allowing agents and other intelligent systems to reason with it.
    * The computational cost should be reasonable.


### Advantages of Ontologies

* **Formal Community View**
    Make it possible to formalise a shared viewpoint over a certain universe of discourse e.g., agreement on how to model time.
* **Interoperability**
    Can support communication and cooperation between systems developed at different sites. The ontological commitments made by a system are made explicit e.g., diagnostic and therapy-control medical systems may share the same underlying generic medical ontology e.g., notion of pathological state, therapeutic procedure.
* **Model-based knowledge acquisition**
    Use the medical guideline ontology to acquire knowledge about particular medical guidelines in a structured way
* **Knowledge-level validation and verification**
    Use the medical guideline ontology to check guideline documents.
    

### KIF: Knowledge Interchange Format

* Developed at Stanford University (1992).
* Idea: to have an exchange format between applications, independent from their internal representations.
* Based in First Order Logic (FOL): Prefix notation + definitions.
* Semantics: Description Logics (Definitions + needed conditions).
* KIF has FOL’s operators:
    * **Boolean** values: `true`, `false`.
    * **Connectives:**
        * `and`, `or`, `not`,
        * `=>` (if) `<=` (only if), `<=>` (definition).
    * **Quantifiers:** `forall`, `exists`.
    * **Vars:** `?x` (individual var) `@x` (var group, as in PROLOG).
    * ***Example:*** `(forall (?x)(> ?x 3))`.
* **Lists** can be built and used as basic data types (as LISP)
![](https://i.imgur.com/raBFaug.png)
* **Functions** can be defined.
![](https://i.imgur.com/j92fryT.png)
* **Relations** can also be defined.
![](https://i.imgur.com/TbYnKxL.png)
* **Metaknowledge** expressions.
![](https://i.imgur.com/hf5tJT6.png)
* **KIF example: Class person:**
![](https://i.imgur.com/Nwl9XQ1.png)

    
---


## Markup Languages

### XML
* Idea of a **Semantic Web**: Information semantically annotated in a machineparseable language.
* HTML is not enough: Language oriented to presentation.
* Idea: to use XML (derived from SGML).
* Advantages:
    * Allows to describe **attributes** in information.
    * Already used by industrial initiatives.
    * Allows integration from different data sources (by means of **XSLT translation rules**).
    * Non-proprietary language.
* An XML document can contain **Data Type Definitions** inside or can refer to a DTD file.
* One can create repositories of reusable definitions (**namespaces**):
* *Example:*
![](https://i.imgur.com/dyH8Z6j.png)


### From XML to DAML+OIL
* **Problems**:
    * XML is too rigid (tree-like structures).
    * Difficult to include relationships to the structures defined.
    * Difficult to assert predicates.
* **Extension: RDF + RDFS**
    * RDF allows to assert statements.
    * RDFS declares classes, attributes and relations.
    * RDFS definitions can be instantiated.
* **Even more powerful extension: DAML+OIL**
    * DARPA agent markup language.
    * Ontology Inference Layer.
* *DAML+OIL Example*
![](https://i.imgur.com/sUhyVjj.png)
![](https://i.imgur.com/Hjc6wRv.png)


### OWL

* Further extension: OWL (Ontology Web Language)
    * Fusion of DAML+OIL, standard of W3C.
    * Has also become standard de-facto for most of Semantic Web applications and Semantic Web Services.
    * 3 levels:
        * OWL lite: defines taxonomies and simple restrictions.
        * OWL DL: provides expressiveness as Description Logic.
        * OWL full: maximum expressiveness (but not available reasoners). 
    * Specification available at http://www.w3.org/TR/2004/REC-owl-features-20040210/#s2.1
    * There is a new specification being defined, OWL 2 (Oct 09).
* There is yet another extension, called OWL-S, used for Web services and the Semantic Web.
* Characteristics:
    * It integrates all elements in DAML+OIL, creating a new namespace: `owl`.
        * All properties that DAML+OIL indlude have been integrated into the `owl` namespace.
        * Sintax is extended to specify **instances**, and a new tag, `owl:Thing`, is added (all instances belong to `owl:Thing`).
        * It allows the definition of all the primitive types included in the XML Schema Datatypes by using the `xsd` namespace.
    * OWL adds new restrictions to classes, properties and individuals:
        * `owl:allValuesFrom`: the property values should belong to certain class.
        * `owl:equivalentClass`, `owl:equivalentProperty`: Equivalence between classes and properties.
        * `owl:sameAs`, `owl:differentFrom`: equal/different Individuals.
        * `owl:SymmetricProperty`: a symmetric property to another one.


---

## Public Ontology Repositories

* http://www.daml.org/ontologies/
    * 282 public Ontologies written in DAML+OIL/OWL
    * Wide variety of topics:
        * academic department, Actors, address book, airport, Bibliography, Biology, Chemistry, Clothing, Weather
        * As 2004
* http://protegewiki.stanford.edu/index.php/Protege_Ontology_Library
    * Is not a repository, but a list to some interesting ontologies (mostly OWL)
    * As 2018

---