---
layout: page
title: "Meeting 047"
location: "Santa Fe, NM, USA"
date: "8-12 October 2007"
parent: Meetings
---

<h3>Host: Bob Baltzer</h3>

<p>Where:  <a href="http://www.santafesageinn.com/">Santa Fe Sage Inn</a>, Santa Fe, New Mexico, USA.
When:  8-12 October 2007
Host:  Bob Baltzer</p>
<p>The pictures on this pages were taken by Carroll Morgan.  For more pictures from the meeting, Santa Fe, and the Albuquerque Balloon Fiesta, see the collections by <a href="http://www.cse.unsw.edu.au/~carrollm/M47/">Carroll Morgan</a> and by <a href="http://picasaweb.google.com/IFIP.WG2.3">Jim Horning et al.</a></p>

<h3>Topics of discussion</h3>
<ul>
	<li>Daniel Jackson, <em>Modelling with events
</em></li>
	<li>Peter M�ller, <em>A Unified Framework for Verification Techniques for Object Invariants
</em>On joint work with Sophia Drossopoulou and Adrian Francalanza

<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/Mueller.jpg" alt="">I will present a unified framework to describe verification techniques for object invariants. I will distil seven parameters, which characterize a verification technique, and identify sufficient conditions on these parameters under which a verification technique is sound. I will also define what it means for a technique to be modular. To illustrate the generality of our framework, I will instantiate it with verification techniques from the literature. The framework facilitates the assessment and comparison of the soundness, modularity, and expressiveness of these techniques.</li>
	<li>
<div id="McIver"><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/McIver.jpg" alt="Annabelle McIver"></div>
<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/Broy.jpg" alt="Manfred Broy">Manfred Broy, <em>Two Sides of Structuring Multi-Functional Software Systems:  Function Hierarchy and Component Architecture
</em>
I would very much like to do a presentation about the material you have already seen which had made good progress in describing a structured view on the functionality of multi-functional systems.
<em> </em></li>
	<li>Jim Woodcock, <em>Modelling Flash Memory</em>

Abstract: Flash memory is a kind of electrically erasable programmable read-only memory. Because it is non-volatile and relatively dense, it is often used as a substitute for magnetic disks, but it has two major limitations: the erasure block size is large and erasure causes memory cells to wear out. To overcome these limitations requires sophisticated algorithms and data structures, and I will give an overview of some of the problems involved. This work is part of the Verified Software Initiative pilot project to mechanically verify a POSIX-compliant file-store for critical applications. Insensitivity to shocks and changes in pressure and temperature and the lack of rotating parts make flash memory particularly attractive in space-slight missions.</li>
	<li>Shriram Krishnamurthi, <em>Fun Implementing a SIGGRAPH paper:  Content-Aware Resizing of Images
</em>
See <a href="http://www.seamcarving.com/">http://www.seamcarving.com/</a>.</li>
	<li>Eric C. R. Hehner, <em>Incomputable Indeed</em>

I argued that there are no incomputable (or uncomputable) functions, see<a href="http://www.cs.utoronto.ca/~hehner/II.pdf">www.cs.utoronto.ca/~hehner/II.pdf</a>.</li>
	<li>Annabelle McIver, What makes a good counterexample in (probabilistic) system verification?
On joint work with Carroll Morgan and Carlos GonzaliaOne of the successes of automated formal verification is in the generation of counterexamples which can lead to debugging specifications, or correcting faulty implementations. In probabilistic system design there is no tradition of using counterexamples in this way to aid system verification, and indeed there is not yet a standard notion of what a counterexample should be.

In this talk I shall explore the question of what makes a "good" counterexample in system verification, using the context of probabilistic systems as a case study.</li>
	<li>Pamela Zave, <em>Message Transmission, From the Top Down</em>
With thanks to Cliff Jones and Jim Woodcock</li>
	<li>
<div id="Woodcock" class="style5"><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/Woodcock.jpg" alt="Jim Woodcock"></div>
Peter Henderson, <em>Located Functions
</em></li>
	<li>Douglas R. Smith, <em>Synthesis of Propositional Satisfiability Solvers
</em></li>
	<li>Ernie Cohen, <em>Short Problem:  Optimal Replay</em>

