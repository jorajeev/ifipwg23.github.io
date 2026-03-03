---
layout: page
title: "Meeting 043"
location: "Prato, Italy"
date: "6-10 September 2004"
parent: Meetings
---

<h3>Host: Bertrand Meyer</h3>

<p>Where:  Prato, Italy
When:  6-10 September 2004
Host:  Bertrand Meyer</p>
<p>Here is an <a href="http://tinyurl.com/5t2fd">overview of Prato and the Monash center</a>.  Here are <a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/index.htm">many more pictures</a>, courtesy of Carroll Morgan and Gary Leavens.</p>

<h2>Topics of discussion</h2>
<ul>
<ul>
	<li>Cliff Jones, <i>Beyond "Verifying Compiler".
</i>
One conclusion:  The "Verifying Compiler" should not be concerned with verifying the absence of bugs, but help with the design of software.

Recommended reading:
<ul>
	<li>Donald MacKenzie's 1995 work that analyzes the failures that led to some 1100+ deaths</li>
	<li>Jones, Hoare, and Randell: "Extending the horizons of DSE [Grand Challenge GC-6 on "Dependable Systems Evolution", accepted by UKCRC]"</li>
</ul>
</li>
	<li></li>
Discussion of the Grand Challenge of a Verifying Compiler (or, a Verifying Development Environment)</ul>
</ul>
 
<ul>
	<li>Gary Leavens, <i>Alias-Free Formal Parameters<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Leavens.jpg" alt="Gary Leavens"></i>

Aliasing among formal parameters, and among formals and globals, causes problems for both optimization and reasoning; such aliases are a source of subtle errors in programs.  Whole-program static analysis could provide knowledge about such aliasing, but it is non-modular, expensive, and conservative. All of these characteristics are undesirable for reasoning.

I will describe a small extension to Java and JML that leads to significantly better optimization opportunities for a compiler and allows modular reasoning.  The extension allows aliasing among arguments and globals at the call site, but guarantees there will be no overlap among arguments and globals inside method bodies, and also allows methods to have specifications that "work" for overlapping arguments.  This is done by having multiple bodies for each procedure, up to one for each aliasing pattern.  Procedure calls are automatically dispatched to the body that matches the run-time aliasing pattern among the actual parameters and the globals.

This talk is based on joint work with Medhat Assaad and Olga Antropova.  Thanks to Jim Horning, Murali Sitaraman, Greg Kulczycki, William Ogden, and Bruce Weide for discussions of related topics.  This work is supported in part by the US National Science Foundation under grants CCR-9803843, CCR-0097907, CCR-0113181, CCF-0428078, and CCF-0429567.</li>
	<li>Peter Müller, <i>Modular verification of object and module invariants</i> <img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Mueller.jpg" alt="Peter Müller">
(joint work with Rustan Leino)

The talk describes a methodology for specifying and verifying object-oriented programs, using object invariants to specify the consistency of data and using ownership to organize objects into dynamic contexts.  Object invariants can describe a large variety of properties, including properties of cyclic data structures.  The methodology is designed to allow modular reasoning, even in the presence of subclasses and callbacks.  Module invariants describe properties of variables that are shared by several objects. I would like to discuss how the presented methodology for object invariants can be adapted to cover module invariants.<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Zave.jpg" alt="Pamela Zave"></li>
	<li>Bertrand Meyer, <i>The Dependent Delegate Dilemma
</i>.<i><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Meyer.jpg" alt="Bertrand Meyer"></i></li>
	<li>Pamela Zave, <i>A formal model of addressing for interoperating networks</i>.</li>
	<li>Annabelle McIver, <i>Optimal strategies for two-player parity games</i>

<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Jackson-Butler-McIver.jpg" alt="Michael Jackson, Michael Butler, Annabelle McIver">In this talk I will discuss the problem of <i>finding </i>optimal strategies for two-player games.

Game models of programs can be useful in the specification and analysis of temporal-style properties.  In such models players compete to optimise some specified reward function.  Of particular interest are the strategies they employ for winning the game and, amongst those, "memoriless" strategies --- those which only depend on the current game configuration --- are arguably the most useful of all.

It has recently been proved that in the stochastic parity-game setting optimal memoriless strategies exist for each player --- and in fact they can be assumed to be "pure", ie. they do not need to be randomised.  Unfortunately determining those optimal memoriless strategies can be problematic.

I will show how optimal memoriless strategies can be computed reasonably simply, provided that non-pure strategies are an acceptable solution.</li>
	<li>Michael Jackson, <i>The problem of the banker with 52 cards</i>.

A “banker” has an ordinary 52-card deck of cards.  You have some positive amount of money.  The banker decides on the order of the cards.  Before the banker turns each card over, you place a bet.  You put some proportion of you money on “red” and the rest on “black”.  After the banker turns over the card, you lose the money you bet on the losing color, and double the money you put on the winning color.  Design a strategy that maximizes your guaranteed gain, and prove this strategy correct.</li>
	<li>Ian Hayes, <i>Finding Faults</i>

Examining systematic methods for detecting faults in components, including timing faults.</li>
	<li>Michael Butler, <i>Semantics and atomicity for long-running transactions</i>

<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Butler.jpg" alt="Michael Butler">Long-running transactions lack the atomicity of ACID transactions.  Instead of rollbacks and checkpoints, compensation is used to recover from error.  The development of a trace semantics has lead to a structured design for a language of long-running transactions and also to a rational basis for the use of compensation in which a degree of atomicty can be recovered.

