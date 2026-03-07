---
layout: page
title: "#44: Niagara Falls, Jun 2005"
location: Niagara Falls, ON, Canada
date: 6–10 June 2005
parent: "Meetings 40–49"
grand_parent: Meetings
nav_order: 956
---

## Meeting 44

**Host:** Eric Hehner  
**Location:** Niagara Falls, ON, Canada  
**Dates:** 6–10 June 2005

## Talks

- **Ralph Back**, *Refinement diagrams and diagrammatic reasoning*
  <details><summary>Abstract</summary>
  I propose a mathematical framework based on lattice theory for describing and analysing large software systems: their construction, architecture and evolution. I propose a diagrammatic way of representing the software structure, and for reasoning about the correctness of the software. The diagrammatic reasoning is essentially equivalent to a Hilbert like proof in a small subtheory of lattices. We have been working on a software tool that shows this kind of diagrams with 3D rendering and browsing.
  </details>
- **Michael Butler**, *Refinement of an automatic refinement checker*
  <details><summary>Abstract</summary>
  Automatic refinement checking has recently been added to the ProB tool for B. Firstly, I will introduce the tool. Secondly, I will describe how a refinement approach (in B) is being used to prove the correctness of the refinement checker. This is joint work with Michael Leuschel.
  </details>
- **Ernie Cohen**, *Soliciting a verifier for a well-structured 40-KLOC C program*
- **John Harrison**, *Verifying the verifier*
  <details><summary>Abstract</summary>
  A complaint sometimes levelled against formal verification is that the theorem prover or model checker may be just as prone to bugs as the system being verified. A partial answer to this is to design the verification system around a small trusted core (e.g. in the "LCF" approach to building a theorem prover). A further step is to perform a verification of this core. I will report on a partial verification of the core of HOL Light (433 lines of OCaml) as well as discussing related work that I know about.
  </details>
- **Rick Hehner**, *Specification Blocks*
- **Tony Hoare**, *Retractions in process algebra*
  <details><summary>Abstract</summary>
  With Jifeng's help, I am hoping to discover how to embed an algebra like CSP within a less abstract one like CCS. I hope the proofs will be elegant too.
  </details>
- **Cliff Jones**, *Dynamically creating objects and sequencing operations: linking 2 approaches*
- **Yannis Kassios**, *Dynamic Frames*
  <details><summary>Abstract</summary>
  Two important features in object oriented refinement theories are (a) the encapsulation through the use of specification attributes (also known as model fields) and dependencies and (b) the support for pointers. It is known that the combination of these two features makes the frame problem hard to solve, because it introduces the possibility of abstract aliasing. In my work, I argue that a problem with existing approaches is that the possibility of abstract aliasing at a certain state is not expressible in their respective languages. I introduce the theory of dynamic frames, which allows such properties to be expressed. I show that dynamic frames address the frame problem without imposing any restriction to the programmer. Furthermore, I argue that object oriented specifications should be decoupled from classes and the more general concept of "theories" should be used instead. I show that dynamic frames can make the use of algebraic-like specifications possible in an environment that supports pointers. This is work in progress, part of a general theory of object oriented refinement for a PhD thesis.
  </details>
- **Shriram Krishnamurthi**, *On a conference submission/review manager*
- **Albert Lai**, *Operationalizing Predicative Programming: Eager and Lazy*
  <details><summary>Abstract</summary>
  We give an operational semantics for predicative programming; it is very general and includes both an eager fragment and a lazy fragment. The eager fragment of this semantics establishes soundness of refinements. We furthermore extend predicative programming to lazy imperative programming: stating and proving refinements of time bounds of lazy programs (without whole-program analysis!), the soundness of which is established by the lazy fragment of our operational semantics.
  </details>
