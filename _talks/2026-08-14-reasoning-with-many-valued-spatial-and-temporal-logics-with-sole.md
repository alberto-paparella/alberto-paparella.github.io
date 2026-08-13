---
title: "Reasoning with Many-Valued, Spatial and Temporal Logics with SOLE"
collection: talks
type: "Conference talk"
permalink: /talks/2026-08-14-reasoning-with-many-valued-spatial-and-temporal-logics-with-sole
excerpt: "Reasoning with temporal and spatial data is crucial in many real-world applications; however, this data is often characterized by uncertainty and unclear boundaries. In this talk, we will see how we can extend spatial and temporal modal logics offered by SOLE through a new submodule, namely ManyValuedLogics, offering support for fuzzy and many-valued logics. Moreover, we will explore a new package called SoleReasoners.jl, offering a reasoning tool for many-valued spatial and temporal logics."
date: 2026-08-14
location: "Johannes Gutenberg University, Mainz, Germany"
slidesurl: 'http://alberto-paparella.github.io/files/JuliaCon26_presentation.pdf'
---

Many real-world applications make use of temporal and spatial data, and reasoning is among the most important tasks, allowing to solve problems spanning from scheduling, to monitoring, up to predicting future scenarios. However, this data is often characterized by uncertainty and unclear boundaries (e.g., due to sensoring and discretization), challenges usually tackled with the use of fuzzy logics.
SoleLogics.jl offers a new submodule, namely ManyValuedLogics, allowing for the treatment of continuous fuzzy logics and finite many-valued logics, definable over their algebraic counterpart up to FLew-algebras. In this talk, we will see through practical examples how we can make use of this new machinery, together with multi-modal logics already offered by SoleLogics.jl to treat spatial and temporal information (e.g., Linear Temporal Logic, Compass Logic, Halpern and Shoham’s Interval Temporal Logic, Lutz and Wolter’s Logic of Topological Relations), to model real world scenarios with more accuracy.
Icing on the cake, SoleReasoners.jl is a new package in the SOLE framework offering a reasoning tool, based on analytic tableau technique, to solve satisfiability and validity for many-valued spatial and temporal logics (the first specialized implementation at this level of generality that we know of!), and we will see how we can make use of it when dealing with logics carrying both a many-valued and a multi-modal component.