Links:
<ul>
	<li><a href="http://www.b4free.com/">Free distribution of B system</a></li>
	<li>The <a href="http://www.ecs.soton.ac.uk/~mal/systems/prob.html">ProB</a> Animator and Model Checker for the B Method</li>
</ul>
</li>
	<li><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Jones.jpg" alt="Cliff Jones">Cliff Jones, <i>Towards a development method, "Splitting atoms safely"</i>.

Some notes:
Wanted:  a method that provides the fiction of atomicity.  Can atomicity be used in program design?  Wants atomicity refinement, especially in combination with data refinement.

Related items:
<ul>
	<li>New (and clear!) database book by Gerhard Weikum</li>
	<li>"Atomicity in system design and execution", Dagstuhl seminar, April 2004</li>
</ul>
</li>
	<li>Mark Utting, <i>Model-Based Testing</i>
<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Hayes-Utting.jpg" alt="Ian Hayes and Mark Utting">
In this talk, I will describe the problems of generating good test suites from formal specifications (pre/post style).  The goal is to build a practical tool (the LTG -- <a href="http://www.leirios.com/">Leirios Test Generator</a>) that engineers can use to semi-automatically generate tests from B, Z, JML, UML or Statechart specifications.</li>
	<li>Bertrand Meyer, <i>The mathematics of object computation</i>.</li>
	<li>Jean-Raymond Abrial, <i>Developing discrete transition systems</i>.

<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Abrial.jpg" alt="Jean-Raymond Abrial">(1) <i>Refinement of Stuttering steps: skip or keep (or both)</i>.  Stuttering steps are usually considered to be refinement of skip.  In certain cases, it is interesting however to think of them as being a refinement of (a sort of) keep (the action that maintain the invariant).  Presentation, problems, discussion.

(2) <i>Temporal Statements and Refinements</i>.  Is it claimed that it is possible to completely avoid certain temporal logic statements and replace them by refinements of stuttering steps.  This raises the problem of characterizing systems which run forever.  Generalization of "pre, post" pairs.</li>
	<li>Carroll Morgan, <i>Compositionality and "pCSP"</i>.

Compositional semantics for probabilistic process algebras have been studied for decades: one of the major problems is the interaction of the various forms of choice: probabilistic, internal, external (to use CSP terminology).  What's the new angle?

Work with Annabelle on sequential semantics for probability and demonic choice has given a logic which is discriminating enough in its observations to reconstruct the operational (but sequential) program that led to the observations.  The proof of that is not trivial, and (therefore?) the technique is not much used by other researchers.  Yet.

(It is <i>expected values</i>, not new for IFIP2.3...)

Thus we hope it might give us some leverage on this problem.  Related issues turn out to be information hiding and (of course) simulation.<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Dietl-Arnout.jpg" alt="Werner Dietl and Karine Arnout"></li>
	<li>Werner Dietl, <i>Object Ownership - Overview and Issues</i>

Abstract:  I will motivate object ownership and show three concrete systems that enforce it - two type systems and one dynamic solution.  There should be multiple possible discussion topics, from the basic motivation and possible applications down to technical problems.</li>
	<li>Alexander Petrenko, <i>Specification Based Testing (SBT): A Practical Concern</i>.

<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Petrenko.jpg" alt="Alexander Petrenko">The talk will discuss different issues related to SBT technology development and application.  I will involve our case studies for KVEST, UniTesK and OTK technologies developed and applied in several projects for Nortel Networks, Microsoft, Intel and other customers.  Main points of the talk are as follows:
<ul>
	<li>KVEST and <a href="http://www.unitesk.com/">UniTesK</a> technologies for test generation from contract specifications</li>
	<li>Roles of models in test suite generation and multiparadigm specifications in real life applications
<ul>
	<li>models of: requirements, faults, test coverage, implementation architecture/structure, behavior (history, trace)</li>
	<li>paradigm combinations: contract specification and FSM/LTS,</li>
	<li>paradigm alternatives in compiler unit testing: contract specification vs. language specification</li>
</ul>
</li>
	<li>Highest priorities of SBT introduction in practice
<ul>
	<li>specification without specification language</li>
	<li>how to use formal methods without mathematic background
<ul>
	<li>learning and management</li>
</ul>
</li>
	<li>SBT vs. conformance testing</li>
	<li>detail vs. simple models and test scenarios</li>
</ul>
</li>
</ul>
</li>
	<li>Rustan Leino, <i>On bounded model checking, induction, and interpolants</i>.

Many interesting state-based computer systems--both software programs and hardware circuits--can be represented as <i>transition systems</i>.  An execution of a transition system begins in some initial state and then repeatedly applies a transition relation to obtain the next state.  An important question for such a system is whether or not it is possible for the system to reach some given set of ``bad'' states.  In this discussion, I consider ways to determine such reachability, trying to uniformly present previous attempts.

Slides:  [<a href="http://research.microsoft.com/~leino/papers/krml142.ppt">PowerPoint</a>] [<a href="http://research.microsoft.com/~leino/papers/krml142-slides-wg23.pdf">PDF</a>]</li>
	<li> <img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/McIlroy.jpg" alt="Doug McIlroy">Bertrand Meyer, <i>"Test Studio" from Eiffel Software / ETH</i>.<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Leino-Sintzoff.jpg" alt="Rustan Leino and Michel Sintzoff"><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/43/Hehner.jpg" alt="Eric Hehner"></li>
	<li>Also present:
<ul>
	<li>Karine Arnout</li>
	<li>Eric Hehner</li>
	<li>Doug McIlroy</li>
	<li>Michel Sintzoff</li>
</ul>
</li>
</ul>
