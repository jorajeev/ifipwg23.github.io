---
layout: page
title: "#42: Philadelphia, Jan 2004"
location: Philadelphia, PA, USA
date: 5–9 January 2004
parent: "Meetings 40–49"
grand_parent: Meetings
nav_order: 958
---

## Meeting 42

**Host:** Ernie Cohen  
**Location:** Philadelphia, PA, USA  
**Dates:** 5–9 January 2004

## Talks

- **Rajeev Alur**, *Software synthesis from hybrid automata*
- **Manfred Broy**, *Services and features: specification and multi-view modeling of software systems*
- **Michael Butler**, *Modelling and reasoning about long-running business transactions*
  <details><summary>Abstract</summary>
  We recently collaborated with a group at IBM UK Labs on formalizing compensation mechanisms in long-running transactions. An outcome of this collaboration was a formal modeling language called StAC (Structured Activity Compensation). This language is similar to process algebraic languages such as Hoare's CSP or Milner's CCS but StAC has additional operators dealing with compensation and with early termination of processes. Compensation and termination are also found in languages such as XLANG, BPEL4WS and BPML. I propose to give an overview of the StAC language, its semantics and its relationship with BPEL4WS. I also propose to discuss some ideas on reasoning about StAC processes. This work is joint work with Carla Ferreira.
  </details>
- **Ernie Cohen**, *The NGSCB Nexus*
  <details><summary>Abstract</summary>
  The goal of Microsoft's NGSCB project is to turn the PC into a trustworthy computing platform. The heart of NGSCB is the (inner) nexus, a small exokernel that allows a number of concurrently executing, mutually distrustful supervisor-mode components to safely share hardware resources. I'll describe the nexus and how we're assuring its correctness.
  </details>
- **Masami Hagiya**, *UML Scrapbook and Realization of Snapshot Programming Environment*
  <details><summary>Abstract</summary>
  Joint work with Richard Potter et al. We have developed SBUML (Scrapbook for UML), an extension of UML (User-Mode Linux), by adding the checkpointing functionality to UML. In this paper, we first describe the design and implementation of SBUML, and then propose a new snapshot programming environment, which is realized by the SBUML programming interfaces. The intended applications of SBUML include intrusion detection and sandboxing for network security, and software model checking for verifying multi-threaded programs. In particular, using snapshot programming, one can easily enumerate state spaces of programs actually running under Linux.
  </details>
- **John Harrison**, *Formal verification of mathematical algorithms*
- **Daniel Jackson**, *Subtypes for specification*
  <details><summary>Abstract</summary>
  We've developed a new type system for Alloy that incorporates subtypes, ad hoc union types, and parametric polymorphism in a surprisingly simple way. Type errors correspond to expressions that are redundant, in the sense that their value doesn't affect the value of the formula as a whole. Using subtypes, we can also decompose formulas for more efficient analysis.
  </details>
- **Michael Jackson**
- **Gary T. Leavens**, *Advances and Issues in JML*
  <details><summary>Abstract</summary>
  The Java Modeling Language (JML) is a behavioral interface specification language tailored to Java. Its goals are to help record detailed design decisions about Java classes and interfaces and to support a wide range of tools that help programmers. JML combines features of Eiffel, the Larch family of interface specification languages, and the refinement calculus. JML is an open project that is intended to foster some commonality among the specification notations used by various groups doing research on formal methods for Java programs. This talk briefly describes some advances that JML's design has made over these other specification languages. It then focuses on problems and issues remaining in its design. In particular it describes the following advances and issues related to them: purity checking to prevent side effects in assertions, and protected and private specifications. This talk is based in part on joint work with Curt Clifton, Clyde Ruby, and others at Iowa State, and also with Rustan Leino, Erik Poll, Bart Jacobs, Michael Ernst, and others.
  </details>
- **K. Rustan M. Leino**, *Abstract interpretation for heap structures*
  <details><summary>Abstract</summary>
  Many abstract domains are defined over a program state space whose form is a Cartesian product of variables, that is, where each variable is an independent coordinate. A particular abstract domain may keep track of a relation between some variables, say those variables with integer values, and ignore the others. For an object-oriented program, one can think of the heap as one big variable: a two-dimensional matrix indexed by object identities and field names. For the heap variable, one would like to relate the values at certain locations (object-field pairs) with each other and with other program variables, which independent-coordinate abstract domains don't immediately do. I will present the preliminary design of a system for doing abstract interpretation over a program state space that includes such a heap variable. The design is parameterized by any independent-coordinate abstract domain. It automatically maintains new variable names for interesting heap locations, letting the underlying abstract domain operate on these variables.
  </details>
