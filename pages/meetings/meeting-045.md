---
layout: page
title: "Meeting 045"
location: "Bruges, Belgium"
date: "13-17 March 2006"
parent: Meetings
---

<h3>Host: Michel Sintzoff</h3>

<p>Where:  <a href="http://www.brugge.be/internet/en/index.htm">Bruges</a>, Belgium.  <a href="http://book.bestwestern.com/bestwestern/productInfo.do?propertyCode=92603">Navarra Hotel</a>, 41 Sint-Jakobsstraat, +32 50 340561  --  <a href="http://www.viamichelin.co.uk/viamichelin/gbr/tpl/hme/MaHomePage.htm">maps</a>  --  <a href="http://www.b-rail.be/main/E/index.php">trains</a>.
When:  13-17 March 2006
Host:  Michel Sintzoff</p>

<h2>Topics of discussion</h2>
<ul>
	<li>Ralph Back

I have two topics that I would like to talk about,
- <i>Invariant based programming</i>, and
- <i>The software factory approach to experimental software construction</i>
in this order.</li>
	<li>Dines Bjørner</li>
	<li>John R. Harrison, <i>Proving invariants using many-sorted logic</i>

[<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/45/Harrison-slides.pdf">slides</a>] [<a href="http://www.cl.cam.ac.uk/users/jrh/papers/manysorted.pdf">paper (PDF}</a>]</li>
	<li>Peter Henderson</li>
	<li>Tony Hoare, <i>VSTTE conference</i>

To give a preliminary report on the Conference, and discuss further developments.</li>
	<li>Michael Jackson</li>
	<li>Cliff Jones</li>
	<li>Shriram Krishnamurthi, <i>The Interactive Web</i>

Web programs are important, increasingly representing the primary public interfaces of commercial organizations.  Unfortunately, Web programs also exhibit numerous flaws.  In addition to the usual correctness problems faced by software, Web programs must contend with numerous subtle user operations such as clicking the Back button or cloning and submitting a page multiple times.  Many existing Web verification tools fail to even consider, much less effectively handle, these operations.

I describe a model checker designed to identify errors in Web software.  I present a technique for automatically generating novel models of Web programs from their source code; these models include the additional control flow enabled by these user operations.  In this technique, I exploit a constraint-based approach to avoid over-approximating this control flow; this approach allows us to evade exploding the size of the model.  Time permitting, I will also outline a base property language that permits specification of useful Web properties, along with property idioms that simplify specification of the most common Web properties.</li>
	<li>Butler W. Lampson</li>
	<li>Gary T. Leavens, <i>Verification by Construction</i>

In this talk I will present a draft of the research roadmap being worked on by the Verification by Construction subgroup of the Verified Software: Theories, Tools, Experiments conference.  Discussions about the recommendations will be welcome.</li>
	<li>K. Rustan M. Leino, <i>Integrated Verification</i>

In this talk I will present a draft of the research roadmap being worked on by the Integrated Verification subgroup of the Verified Software: Theories, Tools, Experiments conference.  Discussions about the recommendations will be welcome.</li>
	<li>Peter Müller, <i>Data Abstraction in Spec# and Boogie</i></li>
	<li>Tobias Nipkow, <i>A machine-checked proof of the enumeration of tame plane graphs</i>

Hales' proof of the Kepler conjecture defines a class of tame plane graphs, enumerates that class by computer and checks (again by computer) that none of these graphs constitute a counterexample to the conjecture.  This talk reports on the verification of a functional version of Hales' Java program for enumerating tame plane graphs: it is shown that all such graphs are found.  This is part of Hales' Flyspeck project to check his whole proof by computer.

Throughout the talk we concentrate on the issues that arise when checking mathematical arguments by machine, in particular the challenge of writing programs that are both efficient enough to perform complex searches and enumerations but simple enough that machine-checked correctness proofs become feasible.

Joint work with Gertrud Bauer and Paula Schultz.  Here's a link to the <a href="http://www.in.tum.de/~nipkow/pubs/Flyspeck/">slides</a>.</li>
	<li>J. R. Rao, <i>Recent advances in side-channel cryptanalysis</i></li>
	<li>Jean-François Raskin, <i>A lattice theory for solving games of imperfect information</i> [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/45/Raskin-paper.pdf">pdf</a>] [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/45/Raskin-GamesOfImperfectInformation.pdf">slides</a>]

In this paper, we propose a fixed point theory to solve games of imperfect information.  The fixed point theory is defined on the lattice of antichains of sets of states.  Contrary to the classical solution proposed by Reif, our new solution does not involve determinization.  As a consequence, it is readily applicable to classes of systems that do not admit determinization.  Notable examples of such systems are timed and hybrid automata.  As an application, we show that the discrete control problem for games of imperfect information defined by rectangular automata is decidable.  This result extends a result by Henzinger and Kopke.</li>
	<li>Augusto Sampaio, <i>Test sequence generation from process algebra use models</i>

My talk will be in the context of a cooperation project between the Federal University of Pernambuco and Motorola.  The general purpose of the project is to define a formal strategy for supporting several aspects of software testing.  From requirements written in a controlled natural language (with a fixed BNF), the first step is to build a use model represented in CSP.  From the use model, several artifacts are generated.  I will concentrate on some initial ideas towards a strategy for automatically generating test sequences direct from the CSP use model: either addressing the entire model or just a subset of the model, based on the concept of test purposes (also described as CSP processes).  The actual extraction of test sequences is based on refinement checking and can be mechanised using FDR.  The major intended contribution is to recast consolidated approaches to test sequence generation (typically based on more operational models like LTS or FSM) entirely in the context of a process algebra.

This cooperation involves some colleagues and students at my university.  The particular approach to test sequence generation is joint work with Alexandre Mota and Sidney Nogueira.</li>
	<li>Michel Sintzoff (chair)</li>
	<li>Douglas R. Smith, <i>Features/Policies/Aspects: Specification and Enforcement</i>

The focus of my recent work has been on synthetic techniques for system design by feature composition.  I developed a technique for specifying AspectJ-style aspects as logical invariants, and then treating aspect weaving as automatic invariant maintenance (ala Paige's Finite Differencing technique).  I also developed an automata-based formalism for specifying features/policies and corresponding enforcement mechanisms based on static analysis.  The topic I pose is how to lift such automata-based policies to logical specifications from which we can calculate the the same effect as enforcing an automaton-based policy.

Here is a paper that reports some of the ideas in my presentation: [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/45/Smith.pdf">pdf</a>]</li>
	<li>Ketil Stølen, <i>STAIRS towards formal design with sequence diagrams</i> [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/45/St%C3%B8len-20060313.IFIP-WG2.3.pdf">slides</a>]

The STAIRS-method addresses the challenges of harmonizing intuition and formal reasoning.  That UML interactions (e.g. sequence diagrams) are attractive and intuitive and have been established for years.  With the new structuring mechanisms of UML 2.0, they have become more powerful and compact.  How can we make sure the intuitive feeling is kept in a process of gradually making the diagrams more elaborate and precise?  How can we make the descriptions such that they are maintainable through the lifecycle of the full UML model?  Our answer lies in a precise understanding of the partial nature of sequence diagrams, and of consistent refinement of such partial understanding to a more complete one.</li>
	<li>Peter Van Roy, <i>Convergence in language design: a case of lightning striking four times in the same place</i> [<a href="http://research.microsoft.com/en-us/um/people/leino/IFIP-WG2.3/media/45/VanRoy-FLOPStalkIFIP.ppt">slides</a>]<i>

</i>What will a definitive programming language look like?  By <i>definitive language</i> I mean a programming language that gives good solutions at its level of abstraction, allowing computer science researchers to move on and work at higher levels.  Given the evolution of computer science as a field with a rising level of abstraction, it is my belief that a small set of definitive languages will eventually exist.  But how can we learn something about this set, considering that many basic questions about languages have not yet been settled?  In this paper, I give some tentative conclusions about one definitive language.  I present four case studies of substantial research projects that tackle important problems in four quite different areas: fault-tolerant programming, secure distributed programming, network-transparent distributed programming, and teaching programming as a unified discipline.  All four projects had to think about language design.  In this paper, I summarize the reasons why each project designed the language it did.  It turns out that all four languages have a common structure.  They can be seen as layered, with the following four layers in this order: a strict functional core, then deterministic concurrency, then message-passing concurrency, and finally shared-state concurrency (usually with transactions).  This confirms the importance of functional programming and message passing as important defaults; however, global mutable state is also seen as an essential ingredient.</li>
	<li>Pamela Zave, <i>Toward a discipline of service routing

</i>This talk introduces basic ideas about what service routing is, why it is not supported by the current Internet architecture, what architectural  support might look like, and why it would be valuable to have in the next-generation Internet.</li>
</ul>
