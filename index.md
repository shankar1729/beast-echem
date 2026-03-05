---
layout: page
title: Home
description: "BEAST collaboration develops solvated beyond-DFT methods for electrochemistry, accelerated by machine learning."
permalink: /
---

Computational modeling of electrochemistry is limited in accuracy by
1) the lack of a universal framework that efficiently treats arbitrary electrolytes, solvents and applied potentials with sufficient detail and fidelity to realistically and accurately model electrochemical systems, and
2) the deficiencies of density functional theory (DFT), the primary computational tool for reaction modeling, in describing charge transfer and reaction barriers.
Accurate reaction barriers are crucial for connecting predictions to measured rates of chemical reactions, and quantum chemical techniques that may be accurate enough are not yet practicable for heterogeneous and electrocatalyst systems involving solid-liquid interfaces.

Funded by the DoE Computational Chemical Sciences program under DE-SC0022247 since October 2021, the BEAST collaboration is addressing both challenges above by developing accurate and efficient exascale-ready solvated beyond-DFT methods, including:

+ [Accurate atomic-scale electrolyte solvation models](/thrust1) that capture the equilibrium effect of electrolyte in a single electronic structure calculation.
+ GW many-body perturbation theory and the [random phase approximation (RPA) total energy](/thrust2), which are accurate methods beyond DFT, into solvated and grand-canonical techniques to make them practicable for electrochemistry including solvation and bias effects.
+ Machine learning (ML) approaches trained to a beyond-DFT electrochemical database, [BEAST DB](https://beast-echem.org/beastdb) to [make RPA-quality predictions at DFT cost](/thrust3) in order to make high-quality predictions based on the exascale methods more widely accessible to the community.

The BEAST team conducts [annual workshops](/workshops) that introduce the most recent techniques for accurate first-principles electrochemistry, starting from a beginner's level on each of the software tools being developed as a part of this project.

<img alt="Institute logos" width="100%" src="/images/institutes.jpg"/>

## Team

+ Rensselaer Polytechnic Institute (PI: Ravishankar Sundararaman)
+ University of Colorado Boulder (PI: Charles Musgrave)
+ National Renewable Energy Laboratory (PI: Derek Vigil-Fowler)
+ University of South Carolina (PI: Christopher Sutton)
+ Lawrence Berkeley National Laboratory (PI: Mauro Del Ben)

## Software

The techniques developed by the BEAST team are available through the following open-source software projects.

<table>
<tr>
<th style="width: 25%">
<a href="http://jdftx.org"><img alt="JDFTx" width="50%" src="/images/jdftx.png"/></a>
</th>
<th style="width: 50%">
<a href="https://berkeleygw.org"><img alt="BerkeleyGW" width="80%" src="/images/bgw.png"/></a>
</th>
<th style="width: 25%">
<a href="https://qimpy.org"><img alt="QimPy" width="80%" src="/images/qimpy.png"/></a>
</th>
</tr>
</table>


## News

{% for post in site.posts limit:3 %}
+ {{ post.date | date: "%b %-d, %Y" }}: [ {{ post.title }} ]( {{ post.url | prepend: site.baseurl }} )
{% endfor %}
+ [Older news](/news/)