- **Annabelle McIver**, *Probabilistic loop guards*
- **Dominique Mery**, *Incremental Proof-based Design of Models for Deriving System On Chip Architecture*
  <details><summary>Abstract</summary>
  The Digital Video Broadcasting (DVB) set of digital TV standards specify baseline systems for various transmission media: satellite, cable, terrestrial. The design of these systems requires a common understanding of measurement techniques and the interpretation of measurement results. The evaluation of the quality of signal transmission is a critical issue for the DVB-T context; it requires the design of a monitoring tool conform to the normalisation documents. The methodology, for designing models of system from requirements, leads to formally justified hints on the future architectural choices of that system; it is based on the B event-based method, which integrates the incremental development of models using a theorem prover to validate each step of development called refinement. Dependency graphs are derived from abstract mathematical models of the system; they express a hierarchy among parameters which is automatically validated through the refinement process; they provide hints for the future architecture of the SoC.
  </details>
- **Bertrand Meyer**, *Proving object-oriented components*
- **Carroll Morgan**, *Exact expected convergence time for Herman's Ring*
  <details><summary>Abstract</summary>
  "Herman's Ring" is an algorithm for self-stabilisation of a token ring, and dates from about 1990. Its expected time to stabilisation was originally stated to be O(n^2 * log.n); since then it has been improved to O(n^2). Recently we have found an exact solution, in probabilistic programming logic, for the expected time to stabilisation from initial states comprising just three tokens (and it is Theta(n^2)). However, tabulations using the PRISM probabilistic model-checker of expected convergence from demonically selected initial states agree with our exact value for just three tokens. Can it be proved therefore that the three-token case is no faster on average than any of the other odd-number-of-token cases, so that our exact solution will apply in general?
  </details>
- **Madhu Parthasarathy**, *Pending Calls and Matching Returns in Temporal Specifications*
  <details><summary>Abstract</summary>
  Model checking of linear temporal logic (LTL) specifications with respect to pushdown systems has been shown to be a useful tool for analysis of programs with potentially recursive procedures. LTL, however, can specify only regular properties, and properties such as correctness of procedures with respect to pre and post conditions, that require matching of calls and returns, are not regular. We introduce a temporal logic of calls and returns (Caret) for specification and algorithmic verification of correctness requirements of structured programs. Besides the standard global temporal modalities, Caret admits the abstract-next operator that allows a path to jump from a call to the matching return. Caret also admits the last-caller modality that jumps to the most recent pending call, and such caller modalities allow specification of a variety of security properties that involve inspection of the call-stack. We show that model checking Caret formulas against a pushdown model is decidable, with the same complexity as checking LTL formulas.
  </details>
- **Benjamin C. Pierce**, *Harmony: A synchronization framework for tree-structured data*
  <details><summary>Abstract</summary>
  Increased use of optimistic data replication has led to increased interest in synchronization technologies. The goal of the Harmony project is to develop a generic framework for synchronizing tree-structured data -- i.e., a tool for propagating updates between different copies, possibly stored in different formats, of tree-shaped data structures. For example, Harmony can be used to synchronize the bookmark files of several different web browsers, allowing bookmarks and bookmark folders to be added, deleted, edited, and reorganized by users running different browsers on disconnected machines. Other Harmony instances under development include synchronizers for calendars, address books, Keynote presentations, structured documents, file systems, and generic XML and HTML. Joint work with Michael Greenwald and Alan Schmitt.
  </details>
- **Michel Sintzoff**
- **Geoffrey Washburn**
- **Pamela Zave**, *Symmetry in network connections*
  <details><summary>Abstract</summary>
  Usually, protocols and features for telecommunications are highly asymmetric -- they make a strong distinction between the initiating and receiving ends. However, experience shows that many feature functions are symmetric, and many end-to-end connections consist of segments set up in alternating directions. The question: how can we organize and analyze network connections, when taking this richer view?
  </details>