- **Gary Leavens**, *Adapting Observational Purity to JML*
  <details><summary>Abstract</summary>
  The type system of the Java modeling language (JML) uses a notion of purity to prevent side effects in assertions. However, JML's notion of purity checking is too conservative. In particular, the equals method of Java's Object class must be declared pure, because this method needs to be used in the specification of various collection classes; however, some subclasses of Object, such as String, have side effects in their equals methods, and since purity is inherited, Object's equals method cannot be pure. We discuss semantical and language design issues involved in adapting recent work, in particular that of Barnett and Naumann, to solving this problem. Joint work with David Cok and David Naumann.
  </details>
- **Rustan Leino**, *Loop invariants on demand*
  <details><summary>Abstract</summary>
  I will talk about a technique for putting an abstract interpreter into a theorem prover, with the goal that the abstract interpreter will be invoked at times when the proof requires stronger loop invariants. This provides an opportunity to dynamically choose abstract domains to gradually increase the power and cost of the inference. It also provides an opportunity to dynamically perform trace partitioning, where the loop invariant inferred applies only to a subset of the program's executions. Joint work with Francesco Logozzo.
  </details>
- **Jay Misra**, *Orc: A Deterministic Distributed Programming Model*
  <details><summary>Abstract</summary>
  Orc is a new model of distributed programming which provides a strong theoretical foundation for internet computing based on compositions of web-services. Orc combines some of the power and flexibility of process algebra with the simplicity and determinism of synchronous programming models. We present an operational semantics of Orc and prove some laws analogous to those of Kleene algebra. We validate the deterministic operational semantics by proving it equivalent to a deterministic form of trace semantics.
  </details>
- **Jay Misra**, *Orchestration in Orc (with William Cook)*
- **Jay Misra**, *A Tree Semantics of an Orchestration Language (with Tony Hoare and Galen Menzel)*
- **Greg Nelson**, *The Straight-Line Automatic Programming Problem*
  <details><summary>Abstract</summary>
  In general, the automatic programming problem is the problem of constructing a program that meets a given specification. The Straight-Line Automatic Programming Problem is a special case in which the specification is a multi-assignment to be performed and the program to be constructed is restricted to a sequential composition of primitives that model machine instructions. I propose to define the problem precisely and then describe a reduction of the problem to problems for which we have practical solutions, namely SAT solving and E-graph matching.
  </details>
- **Alexander Petrenko**, *Unsolved solved problems*
  <details><summary>Abstract</summary>
  I am going to prepare a talk on real use of theory results in Computer Science/Software development. My point is as follows: one of the significant reasons of troubles in introduction of theory results in practice is moving of research focuses from solved (almost solved) problems to newest ones.
  </details>
- **Ralph Back**, *Teaching mathematics in high school*
- **Augusto Sampaio**, *Laws of Object-Oriented Programming*
  <details><summary>Abstract</summary>
  After introducing recent work with Paulo Borba, Ana Cavalcanti and Marcio Cornelio on a comprehensive set of laws for an object-oriented language similar to sequential Java, but with copy semantics, I would like to raise discussion on the following issues: laws that remain valid considering reference semantics; a data refinement law for class hierarchies; suitable semantic frameworks for proving these laws; and adequacy of the algebraic style as a basis for justifying larger grain transformations like refactorings and patterns.
  </details>
- **Shankar**, *Simplex in logical form*
- **Emil Sekerinski**, *Action-Based Object-Oriented Concurrent Programming*
  <details><summary>Abstract</summary>
  Lime is an experimental programming language that (1) separates class extension (subclassing) from class implementation (subtyping), (2) includes some specification and documentation constructs, and (3) allows objects to run concurrently by specifying actions in classes. After a brief introduction to the language and its implementation, I like to go into the particular model of concurrency and discuss the difficulties about the atomicity of actions and methods, both in the refinement rules and the current implementation.
  </details>
- **Michel Sintzoff**
- **Pamela Zave**, *Compositional Control of End-to-End Media in IP Networks: A Verification Case Study*
