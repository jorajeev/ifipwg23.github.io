---
layout: page
title: "Meeting 046"
location: "Sydney, Australia"
date: "8-12 January 2007"
parent: Meetings
---

<h3>Host: Annabelle McIver</h3>

Where:  <a href="http://www.wesley.usyd.edu.au/">Wesley College, University of Sydney</a>, Sydney, Australia.  <a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/46/DirectionsN.pdf">Directions</a>.
When:  8-12 January 2007
Host:  Annabelle McIver

Sydney University is Australia's oldest, and is not too far from downtown, as well as having nearby a busy "university suburb" with nice restaurants etc.
<h2>Topics of discussion</h2>
<ul>
	<li>Michael Butler, <em>Refining reactive models to concurrent programs

</em>Second topic:  <em>Applying Event-B to Modex
</em></li>
	<li>Carlos Gonzalia</li>
	<li>Ian Hayes, <em>Iteration in real-time programs: finite, infinite, or either
</em></li>
	<li>Joe Hurd, <em>Mechanizing the Probabilistic Guarded Command Language</em></li>
	<li>The probabilistic guarded-command language pGCL contains both demonic and probabilistic nondeterminism, which makes it suitable for reasoning about a wide range of algorithms.  In this talk I'll present a mechanization of pGCL in the HOL theorem prover, which validates the theory and can be used as a platform for building software verification tools.  Along these lines I'll describe a verification condition generator used to verify the partial correctness of the probabilistic voting stage in Rabin's mutual-exclusion algorithm, as well as some more recent work looking at probabilistic termination.</li>
	<li>Gerwin Klein, <em>Verifying an operating system kernel
