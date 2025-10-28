---
title: "Modal FLew-Algebra Satisfiability Through First-Order Translation"
collection: talks
type: "Conference talk"
permalink: /talks/2025-07-21-modal-flew-algebra-satisfiability-through-first-order-translation
excerpt: "In this work, we provide an accessible and open-source algorithmic tool for (i) defining finite FLew-algebras, (ii) writing formulas in a specified FLew-algebra, and (iii) asking alpha-satisfiability and alpha-validity for a given value alpha in the algebra of the formula through a first-order translation and making use of a sat or a smt solver, such as z3."
venue: "Logic, Algebra, and Truth Degrees (LATD 2025)"
date: 2025-07-21
location: "University of Siena, Siena, Italy"
slidesurl: 'http://alberto-paparella.github.io/files/LATD25_presentation.pdf'
---

Modal logics offer a valid treatment for temporal and spatial data, which are critical in modeling many real-world scenarios and, therefore, are becoming more popular by the day in artificial intelligence applications, specifically when dealing with symbolic machine learning. Some notable examples are [[1](#1)], [[2](#2)], introducing modal logics for treating interval temporal relations and topological (i.e., spatial) relations, respectively. However, practitioners handling temporal and spatial data typically encounter challenges, as sensing and discretizing signals that often introduce inaccuracies in the data. Fuzzy logics are renowned as a common approach to deal with uncertainty and unclear boundaries in the data. Furthermore, Melvin Fitting proposed in [[3](#3)] a many-valued approach leveraging Heyting algebras to tackle many-expert scenarios, another compelling application in artificial intelligence. In this talk, we want to present a framework that is general enough to treat modal many-valued logics, including Fitting's proposal, and can be endowed with reasoning tools suitable for real-world applications.

FLew-algebras (Full Lambek calculus with exchange and weakening, see, e.g.,[[4](#4)]) proved to be a valid candidate, as it generalizes most common algebraic structures of many-valued logics, such as Goedel algebras (G, for short) [[5](#5)], MV-algebras [[6](#6)] (MV) on which Łukasiewicz logic is based [[7](#7)], product algebras (Pi) [[8](#8)], and Heyting algebras (H).
FLew-algebras are bounded integral commutative residuated lattices; i.e., an FLew-algebra A is a lattice ordered by a partial ordering relation <=, with a top (1) and a bottom (0) element. When the order is linear, we use the term FLew-chain. The difference between FLew-algebras and common bounded lattices is the presence of an internal operation, usually denoted by  o, and assumed to be commutative, associative and having 1 as a neutral element, usually referred to as t-norm, that is, such that (A,  o,1) is a monoid; hence, we will often refer to the multiplication as the monoidal operation. Intuitively, the multiplication in an FLew-algebra generalizes the interpretation of the logical conjunction. Moreover, an FLew-algebra is assumed to have the residuation property, that is, it is assumed that for fixed elements a,b in A, there exists a unique maximal element x such that a o x <=> b; this element is denoted by a -> b, and the implication operator  -> generalizes the logical implication. All commonly used algebras in the field of many-valued logics are particular cases of some FLew-algebra (A, o, ->,1,0); each specific case differs from the others in how the monoidal operation is defined. 

While modal many-valued logics [[3](#3)], [[9](#9)] have already been applied in different contexts, they are just starting to be studied in depth.
Automated theorem proving for modal FLew-algebra formulas encompassing a many-valued generalization of Halpern and Shoham's interval temporal logic [[1](#1)] has been tackled in [[10](#10)] using a tableaux system inspired by the one proposed by Melvin Fitting in [[11](#11)] and already extended to Heyting Algebras in [[12](#12)].
When tackling formulas satisfiability and validity in FLew-algebras (and, more generally, many-valued logics defined over a lattice representing a partial order), the problem can be relaxed to finding, given a formula  f and a value alpha in the algebra, if a model exists such that (resp., for all possible models) the formula has at least value alpha. This problem is referred to alpha-satisfiability (resp.alpha-validity).

In this work, we propose a different approach leveraging well-known sat and smt solvers, such as z3, with the hope of gaining better performance while maintaining some sort of interpretability. In order to do so, one has to translate the alpha-satisfiability problem to a two-sorted first-order problem, with a first sort A representing the values in the FLew-algebra and a second sort W representing the worlds, such that given a formula  f interpreted on an FLew-algebra A,  f is alpha-satisfiable if and only if it exists M,w inW so that V_M(w,a)>=alpha.

We provide an accessible and open-source algorithmic tool for (i) defining finite FLew-algebras, (ii) writing formulas in a specified FLew-algebra, and (iii) asking alpha-satisfiability %and alpha-validity
for a given value alpha in the algebra of the formula through a first-order translation and making use of a sat or a smt solver, such as z3. This tool is offered as part of a long-term open-source framework for learning and reasoning, namely [Sole.jl](https://github.com/aclai-lab/Sole.jl). In particular, the tool can be found in the ManyValuedLogics submodule of the [SoleLogics.jl](https://github.com/aclai-lab/SoleLogics.jl) package, which provides the core data structures and functions for an easy manipulation of propositional, modal and many-valued logics. For the benefit the reader, the tool is also available in a [standalone repository](https://github.com/aclai-lab/LATD2025b), using many-valued Halpern and Shoham's interval temporal logic as an example.

## References
<a id="1">[1]</a> 
J. Y. Halpern and Y. Shoham.
A Propositional Modal Logic of Time Intervals.
Journal of the ACM.
vol. 38 (1991), no. 4, pp. 935-962.

<a id="2">[2]</a> 
C. Lutz and F. Wolter.
Modal Logics of Topological Relations.
Logical Methods in Computer Science.
vol. 2 (2006), no. 2.

<a id="3">[3]</a> 
M. Fitting.
Many-valued modal logics.
Fundamenta Informaticae.
vol. 15 (1991), no. 3-4, pp. 235-254.

<a id="4">[4]</a> 
N. Galatos.
Residuated lattices: an algebraic glimpse at substructural logics.
Elsevier.
2007.

<a id="5">[5]</a> 
M. Baaz and N. Preining and R. Zach.
First-order Gödel logics.
Annals of Pure and Applied Logic.
vol. 147 (2007), pp. 23-47.

<a id="6">[6]</a> 
C. C. Chang.
Algebraic analysis of many valued logics.
Transactions of the American Mathematical society.
vol. 88 (1958), no. 2, pp. 467-490.

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
W. Conradie and D. Della Monica and E. Muñoz-Velasco and G. Sciavicco and I. E. Stan.
Fuzzy Halpern and Shoham's interval temporal logics.
Fuzzy Sets and Systems.
vol. 456 (2023), pp. 107-124.

<a id="10">[10]</a> 
G. Badia and C. Noguera and A. Paparella and G. Sciavicco and I. E. Stan.
Fitting’s Style Many-Valued Interval Temporal Logic Tableau System: Theory and Implementation.
31st International Symposium on Temporal Representation and Reasoning (TIME 2024).
vol. 318 (2024), pp. 1-16.

<a id="11">[11]</a> 
M. Fitting
Tableaus for many-valued modal logic.
Studia Logica.
vol. 55 (1995), pp. 63-87.

<a id="12">[12]</a> 
W. Conradie and R. Monego and E. Muñoz-Velasco and G. Sciavicco and I. E. Stan.
A Sound and Complete Tableau System for Fuzzy Halpern and Shoham's Interval Temporal Logic.
Proc. of the 30th International Symposium on Temporal Representation and Reasoning (TIME).
vol. 278.
Schloss Dagstuhl.
2023.
pp. 9:1-9:14.
