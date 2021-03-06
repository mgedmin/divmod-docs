============
Divmod Axiom
============

Axiom is an object database whose primary goal is to provide an
object-oriented layer with what we consider to be the key aspects of OO, i.e.
polymorphism and message dispatch, without hindering the power of an RDBMS.
It is designed to 'feel Pythonic', without encouraging the typical ORM
behavior such as :doc:`../philosophy/potato`.

Axiom provides a full interface to the database, which strongly suggests that
you do not write any SQL of your own. Metaprogramming is difficult and
dangerous (as many, many SQL injection attacks amply demonstrate). Writing
your own SQL is still possible, however, and Axiom does have several methods
which return fragments of generated schema if you wish to use them in your own
queries.

Axiom currently supports only SQLite and does NOT have any features for
dealing with concurrency. We do plan to add some later, and perhaps also
support other databases in the future. Take a look at
[wiki:DivmodAxiom/ConcurrencyScalability our concurrency and scalability page]
for more information - we'll update this as the community makes progress on
these issues.

Performance
===========

How does Axiom perform?

Here are some simple third-party [http://www.livejournal.com/users/william_os4y/1271.html benchmarks].

Download
========

 * Stable: [http://divmod.org/trac/attachment/wiki/SoftwareReleases/Axiom-0.6.0.tar.gz?format=raw Download the latest release - 0.6.0!] (Requires [wiki:DivmodEpsilon Epsilon]) ([source:/tags/releases/Axiom-0.6.0/NEWS.txt Release Notes])
 * Trunk: svn co http://divmod.org/svn/Divmod/trunk/Axiom Axiom

See Also
========

 * [wiki:DivmodAxiom/Tutorial]: The Axiom tutorial. (Still in progress.)
 * [wiki:DivmodAxiom/AxiomTutorial Exarkun's Axiom and Mantissa tips]: Short, sharp Axiom/Mantissa tips and tricks.
 * [wiki:DivmodAxiom/WhyAxiom Why Axiom]: Glyph writes about the advantages of Axiom over other RDBMS and ORM alternatives.
 * [wiki:DivmodAxiom/Reference Reference]: A reference to the Axiom public API. (Incomplete but evolving!)
 * ''Development'' version of the [http://buildbot.divmod.org/apidocs/axiom.html Axiom API docs]
 * [wiki:DivmodAxiom/Examples Examples]
 * [query:?status=new&status=assigned&status=reopened&groupdesc=1&group=type&component=Axiom&order=priority Axiom tickets]
 * [wiki:Axiomatic axiomatic]
 * [wiki:DivmodAxiom/DependencyTransition Dependencies]: How to transition from pre-{{{axiom.dependency}}} code.
 * [wiki:DivmodAxiom/Powerups Powerups]
 * WritingUpgradeTests: writing stubloader tests for schema upgrades.
 * [wiki:DivmodAxiom/Files How to handle files in Axiom]