</em></li>
	<li>Shriram Krishnamurthi, <em>Towards Reasonability Properties for Access Control Policy Languages</em></li>
	<li>Gary Leavens, <em>Modular Verification of Higher-Order Methods in JML</em>  [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/46/Leavens.ppt">slides - PPT</a>] [<a href="ftp://ftp.cs.iastate.edu/pub/techreports/TR07-04/TR.pdf">Technical Report</a>]We describe a simple, intuitive, and modular approach to specifying higher-order methods in JML.  We also show how to verify code, using Hoare-style, first-order verification conditions, in a sound and modular way.  Verification of client code that calls higher-order methods can take advantage of the client's knowledge about the mandatory calls to make strong conclusions.  The verification technique validates and explains traditional documentation practice for higher-order methods, which typically shows their code.  However, a JML specifications does not have to expose all of its code to clients, but only enough to determine what mandatory calls the method makes and in what states those calls are made.</li>
	<li>This is joint work with Steve M. Shaner (of Iowa State) and David A. Naumann, and is supported in part by NSF grant CCF-0429567.

Short topic:  A picture to illustrate pre- and postconditions</li>
	<li>Some important kinds of methods in object-oriented code involve mandatory dynamically-dispatched calls to unknown methods with very weak specifications.  Such ``higher-order'' methods are used, for example, to notify observers in the Observer pattern.  For these higher-order methods, classical specification techniques use higher-order logic, which tend to be both unintuitive and verbose.  For such specifications, standard verification techniques do not technically require that the mandatory calls are actually made (but only that their effects happen), and the use of higher-order logic makes verification more difficult.</li>
	<li>Rustan Leino, Automatic verification of summations

The goal is to device a way to verify programs that make use of arithmetic summations, carrying out the proofs automatically with an SMT solver.  [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/46/Automatic-verification-of-summations.ppt">slides - PPT</a>]

Short topic:  <a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/46/krml95.pdf">The Golden Rule of Positive Integers</a></li>
	<li>Annabelle McIver</li>
	<li>Carroll Morgan, <em>Schrödinger's Shadow: hidden probabilities; hidden nondeterminism</em>We have both given many speculative talks on the topic, over the years.  Indeed some members might recall Annabelle's spectacular experience at the Napa meeting in California --- proof, if any were needed, that the material she was presenting, our "quantum model" (more below), was truly ahead of its time.  In my case, the only occasion ever, in any 2.1 or 2.3 meeting, that I was successfully prevented for the whole hour from leaving my first slide was when I tried to give a similar talk at the Oxford 2.1 meeting.Our current plans are, now, to use the Shadow model as a guide for hiding probability on its own; if that works then, later still, we will try to hide both probability and nondeterminism, which was our original goal (some 10 years ago).  Approached this way, we might end up with a technique that benefits from its gradual evolution rather than, as with some other methods, having sprung "Athena-like" fully equipped out of someone's head all at once.Specifically --- I will give as an introduction to the topic an explanation of the Shadow model but (differing from all my earlier presentations of it) I will describe its key features from the point of the hidden agenda referred to above.  I will then discuss what our initial ideas for replacing nondeterminism by probability are, and will solicit suggestions from the Group.  With luck I will have reached at least Slide 2 by that point.</li>
	<li>This is work we are on the point of beginning, but have not yet started.</li>
	<li>Both the Shadow- and the Quantum model have as an appealing feature that the hidden variables are somehow "fuzzy" until one looks at them, at which point they "collapse"; and that is why we named the latter model as we did.</li>
	<li>Undeterred, we have taken a more roundabout approach in the meantime, including (with Ernie Cohen) via Kleene-style algebra.  Recently I have published a model/logic for "ignorance refinement" of sequential programs (called "The Shadow Knows..."): it has (I believe) applications for security protocols, etc; and I have used it to derive (post-hoc) Chaum's Dining Crypographers and Rivest's Oblivious Transfer.  Its hidden agenda, however, was to abstract from modularised probability to just modularised nondeterminism (ie unquantified) and then to see whether --- in that simpler context --- it would be move obvious what steps to take for data refinement etc.  I believe that experiment worked.</li>
	<li>Annabelle McIver and I discovered some time ago that the "standard" model for sequential probabilistic/demonic programs has unusual difficulties with data refinement.  The problem is that the usually automatic "hiding" of a module's internal state does not occur easily when probability is hiding from nondeterminism, or vice versa.</li>
	<li>Peter Müller, <em>Alias Control with Universe Types - Overview and Challenges</em>At least half of this talk discusses a new solution to the long-standing ownership transfer problem.  This solution is work in progress and still unpublished.</li>
	<li>In object-oriented programs, an object can potentially reference any other object in the heap and read and modify its fields.  Such programs with arbitrary object structures are difficult to understand, to maintain, and to reason about.  In this talk, I will present the Universe type system, which allows programmers to organize the heap into ownership contexts and to control modification of objects.  I will give an overview of the Universe type system and explain how it enables modular verification of object invariants.  I will also propose a new solution to the ownership transfer problem.</li>
	<li>Shankar, <em>Beyond Satisfiability</em></li>
	<li>Second topic:  An overview of the Verified Software Roadmap</li>
	<li>Michel Sintzoff, <em>Symbolic generation of optimal discrete control

</em>[<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/46/Sintzoff-slides-wg2.3.pdf">slides - PDF</a>]</li>
	<li>Ketil Stølen, <em>Relating computer systems to sequence diagrams with underspecification, inherent nondeterminism and probabilistic choice</em>Having a specification and a computer system, we need to answer the question: Is the system compliant with the specification in the desired way?  In this paper we present three techniques for answering this question when the specification is given as a sequence diagram.  All techniques are independent of the choice of programming language used for the system.  The three techniques correspond to three variations of sequence diagrams: Sequence diagrams with underspecification, sequence diagrams with inherent nondeterminism and sequence diagrams with probabilistic choice.  The first technique is a special case of the two others, meaning that for the simplest sequence diagrams all techniques will give the same answer.  The semantics of sequence diagrams is given by denotational trace semantics.  In order to answer the initial question, all three techniques start by obtaining the trace-set of an implementation by e.g. testing, and then transforming this into the same semantic model as that used for sequence diagrams in order to be able to compare the two semantics.  We define different conformance relations, to be used for relating systems to sequence diagrams produced at various stages in the development process.</li>
	<li>Joint work with Ragnhild Kobro Runde and Atle Refsdal.</li>
	<li>This presentation attempts to answer all the questions the audience had with respect to the notion of implementation for sequence diagram specifications in STAIRS at the meeting in Brugge.</li>
	<li>Mark Utting, <em>Practical Model-Based Testing</em></li>
	<li>Ron van der Meyden, <em>What, Indeed, is Intransitive Noninterference?</em></li>
	<li>The notion of intransitive noninterference from the literature on computer security is intended to express architectural constraints on information flow.  Roscoe and Goldsmith have argued that Rushby's definition of noninterference for intransitive security policies has weaknesses, but their analysis has been felt to be contentious.  A new, and more compelling, example will be presented to show that Rushby's definition admits information flows that are not in accordance with the intuitions it seeks to formalise.  Several alternative definitions will be discussed, all of which are equivalent to the classical definition of noninterference with respect to transitive policies.  One of the definitions is shown to be related to unwinding conditions and security of access control systems in ways that improve upon results of Rushby.  Results will also be presented on
the complexity of checking whether a finite state system satisfies these definitions of noninterference.</li>
	<li>Jim Woodcock, <em>Trading assertions in the verified software repository
</em>
As part of the international grand challenge in verified software, the recent re-examination of the Mondex electronic purse has generated several thousand refinement verification conditions, which have been discharged amongst five different theorem provers. These assertions are to be curated in the verified software repository, and this raises the question of how such assertions can be traded between different theorem provers. One of the immediate problems is to resolve the different treatments of undefinedness. We present a unifying theory and use it to discuss how classical logic can be used to prove and to refute conjectures written in the different logics used in the Mondex experiment.

This is joint work with Mark Saaltink and Leonardo Freitas.</li>
	<li>Pamela Zave</li>
</ul>
