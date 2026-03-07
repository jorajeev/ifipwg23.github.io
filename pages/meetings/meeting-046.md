---
layout: page
title: "#46: Sydney, Jan 2007"
location: Sydney, Australia
date: 8–12 January 2007
parent: "Meetings 40–49"
grand_parent: Meetings
nav_order: 954
---

## Meeting 46

**Host:** Annabelle McIver  
**Location:** Sydney, Australia  
**Dates:** 8–12 January 2007

## Talks

- **Michael Butler**, *Refining reactive models to concurrent programs*
- **Carlos Gonzalia**
- **Ian Hayes**, *Iteration in real-time programs: finite, infinite, or either*
- **Joe Hurd**, *Mechanizing the Probabilistic Guarded Command Language*
  <details><summary>Abstract</summary>
  The probabilistic guarded-command language pGCL contains both demonic and probabilistic nondeterminism, which makes it suitable for reasoning about a wide range of algorithms. In this talk I'll present a mechanization of pGCL in the HOL theorem prover, which validates the theory and can be used as a platform for building software verification tools. I'll describe a verification condition generator used to verify the partial correctness of the probabilistic voting stage in Rabin's mutual-exclusion algorithm, as well as some more recent work looking at probabilistic termination.
  </details>
- **Gerwin Klein**, *Verifying an operating system kernel*
- **Shriram Krishnamurthi**, *Towards Reasonability Properties for Access Control Policy Languages*
- **Gary Leavens**, *Modular Verification of Higher-Order Methods in JML*
  <details><summary>Abstract</summary>
  We describe a simple, intuitive, and modular approach to specifying higher-order methods in JML. We also show how to verify code, using Hoare-style, first-order verification conditions, in a sound and modular way. Verification of client code that calls higher-order methods can take advantage of the client's knowledge about the mandatory calls to make strong conclusions. The verification technique validates and explains traditional documentation practice for higher-order methods, which typically shows their code. However, a JML specification does not have to expose all of its code to clients, but only enough to determine what mandatory calls the method makes and in what states those calls are made. Joint work with Steve M. Shaner and David A. Naumann.
  </details>
- **Rustan Leino**, *Automatic verification of summations*
- **Annabelle McIver**
- **Carroll Morgan**, *Schrodinger's Shadow: hidden probabilities; hidden nondeterminism*
  <details><summary>Abstract</summary>
  Annabelle McIver and I discovered some time ago that the "standard" model for sequential probabilistic/demonic programs has unusual difficulties with data refinement. The problem is that the usually automatic "hiding" of a module's internal state does not occur easily when probability is hiding from nondeterminism, or vice versa. We have used the "Shadow" model to abstract from modularised probability to just modularised nondeterminism (i.e. unquantified) and then see whether -- in that simpler context -- it would be more obvious what steps to take for data refinement. I will give an explanation of the Shadow model and discuss initial ideas for replacing nondeterminism by probability. Applications include security protocols such as Chaum's Dining Cryptographers and Rivest's Oblivious Transfer.
  </details>
- **Peter Müller**, *Alias Control with Universe Types -- Overview and Challenges*
  <details><summary>Abstract</summary>
  In object-oriented programs, an object can potentially reference any other object in the heap and read and modify its fields. Such programs with arbitrary object structures are difficult to understand, to maintain, and to reason about. In this talk, I will present the Universe type system, which allows programmers to organize the heap into ownership contexts and to control modification of objects. I will give an overview of the Universe type system and explain how it enables modular verification of object invariants. I will also propose a new solution to the ownership transfer problem.
  </details>
- **Shankar**, *Beyond Satisfiability*
- **Shankar**, *An overview of the Verified Software Roadmap*
- **Michel Sintzoff**, *Symbolic generation of optimal discrete control*
- **Ketil Stølen**, *Relating computer systems to sequence diagrams with underspecification, inherent nondeterminism and probabilistic choice*
  <details><summary>Abstract</summary>
  Having a specification and a computer system, we need to answer the question: Is the system compliant with the specification in the desired way? In this paper we present three techniques for answering this question when the specification is given as a sequence diagram. All techniques are independent of the choice of programming language used for the system. The three techniques correspond to three variations of sequence diagrams: sequence diagrams with underspecification, sequence diagrams with inherent nondeterminism and sequence diagrams with probabilistic choice. The semantics of sequence diagrams is given by denotational trace semantics. Joint work with Ragnhild Kobro Runde and Atle Refsdal.
  </details>
- **Mark Utting**, *Practical Model-Based Testing*
- **Ron van der Meyden**, *What, Indeed, is Intransitive Noninterference?*
  <details><summary>Abstract</summary>
  The notion of intransitive noninterference from the literature on computer security is intended to express architectural constraints on information flow. Roscoe and Goldsmith have argued that Rushby's definition of noninterference for intransitive security policies has weaknesses. A new, and more compelling, example will be presented to show that Rushby's definition admits information flows that are not in accordance with the intuitions it seeks to formalise. Several alternative definitions will be discussed, all of which are equivalent to the classical definition of noninterference with respect to transitive policies. Results will also be presented on the complexity of checking whether a finite state system satisfies these definitions of noninterference.
  </details>
- **Jim Woodcock**, *Trading assertions in the verified software repository*
  <details><summary>Abstract</summary>
  As part of the international grand challenge in verified software, the recent re-examination of the Mondex electronic purse has generated several thousand refinement verification conditions, which have been discharged amongst five different theorem provers. These assertions are to be curated in the verified software repository, and this raises the question of how such assertions can be traded between different theorem provers. One of the immediate problems is to resolve the different treatments of undefinedness. We present a unifying theory and use it to discuss how classical logic can be used to prove and to refute conjectures written in the different logics used in the Mondex experiment. Joint work with Mark Saaltink and Leonardo Freitas.
  </details>
- **Pamela Zave**