A solution written in BoogiePL (which verifies in 1.5 seconds with Boogie): <a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/ErniesBrkpts.bpl">ErniesBrkpts.bpl</a></li>
	<li><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/Joshi.jpg" alt="Rajeev Joshi">Rajeev Joshi, <em>Formally Specifying Filesystems Robust to Hardware Failures</em>
Joint work with Gerard Holzmann and Alex Groce</li>
	<li>Rustan Leino, <em>Designing a Type System for BoogiePL 2
</em></li>
	<li>Michael Butler, <em>Experience with Refining Event Atomicity</em></li>
	<li>William Cook, <em>Models for Application Programming
</em></li>
	<li>Clark Barrett, <em>Satisfiability Modulo Theories
</em></li>
	<li>Carroll Morgan, <em>Horses for Courses:  Multi-paradigm Specification and Proof ...Eventually
</em>Reporting the work of Annabelle McIver and Ernie Cohen.

Rabin's (distributed, probabilistic) mutual exclusion algorithm addresses the liveness of resource sharing by guaranteeing a probabilistic lower bound on the chance that a process competing for a shared resource will actually get it. At its core is a clever and unexpected mathematical "gem" around which the details of concurrency and overlapping executions are set: the gem is not obvious (to anyone but Rabin), but is nevertheless easily proved; the details of organising the concurrency, on the other hand, are obvious but not so easily proved. In fact there was an error in Rabin's original presentation.

A rigorous proof/development of Rabin's algorithm seems very difficult; "Horses for Courses" means choosing the right tool for the job which, in this case, suggests a "multi-layered" technique with a different formalism for each layer. One layer uses probabilistic sequential techniques (pGCL, not much discussed in this talk); one -- the most intricate-- uses a probabilistic extension of Separation-and- Reduction technique (pKA, this talk); and one can be done in "ordinary maths" on a napkin.

The talk summarises the history of the problem, and the proposed solution strategy (due to Annabelle and Ernie), and sketches what the progress so far has delivered. There turn out to be interesting links between pKA and other Kleene-style algebras invented for a wholly different purpose.</li>
	<li>Greg Nelson, <em>P47: A Short Film</em>

I would like to lead a discussion on <em>proof animation</em>.  I will start the discussion off by showing an animated proof of approximately 5 minutes that I have produced over the last few months and ask for the reactions of the group.</li>
	<li>Ernie Cohen, <em>Infinite Atomic Actions
</em>
I will talk about how to extend sequential programming semantics to allow information to escape infinite loops. The interesting thing is that there turns out to be essentially no choice about the language used to specify state properties.</li>
	<li>Ian J. Hayes, <em>Teleo-Reactive Systems and Timebands
</em></li>
	<li>Greg Nelson, <em>Choice of Choice Compositions in Guarded Commands
</em></li>
	<li><img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/FantasticFour.jpg" alt="McIver, Cohen, Smith, Jackson">Ernie Cohen, <em>Pessimistic Testing
</em>
Pessimistic testing is an approach to model-based testing of nondeterministic systems where you stop testing as soon as the system has a strategy to stop you from making progress.</li>
	<li>Ian Hayes, <em>An Alternative Typing of Records:  moving typing information back from fields to records
</em></li>
	<li>Ernie Cohen, <em>The Hypervisor Verification Project</em>

I will talk about the Hypervisor Verification project, some of the tricks we're using, and some of the challenges we face. This would hopefully stir discussion.</li>
</ul>
<h3>Attendees</h3>
<ul>
	<li>Bob Balzer (host)<img src="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/47/Balzer.jpg" alt="Bob Balzer"></li>
	<li>Clark Barrett</li>
	<li>Manfred Broy</li>
	<li>Michael Butler</li>
	<li>Ernie Cohen</li>
	<li>William Cook</li>
	<li>Ian Hayes</li>
	<li>Eric Hehner</li>
	<li>Peter Henderson</li>
	<li>Jim Horning</li>
	<li>Daniel Jackson</li>
	<li>Rajeev Joshi</li>
	<li>Shriram Krishnamurthi</li>
	<li>Butler Lampson</li>
	<li>Rustan Leino</li>
	<li>Annabelle McIver</li>
	<li>Carroll Morgan</li>
	<li>Peter Müller</li>
	<li>Greg Nelson</li>
	<li>Michel Sintzoff</li>
	<li>Doug Smith</li>
	<li>Jim Woodcock</li>
	<li>Pamela Zave</li>
</ul>
