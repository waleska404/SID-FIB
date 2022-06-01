# BDI: Belief, Desire, Intention

###### tags: `SID-teo`

* [Intentionality](#intentionality)
   * [Agent = Intentional System](#Agent-=Intentional-System)
   * [Intentional Attitudes](#intentional-attitudes)
* [Modalities](#modalities)
   * [Examples of unary modal operators](#examples-of-unary-modal-operators)
* [Modal Logic](#modal-logic)
   * [Semantics](#semantics)
   * [Basic Equivalences](#basic-equivalences)
   * [Properties](#properties)
   * [Epistemic Logic](#epistemic-logic)
   * [Systems in Modal Logics](#systems-in-modal-logics)
* [Knowledge vs Beliefs](#knowledge-vs-beliefs)
* [Intentions in Practical Reasoning](#intentions-in-practical-reasoning)
* [Agents and Actions](#agents-and-actions)
* [Logical Omniscience](#logical-omniscience)
   * [Logical Omniscience Problem](#logical-omniscience-problem)
* [Intentions - Beliefs - Desires]
   * [Intentions and Beliefs]
   * [Desires and Intentions]
* [BDI: A Logic Framework]
* [Mental States of an Agent]
   * [Agent Activity Diagram]
* [Beliefs about Competences]
* [Implementing BDI Agents]
   * [Agent Control Loop]
   * [Deliberation]
   * [Problems]
* [Glosary]

---

> One can define an agent’s solving problem mechanism in terms of its **beliefs**, how it proceeds to achieve its goals, its capabilities and relate its behaviour with its individual characteristics and attributes as its **preferences**. - *Haddadi96*

> The problem is that intentional notions --such as beliefs and desires-- are referentially opaque, in that they set up opaque contexts in which the standard substitution rules of first-order logic do not apply. In classical (propositional and first-order) logic, the denotation, or semantic value, of an expression is dependent solely on the denotation of its sub-expressions. For example, denotation of the propositional logic formula pq is a function of the truth-values of p and q. In contrast, the intentional notions are not truth functional. It is surely not the case that the truth-value of the sentence: “**Jaime believes p**” is dependent solely on the truth-value of p. - *Wooldrige, 1992*

* **Beliefs**: Are used to model the state of the world.
* **Desires**: Allow the selection of possible states of the world.
* **Intentions**: Are compromises to achieve a given state.

🢂 <u>BDI architectures</u> are aimed to model the rational or the intentional **agenciality**.

🢂 <u>Symbols</u> representing the world do correspond with **mental attitudes**.

---

## Intentionality

**Intentionality** is a property of many **mental states** and **events** which can then be mapped into **states of affairs**.

*Example:*
If I have a desire, this (desire) should be of doing something or willing that something happens (in the world) in a way.

**Beliefs** and **Desires** are intentional.


### Agent = Intentional System

**Intentionality** refers to the agent’s intentions as **rationally** implied by its beliefs (about the world). 

*Example*: 
If I assume that Agent i believes p,q,r… I assume that the agent believes all that it can be deduced from propositions p,q,r…

* **<u>Intentions</u>**:
    * Direct goal-based **reasoning**.
    * Constraint future **deliberation**.
    * Are **persistent**.
    * Are **beliefs** upon which pragmatic reasoning is built.



### Intentional Attitudes

Intentional Attitudes play different roles in the  Agent’s personality definition.
* **Cognitives** refer to epistemological aspects.
* **Volitives** refer to action and control. These denote an attempt to perform an action (conative).
* **Affectives** refer to the Agent’s dynamics



---
## Modalities

* **<u>Modality</u>**: operator that if applied to a formula produces a new formula with a new meaning.

*Example:*
`The operator  applied to the formula Ψ produces a new formula Ψ.`

* The only difference with the classic logic is that truth value of Ψ is only determined by the value of Ψ. 🢂 **Modalities do not maintain the truthiness.**

### Examples of unary modal operators

* Ψ --- Ψ is necessary. ⮞ Modal Logic
* ◊Ψ --- Ψ is possible. ⮞ Modal Logic
* ...............................................
* FΨ --- At some point in the future Ψ will be true. ⮞ Temporal Logic
* PΨ --- At some point in the past Ψ was true. ⮞ Temporal Logic
* ...............................................
* BiΨ --- Agent i believes Ψ. ⮞ Doxastic Logic
* KiΨ --- Agent i knows Ψ. ⮞ Doxastic Logic
* ...............................................
* OiΨ --- Agent i is obliged to Ψ. ⮞ Deontic Logic



---
## Modal Logic

* <u>**Modal Logic**</u>: The language to express the <u>semantics of a possible world</u>. Modal logic was developed to formalize expressions (arguments) that include **necessity** and **possibility**.
    * A <u>necessary proposition</u> is a truthful proposition that cannot be false. **Is true in all the possible worlds**.
    * A <u>possible proposition</u> is one that can be true. **At least is true in one world.**

* <u>**Syntax**</u>: the one of Classic Logic with the addition of two modal operators:
    *   necessity.
    *  ◊ possibility.

![](https://i.imgur.com/JC2MGeM.png)

* **<u>Semantic</u>**: defined as a model ==**M=<W,R,π>**==
    * **W** is a set of **possible worlds**.
    * **R** is a binary function, called **accessibility function**.
    * **π** is an **assignation function** that determines for each w∈W, the true values of the propositions in W.

> It can be seen as a graph (W, R) with a true value assignation function  that indicates which propositional functions are true and in which node.[color=#37B9BF]



* All **<u>valid formulas</u>** are interpreted according to a pair **<M,w>** using the satisfaction function **(M ⊨ p)**.
    * A formula is ==**<u>satisfactible</u>**== if it is satisfied in at least one pair model/world.
    * A formula is ==**<u>true</u>**== if satisfactible in each of the worlds of the model.
    * A formula is ==**<u>valid</u>**== if it is true in each of the model/world pairs.


### Semantics

![](https://i.imgur.com/aJOrYxP.png)

### Basic Equivalences

![](https://i.imgur.com/nSfRHBi.png)

### Properties

![](https://i.imgur.com/pcIYQTg.png)

### Epistemic Logic

:::warning
**Lógica epistémica**: campo de la lógica modal que se ocupa del razonamiento sobre el conocimiento. 

**Axioma**: principio indemostrables sobre los que, por medio de un razonamiento deductivo, se construye una teoría.
:::


* **K:** An agent’s knowledge is closed under implication, that is an agent knows all consequences of its **valid beliefs**.
* **T:** It says that if an agent knows facts, the facts must be true. This has often been taken as the major distinguishing feature between knowledge and belief. While you can believe something that is false, **you cannot know something that is false.**
* **D:** An agent’s valid **beliefs are not contradictory.**
* **4:** The **Positive Introspection Axiom** says that agents know what they do know.
* **5:** The **Negative Introspection Axiom** says that agents know what they do not know.
* **NEC:** The necessity rule establishes that an agent knows every valid formula and in consequence all tautologies.


### Systems in Modal Logics

* Usual attributes of **knowledge** and **beliefs** are referred to **truthness** (the truth of knowledge, the consistency of beliefs) and **introspection**.
    * T = NKT
    * S4 = NKT4
    * S5 = NKT5
    * S5+ = KD45


![](https://i.imgur.com/fsD221N.png)
![](https://i.imgur.com/4frndE6.png)


* The K System:


![](https://i.imgur.com/JtUu48x.png)





---
## Knowledge vs Beliefs

**Knowledge** can be distinguished from **beliefs** considering that <u>knowledge is a belief that is true</u>:
![](https://i.imgur.com/eNXMLM7.png)

* K~i~ φ denotates that “an agent i knows φ”



---
## Intentions in Practical Reasoning

1. Intentions pose problems for agents, who need to determine ways of achieving them.
    * If I have an intention to Φ, you would expect me to devote resources to deciding how to bring about Φ.
2. Intentions provide a filter for adopting other intentions, which  must not conflict.
    * If I have an intention to Φ, you would not expect me to adopt an intention Ψ such that Φ and Ψ are mutually exclusive.
3. Agents track the success of their intentions, and are inclined to try again if their attempts fail.
    * If an agent’s first attempt to achieve Φ fails, then all other things being equal, it will try an alternative plan to achieve Φ.


---
## Agents and Actions

* What it means that an agent can do action a?
* What it means that an agent has the **ability** to do action a?
    * **Control**: The action a should be in the control of A~i~ or the truth of φ should be under A~i~'s control.
    * **Repeatability**: A~i~ should be able to repeatedly do action a or repeatedly bring about formula φ.
    * **Avoidability**: A~i~ should be able to avoid doing action a.
    * **Free-will**: A~i~ should be free to decide whether or not to do action a.
    * **Causality**: A~i~ should cause action a to take place or the formula φ to become true.
    * **Intentionality**: A~i~ should intentionally do action a or bring about φ.
* Do(a) “The Agent does a”.
    * K --- Do(a⇨b) ⇨ (Do(a) ⇨ Do(b))
     T --- Do(a) ⇨ a
     Nec --- if ⊨ a then ⊨ Do(a) 
     (⊨ : entails)
    * T says “if the Agent does a then a is the case”.
* The Agent can achieve  in a situation s.
    * Result(s, a) = s’ (the result of executing action a in situation s is situation s´).
    * Can(s, φ) := ∃a (Result (s,a) satisfies φ).
* What does it mean for an Agent to know how a plan will achieve its goal?
    * If K(s, φ) is true.
    * If ∃a : K(Result (s,a), Can(Result (s,a) φ)).



---
## Logical Omniscience

The necessity rule and the Knowledge axiom together imply that agent <u>**believes** all the valid formulas</u> and that it <u>**knows** all the logical consequences of its valid beliefs</u>.

* **Logical consistency**: an agent cannot believe that φ and ψ at the same time if φ ⇒ ¬ψ.
* **Logical equivalence**: given two propositions: if ψ is true then i) and ii) are logically equivalent.
    * i) φ 
    * ii) φ∧ψ

### Logical Omniscience Problem

* If epistemic logic is to be interpreted as describing actual **knowledge** of realistic (though idealized) agents, then the discussed closure properties require agents to be very powerful reasoners whose computational capacities cannot be achieved by real (human or artificial) agents, who are simply not logically omniscient.
* **Logical omniscience poses a problem because it contradicts the fact that agents are limited in their reasoning powers.** They are inherently resource bounded and therefore cannot handle an unlimited amount of information. Agents may establish immediately certain logical truths or simple consequences of what they consciously assented to.
* However, there are highly remote dispositional states which could only be established by complex, time-consuming reasoning. The modal framework cannot distinguish between a sentence that an agent consciously assented to and a piece of potential knowledge which could never be made actual by the agent and is therefore not suited to model resource-bounded reasoning.




---
## Intentions - Beliefs - Desires

### Intentions and Beliefs

* **Consistency intentions-beliefs**
    * An agent ought to believe that its objectives are possible.
    * An agent cannot believe that it will not reach its objectives.
* **Incompleteness intentions-beliefs**
    * Intentions should be consistent with beliefs but not necessarily to support them.
    * It is possible to have incomplete beliefs about the own intentions.
* **Side-effect Problem**
    * An agent that tries to do a and believes that doing a requires doing b does not have to have the intention of making b.


### Desires and Intentions

* **Internal Consistency**
    * An agents should avoid to have intentions in conflict but it may have conflicting desires.
* **Means-end Analysis**
    * Intentions may create problems for future deliberations, desires not necessarily.
* **Keep memory of successes and failures (of intentions)**
    *  To keep the compromise with a given action; There is no compromise associated to a desire. **==Intentions are desires + compromises to act.==**
* **Consistency with beliefs**
    * Intentions ought to be consistent with the beliefs but not necessarily with the desires.

---
## BDI: A Logic Framework

* The formulation language is FOL, multimodal with equality.
    * Standard FOL operators + **Happens, Done, BEL**, and **GOAL**.
    * The semantics of **BEL**, and **GOAL** is given by their accessibility relations to the possible worlds.
* The world is defined as sequence of discrete events that extends infinitely towards the past and future.
    * **Happens** defines a sequence of events that will occur.
    * **Done** defines a sequence of events that already happen.
    * **e;e’** (e followed by e’).
    * **e|e’** (e or e’).
    * **e?** ( test) **e*** (iteration).
* The temporal operators are: **□ (always), ◊ (sometimes)**, **LATER**, y **BEFORE**. Those symbols should not be identified with the necessity and possibility.
* It is assumed that agents have only a restricted set of accessibility relations. This is known as **realism constraint**. This avoids that agents choose worlds that are outside of their beliefs.
* If an agent believes that  is true (now), it cannot desire it become false (now), an agent cannot chose what it cannot modify.
    ⊨ (BEL~x~ φ) ⇨ ¬ (GOAL~x~ φ) 
* An agent assumes that all its goals are false (not achieved) to possible satisfy them.
     (A_GOAL~x~ φ) = (GOAL~x~(LATER φ)) ∧ (BELx ¬φ)
     
     
     
     
     
---
## Mental States of an Agent

* **Beliefs** represent some knowledge about other agents. Agent a~1~ believes φ about a~2~.
    BEL~a1~ (DO~a2~ φ)
* **Capacities** correspond to the abilities to act.
* **Goals** are generated by the evaluation of other agent’s messages and/or correspond to the agent’s aims.
    * A goal assigned by another agent is a **mission**.
    * An agent remembers all assigned goals:
        * MIS a~1~ a~2~ φ
            G~a~ φ = MIS a,a φ
* **Intentions** correspond to the decision made when adopting a **goal**. An agent only adopts goals that he knows he can achieve.
    * Intention: Is the will to accomplish a desire or to perform an action.
    * ![](https://i.imgur.com/ADQ92lh.png)
    * An intention is **fulfilled** by the **actions** oriented to achieve a **goal**.



### Agent Activity Diagram

![](https://i.imgur.com/vOliLRw.png)


---
## Beliefs about Competences

Who can do what?
↳ By task delegation.
↳ By collaboration.

![](https://i.imgur.com/izWhGih.png)

* Introspective view:
    * Bel(a, (Bel (a, Bel (a, Bel( .... Bel(a,a))...)
* Own model:
    ![](https://i.imgur.com/3HMr1qI.png)

---
## Implementing BDI Agents

### Agent Control Loop

This is the abstract algorithm for the BDI reasoning cycle:
![](https://i.imgur.com/Bc37shB.png)

### Deliberation

* How does an agent deliberate?
    * Begin by trying to understand what the options available to you are.
    * Choose between them, and commit to some.
* Chosen options are then intentions.
* Deliberation can be decomposed into two distinct  functional components:
    * **Option generation**
        In which the agent generates a set of possible alternatives; Represent option generation via a function, options, which takes the agent’s current beliefs and current intentions, and from them determines a set of options (= **desires**).
    * **Filtering**
        in which the agent chooses between competing alternatives, and commits to achieving them. In order to select between competing options, an agent uses a **filter** function.
        

### Problems

* **Overcommitment**
    * An agent has commitment both to **ends** (i.e., the wishes to bring about), and **means** (i.e., the mechanism via which the agent wishes to achieve  the state of affairs).
    * Our agent control loop is overcommitted, both to means and ends.
    * Solution: 
        * **Replan** if ever a plan goes wrong.
        * **Reconsider the intentions** every now and then, to check if they are still achievable.
* **A dilemma on intention reconsideration:**
    * An agent that does not stop to reconsider its intentions sufficiently  often will continue attempting to achieve its intentions even after it is  clear that they cannot be achieved, or that there is no longer any reason  for achieving them.
    * An agent that constantly reconsiders its attentions may spend insufficient time actually working to achieve them, and hence runs the risk of never actually achieving them.
    * Solution: incorporate an explicit **meta-level control** component, that decides whether or not to reconsider.

![](https://i.imgur.com/DwpBSEO.png)

---
## Glosary

* **Competences**: A specific range of skill, knowledge, or ability.
* **Deontic logic**: is the field of logic that is concerned with obligation, permission, and related concepts.
* **Doxastic logic**: is a modal logic that is concerned with reasoning about beliefs.
* **Intuitionistic logic**: The system preserves **justification**, rather than **truth**, across transformations yielding derived propositions. From a practical point of view, there is also a strong motivation for using intuitionistic logic, since it has the existence property, making it also suitable for other forms of mathematical constructivism.
* **Stance**: intellectual or emotional attitude.
* **Volition**: the capability of conscious choice and decision and intention.
