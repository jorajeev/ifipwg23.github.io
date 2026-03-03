---
layout: page
title: "Meeting 044"
location: "Niagara Falls, ON, Canada"
date: "6-10 June 2005"
parent: Meetings
---

<h3>Host: Eric Hehner</h3>

<p>Where:  Niagara Falls, ON, Canada
When:  6-10 June 2005
Host:  Eric Hehner</p>

<h2>Topics of discussion</h2>
<ul>
	<li>Ralph Back

<i>Refinement diagrams and diagrammatic reasoning</i>.  I talked about this at the Marktoberdorf summer school, so if there are too many people who lectured there, so that the material is too familiar, then I will reconsider.  However, this is a topic that I have been working on more intensely for the last year or so.  Essentially, I propose a mathematical framework based on lattice theory for describing and analysing large software systems:  their construction, achitecture and evolution.  I propose a diagrammatic way of representing the software structure, and for reasoning about the correctness of the software.  The diagrammatic reasoning is essentially equivalent to a Hilbert like proof in a small subtheory of lattices.  We have been working on a software tool that shows this kind of diagrams with 3D rendering and browsing.

<i>Teaching mathematics in high school</i>.  Jockum and I are finishing a text book on this topic, and I would like to describe the essential idea of our approach and of the way we have approached the problem in the book.</li>
	<li>Michael Butler, <i>Refinement of an automatic refinement checker</i>

Automatic refinement checking has recently been added to the ProB tool for B.  Firstly, I will introduce the tool.  Secondly, I will describe how a refinement approach (in B) is being used to prove the correctness of the refinement checker.  This is joint work with Michael Leuschel.</li>
	<li>Ernie Cohen, <i>Soliciting a verifier for a well-structured 40-KLOC C program.</i></li>
	<li>John Harrison, <i>Verifying the verifier</i>

A complaint sometimes levelled against formal verification is that the theorem prover or model checker may be just as prone to bugs as the system being verified.  A partial answer to this is to design the verification system around a small trusted core (e.g. in the "LCF" approach to building a theorem prover).  A further step is to perform a verification of this core.  I will report on a partial verification of the core of HOL Light (433 lines of OCaml) as well as discussing related work that I know about.</li>
	<li>Rick Hehner, <i>Specification Blocks</i></li>
	<li>Tony Hoare, <i>Retractions in process algebra</i>

With Jifeng's help, I am hoping to discover how to embed an algebra like CSP within a less abstract one like CCS.  I hope the proofs will be elegant too.</li>
	<li>Cliff Jones, <i>Dynamically creating objects and sequencing operations: linking 2 approaches

