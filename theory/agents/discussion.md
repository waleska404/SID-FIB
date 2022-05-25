# Discussion about Agents

[//]: # (Poner aqui link al pdf/quizas no es muy legal colgar las transpas de otros)

###### tags: `SID-teo`

[ToC]

---


##  Agents vs. Objects

* Are agents just objects by another name?
    * Object:
        * It encapsulates some state.
        * It communicates via message passing.
        * It has methods, corresponding to operations that may be performed on this state.
* Main differences:
    * Agents are **autonomous**:
        Agents embody stronger notion of autonomy than objects, and in particular, they decide for themselves whether or not to perform an action on request from another agent.
    * Agents are **smart**:
        Capable of flexible (reactive, pro-active, social) behavior, and the standard object model has nothing to say about such types of behavior.
    * Agents are **active**:
        A multi-agent system is inherently multi-threaded, in that each agent is assumed to have at least one thread of active control.
* As Wooldridge says:
    * Objects do it for free…
    * …agents do it because they “want”.
    * …agents do it for “money” (aka utility).


---

## Agents vs. Expert Systems

* Aren’t agents just expert systems with another name?
    * Expert systems are deliberative.
    * e.g. MYCIN.
* Main differences:
    * Agents **situated in an environment**:
        MYCIN is not aware of the world — only information obtained is by asking the user questions.
    * Agents **act**:
        MYCIN does not operate on patients.
* Some **real-time** (typically process control) expert systems **are** agents.

---

## Technological Challenges

* Implementing multi-agent systems is still a complex task.
    * Lack of maturity in both methodologies and programming tools.
    * Lack of specialized debugging tools.
    * Lack of skills needed to move from analysis and design to code.
    * Problems associated with awareness of the specifics of different agent platforms.
    * Problems in understanding the nature of what is a new and distinct approach to systems development.
* Increase quality of agent software to industrial standard.
    * Agent oriented design methodologies, tools and development environments.
    * Seamless integration with existing technologies.
        * Web, information systems.
    * Non-functional properties: scalability, performance, reliability, and robustness.
    * Analysis point of view:
        * Agent technology requires dedicated basic concepts and languages:
            * **Dynamic aspects**, such as time and action.
            * **Locality aspects**, such as position in a space.
