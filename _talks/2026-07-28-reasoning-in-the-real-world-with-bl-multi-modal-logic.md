---
title: "Reasoning in the real world with BL multi-modal logic"
collection: talks
type: "Conference talk"
permalink: /talks/2026-07-28-reasoning-in-the-real-world-with-bl-multi-modal-logic
excerpt: "With the aim of modeling real world scenarios through spatial and temporal data, but also taking uncertainty into account, we employ a many-valued extension for well-known temporal and spatial logics based on Basic Fuzzy Logic (BL), introduced by Petr Hájek. We also present an automated reasoning system, based on analytic tableau technique, allowing to solve classical problems like satisfiability, validity, equivalence and entailment with many-valued temporal and spatial logics compliant with the proposed framework. This framework, together with the described reasoning tool, is also implemented in the Julia programming language as part of an open-source package for representing, reasoning, learning and post-hoc analysis from structured and unstructured data, namely Sole.jl"
date: 2026-07-28
location: "Jagiellonian University, Krakow, Poland"
slidesurl: 'http://alberto-paparella.github.io/files/TACL26_presentation.pdf'
---

Many real-world applications make use of temporal and spatial data. Reasoning with
this kind of data is crucial to solve many problems, from monitoring, to scheduling, up
to predicting future scenarios. Unsurprisingly, the literature is abundant in multi-modal
temporal and spatial logic approaches leveraging modal operators to treat the relations
between points in time (Linear Temporal Logic) and space (Compass Logic), or
even time intervals (Halpern and Shoham’s Interval Temporal Logic) or areas in an
image (Lutz and Wolter’s Logic of Topological Relations).
However, most of the time, these applications live in scenarios characterized by uncetainty and vagueness in the data due to many factors, including sensoring, discretization,
and so on. Classically, this problem is tackled using continuous t-norms fuzzy logics such
as Gödel logic (G), Lukasiewic logic (L), and Product logic (Π).
With the aim of modeling real world scenarios through spatial and temporal data, but
also taking uncertainty into account, we employ a many-valued extension for well-known
temporal and spatial logics based on Basic Fuzzy Logic (BL), introduced by Petr Hájek.
In order to do so, we will leverage the notion of a many-valued linear order, allowing for
the definition of a many-valued semantics of modal frames.
We also present an automated reasoning system, based on analytic tableau technique,
allowing to solve classical problems like satisfiability, validity, equivalence and entailment
with many-valued temporal and spatial logics compliant with the proposed framework.
Furthermore, we define a relaxation of the satisfiability problem, namely α-satisfiability, to
inquiry if a model evaluates a formula to a grade greater than a specific value α. 
This framework, together with the described reasoning tool, is also implemented in the
Julia programming language as part of an open-source package for representing, reasoning,
learning and post-hoc analysis from structured and unstructured data, namely Sole.jl.