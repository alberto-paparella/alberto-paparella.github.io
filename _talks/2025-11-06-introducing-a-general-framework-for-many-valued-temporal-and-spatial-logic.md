---
title: "Introducing a general framework for many-valued temporal and spatial logic."
collection: talks
type: "Conference talk"
permalink: /talks/2025-11-06-reasoning-with-many-valued-interval-temporal-logic
excerpt: "We aim to introduce a possible many-valued extension for well-known temporal and spatial logics based on the family of finite FLew-algebras, allowing for a unified treatment of both fuzzy logics and Heyting algebras, leveraging the notion of a many-valued linear order and allowing for the definition of a many-valued semantics of modal frames. This framework is also implemented as part of an open-source framework for representing, reasoning, and learning from structured and unstructured data, namely Sole.jl, serving as the foundation for reasoning and learning tools leveraging many-valued temporal and spatial logics."
venue: "Australasian Association for Logic Conference 2024"
date: 2025-11-06
location: "University of Queensland, Brisbane, Queensland, Australia"
slidesurl: 'http://alberto-paparella.github.io/files/AAL25_presentation.pdf'
---

Reasoning with temporal and spatial information is crucial in many real-world ap-
plications from different fields. In order to do so, many modal temporal and spatial
logics have been proposed throughout the years, leveraging modal operators to treat
the relations between points in time (Linear Temporal Logic [[1](#1)]) and space (Compass
Logic [[2](#2), [3](#3)]), or even time intervals (Halpern and Shoham’s Interval Temporal Logic [[4](#4)])
or areas in an image (Lutz and Wolter’s Logic of Topological Relations [[5](#5)]).
At the same time, these applications live in scenarios characterized by uncertainty
and vagueness in the data. This problem is usually addressed using fuzzy logics, such
as G ̈odel logic (G) [[6](#6)], Lukasiewicz logic [[7](#7)], and product logic (Π) [[8](#8)].

In terms of temporal logic, only a few attempts have been made to study point-
based temporal languages in the fuzzy case, with early contributions [[9](#9), [10](#10), [11](#11)] that
limited to the fuzzification of the propositional side of formulas, while [[12](#12)] provides a
generalization of Linear Temporal Logic allowing to express uncertainty in both atomic
propositions and temporal relations. In the case of interval temporal logic, [[13](#13), [14](#14), [15](#15)]
introduced and studied a many-valued extension of Halpern and Shoham’s Interval
Temporal Logic over a Heyting algebra [[16](#16)], based on a work by Fitting [[17](#17)]. On the
other hand, there seem to be no attempts for a many-valued version of spatial logics.
We aim to introduce a possible many-valued extension for well-known temporal and
spatial logics based on the family of finite FLew-algebras [[18](#18)], allowing for a unified
treatment of both fuzzy logics and Heyting algebras, leveraging the notion of a many-
valued linear order and allowing for the definition of a many-valued semantics of modal
frames. This framework is also implemented as part of an open-source framework for
representing, reasoning, and learning from structured and unstructured data, namely
Sole.jl [[19](#19)], serving as the foundation for reasoning and learning tools leveraging many-
valued temporal and spatial logics.

## References
<a id="1">[1]</a> 
A. Pnueli.
The temporal logic of programs.
18th Annual Symposium on Foundations of Computer Science.
1977.

<a id="2">[2]</a> 
P. Blackburn and M. de Rijke and Y. Venema.
Modal Logic.
Journal of Logic and Computation.
Cambridge University Press.
2001.


<a id="3">[3]</a> 
M. Marx and M. Reynolds.
Undecidability of Compass Logic.
Journal of Logic and Computation.
Oxford University Press.
1999.

<a id="4">[4]</a> 
J. Y. Halpern and Y. Shoham.
A Propositional Modal Logic of Time Intervals.
Journal of the ACM.
vol. 38 (1991), no. 4, pp. 935-962.

<a id="5">[5]</a> 
C. Lutz and F. Wolter.
Modal Logics of Topological Relations. 
Logical Methods in Computer Science.
2006.

<a id="6">[6]</a> 
M. Baaz and N. Preining and R. Zach.
First-order Gödel logics.
Annals of Pure and Applied Logic.
vol. 147 (2007), pp. 23-47.

<a id="7">[7]</a> 
A. Rose.
Formalisations of further ℵ0-valued Łukasiewicz propositional calculi.
Journal of Symbolic Logic.
vol. 43 (1978), no. 2, pp. 207-210.

<a id="8">[8]</a> 
P. Hájek.
The Metamathematics of Fuzzy Logic.
Kluwer.
1998.

<a id="9">[9]</a> 
S. Dutta.
An event based fuzzy temporal logic.
Proc. of the 18th International Symposium on Multiple-Valued Logic.
1988.
pp. 64-71.

<a id="10">[10]</a> 
K. B. Lamine and F. Kabanza.
Using fuzzy temporal logic for monitoring behavior-based mobile robots.
Proc. of the IASTED International Conference, Robotics and Applications.
2000.
pp. 116-121.

<a id="11">[11]</a> 
H. Thiele and S. Kalenka.
On fuzzy temporal logic.
Proc. of the 2nd International Conference on Fuzzy Systems.
IEEE.
1993.
pp. 1027–-1032.

<a id="12">[12]</a> 
A. Frigeri and L. Pasquale and P. Spoletini.
Fuzzy Time in Linear Temporal Logic.
ACM Transactions on Computational Logic.
vol. 15 (2014), no. X, pp. 1-22.

<a id="13">[13]</a> 
W. Conradie and D. Della Monica and E. Muñoz-Velasco and G. Sciavicco.
An Approach to Fuzzy Modal Logic of Time Intervals.
Proc. of the 24th European Conference on Artificial Intelligence (ECAI).
vol. 325.
IOS Press.
2020.
pp. 696-703.

<a id="14">[14]</a> 
W. Conradie and D. Della Monica and E. Muñoz-Velasco and G. Sciavicco and I. E. Stan.
Fuzzy Halpern and Shoham's interval temporal logics.
Fuzzy Sets and Systems.
vol. 456 (2023), pp. 107-124.

<a id="15">[15]</a> 
W. Conradie and R. Monego and E. Muñoz-Velasco and G. Sciavicco and I. E. Stan.
A Sound and Complete Tableau System for Fuzzy Halpern and Shoham's Interval Temporal Logic.
Proc. of the 30th International Symposium on Temporal Representation and Reasoning (TIME).
vol. 278.
Schloss Dagstuhl.
2023.
pp. 9:1-9:14.

<a id="16">[16]</a> 
L. Esakia and G. Bezhanishvili and W. H. Holliday and A. Evseev.
Heyting Algebras: Duality Theory.
Springer.
2019.

<a id="17">[17]</a> 
M. Fitting.
Many-valued modal logics.
Fundamenta Informaticae.
vol. 15 (1991), no. 3-4, pp. 235-254.

<a id="18">[18]</a> 
P. Cintula and P. Hájek and C. Noguera.
Handbook of Mathematical Fuzzy Logic.
Studies in Logic. Mathematical Logic and Foundation.
College publications.
2011.

<a id="19">[19]</a> 
F. Manzella and G. Pagliarini and A. Paparella and G. Sciavicco and I. E. Stan.
Sole.jl – Symbolic Learning in Julia.
GitHub repository.
URL Address: https://github.com/aclai-lab/Sole.jl.
2025.
