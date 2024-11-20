---
title: "Reasoning with many-valued interval temporal logic"
collection: talks
type: "Conference proceedings talk"
permalink: /talks/2024-11-28-reasoning-with-many-valued-interval-temporal-logic
venue: "Australasian Association for Logic Conference 2024"
date: 2024-11-28
location: "University of Sydney, Sydney, New South Wales, Australia"
slidesurl: 'http://alberto-paparella.github.io/files/AAL24_presentation.pdf'
---

[More information here](https://sites.google.com/view/aalogic/aal-conference-2024)

Unlike classical logic, which is grounded in the Boolean two-valued algebra, many-
valued logics involve a more complex algebraic framework, thereby supporting a richer
set of truth values. Such generalization has led to the development of a sophisticated
algebraic taxonomy, accommodating different types of underlying domains and the
properties of algebraic operators, which in turn influences the interpretation of logical
connectives [[1](#1)]. Noteworthy examples include Gödel algebras (G) [[2](#2)], MV-algebras [[3](#3)]
on which Lukasiewicz logic is based [[4](#4)], product algebras (Π) [[5](#5)], and Heyting algebras
(H) on which intuitionistic logic is based [[6](#6)].

Standard (i.e., based on algebras whose lattice reduct is the interval [0, 1] in R)
fuzzy logics (which can be seen as a sub-class of many-valued logics) are crucial in sev-
eral mathematics and computer science areas, particularly within artificial intelligence.
These logics are predominantly employed in rule-based classifier learning [[7](#7)], to enhance
the flexibility and expressive power of classical systems, but also to refine decision-tree
classifiers by supporting more granular decision-making processes [[8](#8)]. In the context
of subsymbolic machine learning, they find their use in fuzzy neural networks, aid-
ing in managing the inherent uncertainty in data improving network adaptability and
performance [[9](#9)].

In terms of temporal logic, only a few attempts have been made to study point-based
temporal languages in the fuzzy case, with early contributions [[10](#10), [11](#11), [12](#12)] that limited
to the fuzzification of the propositional side of formulas, while [[13](#13)] provide a generaliza-
tion of LTL allowing to express uncertainty in both atomic propositions and temporal
relations. While standard algebras are relatively common in practical applications, the
practical necessity for an infinite set of truth values is often debatable; for example,
in the context of machine learning, datasets contain only a finite number of distinct
values, giving rise to a finite number of distinct situations. At the same time, the
conventional reliance on chain algebras can restrict modeling capabilities, disallowing
the possibility of reasoning about different and incomparable experts’ viewpoints. A
more general approach to many-valued modal (and therefore temporal) logics is that of
Fitting [[14](#14)]. In the case of interval temporal logic, [[15](#15), [16](#16), [17](#17)] introduced and studied
a many-valued extension of Halpern and Shoham’s interval temporal logic (HS [[18](#18)])
over a Heyting algebra, providing a tableau system for it in the case of finite algebras.

In this work, we explore a further generalization of HS based on FLew -algebras [[1](#1)].
An FLew -algebra is defined over a bounded commutative integral residuated lattice
and naturally generalizes several common frameworks, including G, MV, Π, and H. To
uniform the terminology, we shall use the term Many-Valued Halpern and Shoham’s
interval temporal logic (MVHS). We extend Fitting’s tableau system to deal with MVHS
over some finite FLew -algebra, we provide a working implementation for it as a part of
our open-source reasoning and learning framework, and we test it to assess its practical
usefulness.

## References
<a id="1">[1]</a> 
P. Cintula and P. Hájek and C. Noguera.
Handbook of Mathematical Fuzzy Logic.
Studies in Logic. Mathematical Logic and Foundation.
College publications.
2011.

<a id="2">[2]</a> 
M. Baaz and N. Preining and R. Zach.
First-order Gödel logics.
Annals of Pure and Applied Logic.
vol. 147 (2007), pp. 23-47.

<a id="3">[3]</a> 
C. C. Chang.
Algebraic analysis of many valued logics.
Transactions of the American Mathematical society.
vol. 88 (1958), no. 2, pp. 467-490.

<a id="4">[4]</a> 
A. Rose.
Formalisations of further ℵ0-valued Łukasiewicz propositional calculi.
Journal of Symbolic Logic.
vol. 43 (1978), no. 2, pp. 207-210.

<a id="5">[5]</a> 
P. Hájek.
The Metamathematics of Fuzzy Logic.
Kluwer.
1998.

<a id="6">[6]</a> 
L. Esakia and G. Bezhanishvili and W. H. Holliday and A. Evseev.
Heyting Algebras: Duality Theory.
Springer.
2019.

<a id="7">[7]</a> 
L. I. Kuncheva.
Fuzzy Classifier Design.
Studies in Fuzziness and Soft Computing.
Springer.
2000.

<a id="8">[8]</a> 
Y. Chen and T. Wang and B. Wang and Z. Li.
A Survey of Fuzzy Decision Tree Classifier.
Fuzzy Information and Engineering.
vol. 1 (2009), no. 2, pp. 149-159.

<a id="9">[9]</a> 
J. J. Buckley and Y. Hayashi.
Fuzzy neural networks: A survey.
Fuzzy Sets and Systems.
vol. 66 (1994), pp. 1-13.

<a id="10">[10]</a> 
S. Dutta.
An event based fuzzy temporal logic.
Proc. of the 18th International Symposium on Multiple-Valued Logic.
1988.
pp. 64-71.

<a id="11">[11]</a> 
K. B. Lamine and F. Kabanza.
Using fuzzy temporal logic for monitoring behavior-based mobile robots.
Proc. of the IASTED International Conference, Robotics and Applications.
2000.
pp. 116-121.

<a id="12">[12]</a> 
H. Thiele and S. Kalenka.
On fuzzy temporal logic.
Proc. of the 2nd International Conference on Fuzzy Systems.
IEEE.
1993.
pp. 1027–-1032.

<a id="13">[13]</a> 
A. Frigeri and L. Pasquale and P. Spoletini.
Fuzzy Time in Linear Temporal Logic.
ACM Transactions on Computational Logic.
vol. 15 (2014), no. X, pp. 1-22.

<a id="14">[14]</a> 
M. Fitting.
Many-valued modal logics.
Fundamenta Informaticae.
vol. 15 (1991), no. 3-4, pp. 235-254.

<a id="15">[15]</a> 
W. Conradie and D. Della Monica and E. Muñoz-Velasco and G. Sciavicco.
An Approach to Fuzzy Modal Logic of Time Intervals.
Proc. of the 24th European Conference on Artificial Intelligence (ECAI).
vol. 325.
IOS Press.
2020.
pp. 696-703.

<a id="16">[16]</a> 
W. Conradie and D. Della Monica and E. Muñoz-Velasco and G. Sciavicco and I. E. Stan.
Fuzzy Halpern and Shoham's interval temporal logics.
Fuzzy Sets and Systems.
vol. 456 (2023), pp. 107-124.

<a id="17">[17]</a> 
W. Conradie and R. Monego and E. Muñoz-Velasco and G. Sciavicco and I. E. Stan.
A Sound and Complete Tableau System for Fuzzy Halpern and Shoham's Interval Temporal Logic.
Proc. of the 30th International Symposium on Temporal Representation and Reasoning (TIME).
vol. 278.
Schloss Dagstuhl.
2023.
pp. 9:1-9:14.

<a id="18">[18]</a> 
J. Y. Halpern and Y. Shoham.
A Propositional Modal Logic of Time Intervals.
Journal of the ACM.
vol. 38 (1991), no. 4, pp. 935-962.