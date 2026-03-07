---
layout: page
title: "#43: Prato, Sep 2004"
location: Prato, Italy
date: 6–10 September 2004
parent: "Meetings 40–49"
grand_parent: Meetings
nav_order: 957
---

## Meeting 43

**Host:** Bertrand Meyer  
**Location:** Prato, Italy  
**Dates:** 6–10 September 2004

## Talks

- **Cliff Jones**, *Beyond "Verifying Compiler"*
  <details><summary>Abstract</summary>
  One conclusion: The "Verifying Compiler" should not be concerned with verifying the absence of bugs, but help with the design of software.
  </details>
- **Cliff Jones, Tony Hoare, and Brian Randell**, *Extending the horizons of DSE*
- **Gary Leavens**, *Alias-Free Formal Parameters*
  <details><summary>Abstract</summary>
  Aliasing among formal parameters, and among formals and globals, causes problems for both optimization and reasoning; such aliases are a source of subtle errors in programs. Whole-program static analysis could provide knowledge about such aliasing, but it is non-modular, expensive, and conservative. I will describe a small extension to Java and JML that leads to significantly better optimization opportunities for a compiler and allows modular reasoning. The extension allows aliasing among arguments and globals at the call site, but guarantees there will be no overlap among arguments and globals inside method bodies, and also allows methods to have specifications that "work" for overlapping arguments. This is done by having multiple bodies for each procedure, up to one for each aliasing pattern. Procedure calls are automatically dispatched to the body that matches the run-time aliasing pattern among the actual parameters and the globals. Joint work with Medhat Assaad and Olga Antropova.
  </details>
- **Peter Müller**, *Modular verification of object and module invariants*
  <details><summary>Abstract</summary>
  Joint work with Rustan Leino. The talk describes a methodology for specifying and verifying object-oriented programs, using object invariants to specify the consistency of data and using ownership to organize objects into dynamic contexts. Object invariants can describe a large variety of properties, including properties of cyclic data structures. The methodology is designed to allow modular reasoning, even in the presence of subclasses and callbacks. Module invariants describe properties of variables that are shared by several objects. I would like to discuss how the presented methodology for object invariants can be adapted to cover module invariants.
  </details>
- **Bertrand Meyer**, *The Dependent Delegate Dilemma*
- **Pamela Zave**, *A formal model of addressing for interoperating networks*
- **Annabelle McIver**, *Optimal strategies for two-player parity games*
  <details><summary>Abstract</summary>
  In this talk I will discuss the problem of finding optimal strategies for two-player games. Game models of programs can be useful in the specification and analysis of temporal-style properties. In such models players compete to optimise some specified reward function. It has recently been proved that in the stochastic parity-game setting optimal memoryless strategies exist for each player. Unfortunately determining those optimal memoryless strategies can be problematic. I will show how optimal memoryless strategies can be computed reasonably simply, provided that non-pure strategies are an acceptable solution.
  </details>
- **Michael Jackson**, *The problem of the banker with 52 cards*
  <details><summary>Abstract</summary>
  A "banker" has an ordinary 52-card deck of cards. You have some positive amount of money. The banker decides on the order of the cards. Before the banker turns each card over, you place a bet. You put some proportion of your money on "red" and the rest on "black". After the banker turns over the card, you lose the money you bet on the losing color, and double the money you put on the winning color. Design a strategy that maximizes your guaranteed gain, and prove this strategy correct.
  </details>
- **Ian Hayes**, *Finding Faults*
  <details><summary>Abstract</summary>
  Examining systematic methods for detecting faults in components, including timing faults.
  </details>
- **Michael Butler**, *Semantics and atomicity for long-running transactions*
  <details><summary>Abstract</summary>
  Long-running transactions lack the atomicity of ACID transactions. Instead of rollbacks and checkpoints, compensation is used to recover from error. The development of a trace semantics has lead to a structured design for a language of long-running transactions and also to a rational basis for the use of compensation in which a degree of atomicity can be recovered.
  </details>
- **Cliff Jones**, *Towards a development method, "Splitting atoms safely"*
  <details><summary>Abstract</summary>
  Wanted: a method that provides the fiction of atomicity. Can atomicity be used in program design? Wants atomicity refinement, especially in combination with data refinement.
  </details>
- **Mark Utting**, *Model-Based Testing*
  <details><summary>Abstract</summary>
  In this talk, I will describe the problems of generating good test suites from formal specifications (pre/post style). The goal is to build a practical tool (the LTG -- Leirios Test Generator) that engineers can use to semi-automatically generate tests from B, Z, JML, UML or Statechart specifications.
  </details>
- **Bertrand Meyer**, *The mathematics of object computation*
- **Jean-Raymond Abrial**, *Developing discrete transition systems*
  <details><summary>Abstract</summary>
  (1) Refinement of Stuttering steps: skip or keep (or both). Stuttering steps are usually considered to be refinement of skip. In certain cases, it is interesting however to think of them as being a refinement of (a sort of) keep. (2) Temporal Statements and Refinements. It is claimed that it is possible to completely avoid certain temporal logic statements and replace them by refinements of stuttering steps. This raises the problem of characterizing systems which run forever.
  </details>
- **Carroll Morgan**, *Compositionality and "pCSP"*
  <details><summary>Abstract</summary>
  Compositional semantics for probabilistic process algebras have been studied for decades: one of the major problems is the interaction of the various forms of choice: probabilistic, internal, external (to use CSP terminology). Work with Annabelle on sequential semantics for probability and demonic choice has given a logic which is discriminating enough in its observations to reconstruct the operational (but sequential) program that led to the observations. Related issues turn out to be information hiding and simulation.
  </details>
- **Werner Dietl**, *Object Ownership -- Overview and Issues*
  <details><summary>Abstract</summary>
  I will motivate object ownership and show three concrete systems that enforce it -- two type systems and one dynamic solution. There should be multiple possible discussion topics, from the basic motivation and possible applications down to technical problems.
  </details>
- **Alexander Petrenko**, *Specification Based Testing (SBT): A Practical Concern*
  <details><summary>Abstract</summary>
  The talk will discuss different issues related to SBT technology development and application, involving case studies for KVEST, UniTesK and OTK technologies developed and applied in several projects for Nortel Networks, Microsoft, Intel and other customers. Main points include: KVEST and UniTesK technologies for test generation from contract specifications; roles of models in test suite generation and multiparadigm specifications in real life applications; and highest priorities of SBT introduction in practice.
  </details>
- **Rustan Leino**, *On bounded model checking, induction, and interpolants*
  <details><summary>Abstract</summary>
  Many interesting state-based computer systems -- both software programs and hardware circuits -- can be represented as transition systems. An execution of a transition system begins in some initial state and then repeatedly applies a transition relation to obtain the next state. An important question for such a system is whether or not it is possible for the system to reach some given set of "bad" states. In this discussion, I consider ways to determine such reachability, trying to uniformly present previous attempts.
  </details>
- **Bertrand Meyer**, *"Test Studio" from Eiffel Software / ETH*
