---
title: "Assessing the (In)Ability of LLMs to Reason in Interval Temporal Logic"
collection: publications
category: conferences
status: accepted
permalink: /publication/2025-08-27-assessing-the-inability-of-llms-to-reason-in-interval-temporal-logic
excerpt: 'In this paper, we tackle the problem of assessing the ability of LLMs to reason about interval-based statements in the form
of validity recognition.'
date: 2025-08-27
venue: '32nd International Symposium on Temporal Representation and Reasoning (TIME 2025), London, UK, 27-29 August 2025'
paperurl: https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.TIME.2025.4
citation: 'Bellodi, Pietro, Casavecchia, Pietro, Paparella, Alberto, Sciavicco, Guido, and Stan, Eduard I. (2025). &quot;Assessing the (In)Ability of LLMs to Reason in Interval Temporal Logic.&quot; <i>32nd International Symposium on Temporal Representation and Reasoning (TIME 2025), London, UK, 27-29 August 2025</i>. 1(1).'
---

The logical reasoning skills of Large Language Models (LLMs) is poorly understood and often over-
stated. Current evaluation suites rely on algebraic or commonsense puzzles that mix reasoning with
symbolic manipulation and/or provide static datasets that quickly saturate or leak into pretraining
corpora. In purely logical terms, the most relevant reasoning skill is the meta-mathematical task
of valid formula recognition, which is at the foundation of higher-level reasoning tasks (including
deduction and minimization of assertions, to name just a few). In the current landscape of LLMs
benchmarking, puzzles are most often stated in propositional or first-order logic, with a few ex-
ceptions for point-based temporal logic, such as LTL; yet, in the real world, event-based temporal
statements are prevalent, and they are more naturally expressed in interval-based temporal logic.
Interval temporal logic offers a much richer (w.r.t. point-based temporal logic, for example) variety
of problems, and not only do different languages present different expressive powers, but also the
computational complexity of the validity problem can vary widely. In this paper, we tackle the
problem of assessing the ability of LLMs to reason about interval-based statements in the form
of validity recognition. We explore whether their accuracy is sensible to the underlying language,
the computational complexity of the associated validity problem, and the intrinsic hardness of the
problem in terms of formula length and modal depth of the problem. We benchmark several frontier
LLMs (Gemma 3 27b It, Llama 4 Maverick, DeepSeek Chat V3 release 0324, Qwen 3 32b, and Qwen
3 235b) and show that, despite apparently impressive performance on algebraic or commonsense
benchmarks, they falter on logically rigorous tasks.
