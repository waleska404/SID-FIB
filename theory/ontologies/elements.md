# Elements, Design & Development
[//]: # (Poner aqui link al pdf/quizas no es muy legal colgar las transpas de otros)

###### tags: `SID-teo`

[ToC]

---

## Elements

* **Concepts**: they serve to model several items including tasks, functions, actions, strategies, plans, etc.
    * Some ontology languages refer to them as **classes** composed by **properties**.
* **Relations**: they model a type of interaction between domain concepts.
* **Functions**: a special kind of relation.
* **Restrictions**: rules that may constrain the domain of values for some concepts and relations.
* **Instances**: constitute the concrete items/individuals represented by the ontology.
* **Axioms**:

![](https://i.imgur.com/4bOiTOt.png)

![](https://i.imgur.com/N2QMs8H.png)
* notese la flecha hacia arriba


---

## Design and Development

### Requirements

* To define the classes in the domain.
* To organize the classes in a taxonomic hierarchy.
* To define each class’ properties and include any restriction on their values.
* To assign values for each property to create instances.
* Note that: 
    * There is no single standard methodology to develop ontologies.
    * There is no single correct method to model a domain. Best solution depends on given application/domain.
    * The development process tends to be iterative.
    * The objects in the ontology should be close to the objects and relations used to describe the domain.
        * Usually they correspond to substantives and verbs which appear in sentences describing the domain.


### Phases in Ontology Development
In SOME methodologies the following 7 phases are present:

* **Phase 1: Determine the domain and coverage for the ontology.**
    * Which is the domain to be covered by the ontology?
    * What will we use the ontology for?
    * Which kind of questions the ontology should answer?
    * Who will use and maintain the ontology?
* **Phase 2: Consider to re-use existing ontologies.**
    * Ontologies are built to communicate Knowledge in a given domain. Therefore they are built to be shared.
    * It is unnecessary to re-do work already done by someone else: if there is already a (good) ontology for our domain we can use it.
* **Phase 3: Enumerate the important terms in the ontology.**
    * Write down a list of the terms useful to refer to our domain, by creating sentences we could use to ask things about it or to explain/describe the domain to others.
        * Which properties do these things/terms have?
        * What would we like to say about them?
* **Phase 4: Define the classes/concepts and their hierarchy.**
    * Several approaches:
        * **Top-down**: we define the most general concepts and then we refine them by a specialization process.
        * **Bottom-up**: we define the most specific concepts and then we group them according to common properties, in a generalization process.
        * **Bi-directional**: we define the most relevant concepts and then we generalize / specialize to complete the ontologyn.
    * None of these methods is the best one, **it depends on the domain** and the **target granularity** of our model.
* **Phase 5: Define the attributes and relations for each class.**
    * Should describe the internal structure of our classes.
    * Define a list of characteristics and to which class do they correspond.
    * We may have different property types:
        * Descriptive properties, e.g. quality
        * Identifying properties, e.g. names
        * Parts
        * Relations with other class instances
    * Properties should be assigned to the most general class, the subclasses will then inherit these properties.
* **Phase 6: Define the attributes’/relations’ characteristics.**
    * For attributes:
        * Cardinality (number of allowed values).
        * Type, value domains.
        * Default values.
        * Mandatory/optional.
    * For relations:
        * Cardinality.
        * Range.
* **Phase 7: Create instances (optional).**
    * If needed, create instances which will be part of the ontology at all times.


### Semantic Web Wedding Cake

![](https://i.imgur.com/QFf0Mfj.png)

### Ontology Development Principles

* **Clarity and Objectivity**.
    * An ontology must provide the user with the meaning of the term defined objectively and in a close-to natural language representation.
* **Completeness**.
    * The definitions must be expressed in terms of necessary and sufficient.
* **Consistency**.
    * To ensure (allow) the inferences derived from the ontology to be consistent with definitions.
* **Maximum monotone extensibility**.
    * New general or specialized terms can be included in the ontology in such a way that it does not require the revision of existing definitions.
* **Principle of ontological distinction**.
    * The classes in an ontology must be disjoint.
    :::warning
    :bulb: Disjunto: Que no tiene ningún elemento en común con otro conjunto.
    :::
* **Diversification**.
    * Diversification of the included hierarchies to increase the power of multiple inheritance mechanisms.
* **Modularity**.
    * To reduce the coupling between modules.
* **Name standardization**.
    * Standardization of names where possible.
* **Minimizing semantic distance**.
    * Minimizing the semantic distance between closely related concepts. Similar concepts will be grouped together and represented using the same primitives.


### Size and Scope of an Ontology

* Two extremes (the reality something in between):
    * One huge ontology (O) that captures *everything*.
    * One (small) ontology for each specific application (A).
    ![](https://i.imgur.com/xnNkRt9.png)
* **"One large ontology" approach**:
    * Benefits:
        * Few or no internal inconsistencies.
        * For an application developer easier to find.
        * Uniform documentation.
        * Less overlapping work!
    * Drawbacks:
        * Who maintains it?
        * Who is responsible?
        * Heavy and slow to use (both for human user and for application).
        * Difficult to take into account everybody's opinions and wishes at design time and when updating.
    * Example: Cyc
* **"Several small ontologies" approach**:
    * Benefits:
        * Ontologies fit well the application demands.
        * Faster to use.
        * Easier to form complete picture of an ontology (fewer concepts and interrelations).
    * Drawbacks:
        * Different ontologies do not fit together without either.
            * Central coordination body.
            * Ontology alignment software (M).
            * Coincidence.
        * Overlapping work - same concepts defined in multiple ontologies, either in the same way or (even worse!) differently.
* **Some mixed/other approaches**:
![](https://i.imgur.com/rgq9Wmm.png)


### Which of the approaches to use with agent systems (in the long run)?
* Agent-systems are typically distributed systems (agent-systems consisting of but one agent are rare and often not useful).
    * Agents typically need to communicate with each other.
    * Agents should understand each other.
* People often design and implement agents independently, unaware of the other developers.
* Agents' understanding each other is (partly) based on ontologies.

![](https://i.imgur.com/Pf9ysM7.png)


### Ontologies - Computer Science Specification of Conceptualizations

Example:
1. Properties of real world objects are identified.
2. Similarities are identified.
3. Concepts are created.
4. And are expressed as a class.
5. Classes are related.

![](https://i.imgur.com/oUjldAP.png)

* Example: The Water Cycle:
![](https://i.imgur.com/DaKv0Zw.jpg)
    * What exactly **is** the “lake”?
        * Is a lake a large body of water?
        * SDTS: Lake: “Any standing body of inland water”.
        * Or is it a (natural) basin that can hold a large amount of water?
        * Or is it a large area covered by water?
        * If the water goes away, is the lake dry, or does the lake cease to exist?
        * If the water rises, what is lake and what is flood?
        * As water flows through it, where does the lake begin and end?
    * What exactly **is** the “river”?
        * Is a river a large stream of water?
        * SDTS: Watercourse: “A way or course through which water may or does flow”.
        * If the water goes away, is the river dry, or does the river cease to exist?
        * If the water rises, what is river and what is flood?
        * Where does surface flow stop and river begin?
        * Where does river stop/start and lake start/stop.
        * How many streams is a braided stream?
    * Water expert:
    ![](https://i.imgur.com/jT4kDUl.png)
    * Two models: Wet vs Dry
        * “**Dry**” model is terrain features that *may* contain water.
        * “**Wet**” model is where water is currently flowing and standing.
        * Initial models are temporal snapshots.
        * Ignored erosional causation, groundwater leakance, etc.
        * Do not necessarily correspond directly to named or topographic features.
        ![](https://i.imgur.com/fVT5Bjp.png)
        ![](https://i.imgur.com/cubGspM.png)





### Some Advices on Ontology Development

* **Do not include singular and plural** versions of a word (the best policy is to only use names in singular or plural).
* **Names are not classes**. We must distinguish the class name which we give, we can have synonyms, but all represent the same class.
* Make sure that the **hierarchy is successfully built**.
* See **transitivity relations** and see if they are correct.
* **Avoid cycles** in the hierarchy.
* All subclasses of a class should be at the **same level of generality**.
* There is no criteria regarding the number of classes, experience is that a number between two and twelve, but you would suggest that we need to structure classes by adding more levels.
    * **When to introduce new classes?**
* Often uncomfortable to browse hierarchies or **too flat or very deep**, you should choose a midway point, some indications would be.
    * <u>New classes have additional properties that do not have the superclass.</u>
    * <u>They have different restrictions. Participate in different relations.</u>
* Decide if we have to use a **property or create a class**.
    * Sometimes an attribute is important enough to consider that its different values correspond to different objects.
* Decide **where is the level for instances**.
* Think what **minimum level of granularity** you need.
* **Limit the scope** of the ontology.
    * The ontology need not include every possible domain class, only the ones needed for the application being developed.
    * We also do not need to include all the attributes/restrictions/possible relationships.