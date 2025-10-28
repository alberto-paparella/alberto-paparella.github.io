---
title: "Symbolic Learning and Rule Extraction with Sole.jl"
collection: talks
type: "Conference talk"
permalink: /talks/2025-10-02-symbolic-learning-and-rule-extraction-with-sole
venue: "JuliaCon Local Paris 2025"
date: 2025-10-02
location: "Paris, France"
slidesurl: http://alberto-paparella.github.io/files/JuliaConLocal25_presentation.pdf
---

[Check it on youtube](https://www.youtube.com/watch?v=JVHeIdVPK8Y)

**Symbolic learning** is a branch of **machine learning** that studies algorithms for building **symbolic models**, classifiers that can be translated to **logical rules**. Hence, differently from neural networks and other statistical models, symbolic models are more easily readable and interpretable. Common examples include **decision trees** and their ensemble counterpart, **random forests**.

**Sole.jl** is a Julia package for symbolic learning and rule extraction, aimed at guiding the user throughout the whole process, from the initial **data** to learning a symbolic **model**, to the extraction and manipulation of logical **rules** from such model.

It is also the entry point to the **SOLE** framework (which stands for **S**ymb**O**lic **LE**arning), an open-source project fully developed in Julia, serving as an interface to both its main packages, such as **SoleData.jl**, **SoleModels.jl**, **SolePostHoc.jl**, as well as useful packages developed by the learning community, such as **DecisionTree.jl**, **ModalDecisionTrees.jl**, **ModalAssociationRules.jl**, **MLJ.jl**, **XGBoost.jl**, and so on.

For instance, given a dataset, one can use **Sole.jl** to fit a **decision tree** model, provided by the **DecisionTree.jl** package, and then extract and eventually manipulate rules from such model through the **SolePostHoc.jl** package. Furthermore, if working with more non-tabular data like images or time-series, one can leverage the **SoleData.jl** package to interpret the dataset as a set of logical interpretations of a more-than propositional logic (e.g., interval or rectangle modal logic) and use a learning package compatible with such logic, such as **ModalDecisionTrees.jl** or **ModalAssociationRules.jl**.

In this presentation, we will have a look at how **Sole.jl** works through a hands-on tutorial, emphatizing on its comprehensiveness and user-friendliness. This will also allow us to introduce two newcomers to the **SOLE**  ecosystem: **ModalAssociationRules.jl**, a package for mining association rules between instances, and **SolePostHoc.jl**, a package to extract, interpret and simplify sets of rules starting from a symbolic model.
