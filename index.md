---
layout: page
title: Home
description: "BEAST collaboration develops solvated beyond-DFT methods for electrochemistry, accelerated by machine learning."
permalink: /
---

Computational modeling of electrochemistry is limited in accuracy by
1) the lack of a universal framework that efficiently treats arbitrary electrolytes, solvents and applied potentials with sufficient detail and fidelity to realistically and accurately model electrochemical systems, and
2) the deficiencies of density functional theory (DFT), the primary computational tool for reaction modeling, in describing charge transfer and reaction barriers. Accurate reaction barriers are crucial for connecting predictions to measured rates of chemical reactions, and quantum chemical techniques that may be accurate enough are not yet practicable for heterogeneous and electrocatalyst systems involving solid-liquid interfaces.

Funded by the DoE Computational Chemical Sciences program under DE-SC0022247 starting October 2021, the BEAST collaboration will address both challenges above by developing accurate and efficient exascale-ready solvated beyond-DFT methods.
The first ingredient in these methods are accurate atomic-scale electrolyte solvation models that capture the equilibrium effect of electrolyte in a single electronic structure calculation.
The second ingredient is the incorporation of GW many-body perturbation theory and the random phase approximation (RPA) total energy, which are accurate methods beyond DFT, into solvated and grand-canonical techniques to make them practicable for electrochemistry including solvation and bias effects.
Finally, in addition to optimizing these combined techniques for exascale computing, we will also make them more widely applicable using machine learning (ML) approaches trained to a beyond-DFT electrochemical database to make RPA-quality predictions at DFT cost.

## Team

+ Rensselaer Polytechnic Institute (PI: Ravishankar Sundararaman)
+ University of Colorado Boulder (PI: Charles Musgrave)
+ National Renewable Energy Laboratory (PI: Derek Vigil-Fowler)
+ University of South Carolina (PI: Christopher Sutton)
+ Lawrence Berkeley National Laboratory (PI: Mauro Del Ben)

## Software

+ [JDFTx](http://jdftx.org)
+ [BerkeleyGW](https://berkeleygw.org)
+ [QimPy](https://qimpy.org)

## News

{% for post in site.posts limit:3 %}
+ {{ post.date | date: "%b %-d, %Y" }}: [ {{ post.title }} ]( {{ post.url | prepend: site.baseurl }} )
{% endfor %}
+ [Older news](/news/)