</i>Slides:  [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/44/Jones-NiagaraWG2.3.ppt">PowerPoint</a>]</li>
	<li>Yannis Kassios, <i>Dynamic Frames</i>

Two important features in object oriented refinement theories are (a) the encapsulation through the use of specification attributes (also known as model fields) and dependencies and (b) the support for pointers.  It is known that the combination of these two features makes the frame problem hard to solve, because it introduces the possibility of <i>abstract aliasing</i>.  Most theories cope by restricting somehow one of the two features.  For theories that provide full support of both features, there are two major proposals to address the frame problem:  Nelson and Leino's 2002 TOPLAS paper [Leino and Nelson 2002] and Müller's universe type system [Müller 2002].  Both approaches work by imposing restrictions on the programmer and thus ensuring that abstract aliasing does not happen at all.

In my work, I argue that a problem with these two approaches is that the possibility of abstract aliasing at a certain state is not expressible in their respective languages.  I introduce the theory of dynamic frames, which allows such properties to be expressed.  I show that dynamic frames address the frame problem without imposing any restriction to the programmer.  I demonstrate the effectiveness of the theory with some examples, the most advanced of which would have been impossible in either of the two other major proposals.

Furthermore, I argue that object oriented specifications should be decoupled from classes and the more general concept of "theories" should be used instead.  Theories are supported by algebraic specification languages, which have however inadequate support for pointers.  I show that dynamic frames can make the use of algebraic-like specifications possible in an environment that supports pointers.

This is work in progress.  It is part of a general theory of object oriented refinement, which is going to be my PhD thesis.</li>
	<li>Shriram Krishnamurthi, <i>On a conference submission/review manager</i></li>
	<li>Albert Lai, <i>Operationalizing Predicative Programming: Eager and Lazy</i>

We give an operational semantics for predicative programming; it is very general and includes both an eager fragment and a lazy fragment (in the future there will also be fragments for parallelism, nondeterministic choice, and "ensure").  The eager fragment of this semantics establishes soundness of refinements.  We furthermore extend predictive programming to lazy imperative programming: stating and proving refinements of time bounds of lazy programs (without whole-program analysis!), the soundness of which is established by the lazy fragment of our operational semantics.</li>
	<li>Gary Leavens, <i>Adapting Observational Purity to JML</i>

The type system of the Java modeling language (JML) uses a notion of <i>purity</i> to prevent side effects in assertions.  However, JML's notion of purity checking is too conservative, which causes several unpleasant properties.  In particular, the <tt>equals</tt> method of Java's <tt>Object</tt> class must be declared pure, because this method needs be used in the specification of various collection classes; however, some subclasses of <tt>Object</tt>, such as <tt>String</tt>, have side effects in their <tt>equals</tt> methods, and since purity is inherited, <tt>Object</tt>'s <tt>equals</tt> method cannot be pure.  We discuss semantical and language design issues involved in adaptating recent work, in particular that of Barnett and Naumann, to solving this problem.  We also explore various practical problems and implications, particularly for run-time assertion checking.

This is joint work with David Cok and David Naumann, and is supported in part by NSF grants CCF-0428078 and CCF-0429567.</li>
	<li>Rustan Leino, <i>Loop invariants on demand</i>

I will talk about a technique for putting an abstract interpreter into a theorem prover, with the goal that the abstract interpreter will be invoked at times when the proof requires stronger loop invariants.  This provides an opportunity to dynamically choose abstract domains to gradually increase the power and cost of the inference.  It also provides an opportunity to dynamically perform trace partitioning, where the loop invariant inferred applies only to a subset of the program's executions.  It would also be nice to be able to apply this technique to procedure calls.  Joint work with Francesco Logozzo.</li>
	<li>Jay Misra, <i>Orc: A Deterministic Distributed Programming Model

</i>Abstract: Orc is a new model of distributed programming which provides a strong theoretical foundation for internet computing based on compositions of web-services.  Orc combines some of the power and flexibility of process algebra with the simplicity and determinism of synchronous programming models.  We present an operational semantics of Orc and prove some laws analogous to those of Kleene algebra.  We validate the deterministic operational semantics by proving it equivalent to a deterministic form of trace semantics.

There are a few papers on this topic at my web site:
<ul>
	<li>Computation Orchestration: A Basis for Wide-Area Computing [<a href="http://www.cs.utexas.edu/users/psp/Wide-area.pdf">PDF</a>]</li>
	<li>Orchestration in Orc: A Deterministic Distributed Programming Model (with William Cook) [<a href="http://www.cs.utexas.edu/users/psp/OpSemantics.Orc.pdf">PDF</a>]</li>
	<li>A Tree Semantics of an Orchestration Language (with Tony Hoare and Galen Menzel) [<a href="http://www.cs.utexas.edu/users/psp/Semantics.Orc.pdf">PDF</a>]</li>
</ul>
</li>
	<li>Greg Nelson, <i>The Straight-Line Automatic Programming Problem</i>

In general, the automatic programming problem is the problem of constructing a program that meets a given specification.  The Straight-Line Automatic Programming Problem is a special case in which the specification is a multi-assignment to be performed and the program to be constructed is restricted to a sequential composition of primitives that model machine instructions.  This mathematical problem is relevant to the engineering problem of generating (optimal) machine code.  I propose to define the problem precisely and then describe a reduction of the problem to problems for which we have practical solutions, namely SAT solving and E-graph matching.</li>
	<li>Alexander Petrenko, <i>Unsolved solved problems</i>

I am going to prepare a talk on real use of theory results in Computer Science/Software development.  My point is as follows: one of the significant reasons of troubles in introduction of theory results in practice is moving of research focuses from solved (almost solved) problems to newest ones.  I'd like to consider several examples from compiling theory, networking and operating systems.</li>
	<li>Augusto Sampaio, <i>Laws of Object-Oriented Programming</i>

After introducing recent work with Paulo Borba, Ana Cavalcanti and Marcio Cornelio on a comprehensive set of laws for an object-oriented language similar to sequential Java, but with copy semantics, I would like to raise discussion on the following issues:
<ul>
	<li>Laws that remain valid considering reference semantics</li>
	<li>A data refinement law for class hierarchies</li>
	<li>Suitable semantic frameworks for proving these laws</li>
	<li>Adequacy of the algebraic style as a basis for justifying larger grain transformations like refactorings and patterns</li>
</ul>
</li>
	<li>Shankar, <i>Simplex in logical form</i></li>
	<li>Emil Sekerinski, <i>Action-Based Object-Oriented Concurrent Programming</i>

Lime is an experimental programming language that (1) separates class extension (subclassing) from class implementation (subtyping), (2) includes some specification and documentation constructs, and (3) allows objects to run concurrently by specifying actions in classes.  After a brief introduction to the language and its implementation, I like to go into the particular model of concurrency and discuss the difficulties about the atomicity of actions and methods, both in the refinement rules and the current implementation.

Slides:  [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/44/Sekerinski-WG-2.3-June-05.pdf">PDF</a>]</li>
	<li>Michel Sintzoff</li>
	<li>Pamela Zave, <i>Compositional Control of End-to-End Media in IP Networks: A Verification Case Study</i>

Joint work with Eric Cheung.</li>
	<li></li>
</ul>
