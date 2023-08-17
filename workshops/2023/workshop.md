---
layout: page
navtitle: Workshops
title: 2nd BEAST Workshop, 2023
description: "Second annual BEAST workshop"
permalink: /workshops/2023/
---

# 2nd BEAST Workshop, 2023

<b>August 17 - 18, 2023, 9 am - 5 pm PDT</b> in hybrid in-person/online mode at:

+ Cal State East Bay Oakland Center, Oakland, CA, USA, and
+ Online (on Zoom)


## Tentative Agenda

Please review [Setup instructions](setup) before / at the start of the workshop.

### Day 1: Thursday, August 17, 2023

+ **9:00 am PDT** [Welcome, introduction to BEAST](beast.pdf)
+ **9:10 am PDT** [Introduction to Joint Density-Functional Theory (JDFT)](jdft.pdf)
+ **9:45 am PDT** [JDFT calculations in practice with JDFTx (and a QimPy intro)](jdftx.pdf)
+ **10:00 am PDT** Practical DFT session I: molecules and solids
+ **12:00 pm PDT** Break for lunch
+ **1:00 pm PDT**  Practical DFT session II: surfaces and adsorbates
+ **3:00 pm PDT**  Practical DFT session III: transition states
+ **5:00 pm PDT** Adjourn

### Day 2: Friday, August 18, 2023

+ **9:00 am PDT** Introduction to JDFT+RPA: Theory and applications
+ **9:30 am PDT** JDFT+RPA calculations in practice with JDFTx+BGW
+ **10:00 am PDT**
   - **Option 1**: Practical JDFTx+BGW session for adsorption energies
   - **Option 2**: Continue Practical DFT sessions II and III
+ **12:00 pm PDT** Break for lunch
+ **1:00 pm PDT** BEAST DB: preview and opportunity for community contributions
+ **2:00 pm PDT** 
   - **Option 1**: QimPy preview and development overview
   - **Option 2**: Continue JDFTx+BGW session for adsorption energies
+ **4:00 pm PDT** Panel discussions, Q&amp;A, feature requests
+ **5:00 pm PDT** Adjourn 

### Tutorial files

The code setup on NERSC for the tutorials and the inputs should remain accessible
to any one with a NERSC account even after the end of the workshop.
However, you may need to modify batch scripts to remove the reservation / change the account.

We have also bundled all the tutorial instructions and input files for download as
[Calculations-clean.tbz2](Calculations-clean.tbz2) to your own computing resource.
You will need to setup JDFTx, BerkeleyGW and GCNEB to work through these tutorials there,
and modify the batch scripts / set up your own interactive sessions as appropriate.
Additionally, to run the visualization notebooks, you will need to place
this custom python package, [ase_ext.tbz2](ase_ext.tbz2), in your PYTHONPATH
within an environment that includes the `ase` and `scikit-image` packages.


## Original announcement

[Register here](https://forms.gle/RjRBjWBvpH18BB977).

We are excited to announce the 2nd Annual BEAST (Beyond-DFT Electrochemistry with Accelerated and Solvated Techniques) Workshop.
This BEAST workshop will include hands-on user sessions on simulation methods best suited for studying electrocatalysis.
The methods will include grand-canonical DFT (GC-DFT) with the latest solvation methods implemented in the JDFTx and/or QimPy computational packages, beyond-DFT random phase approximation (RPA) calculations in the BerkeleyGW package, and an exposure to our soon to be released GC-DFT electrocatalysis database, BEAST DB.
The target participants for the Workshop are graduate students, postdocs, and researchers who are interested in learning about or sharpening their skills on ab initio calculations of electrocatalytic systems, including the effect of solvation, self-consistent applied potential and beyond-DFT exchange-correlation effects.
This second workshop will once again start from basics, but provide options for more advanced calculations, building on last year's workshop. 

The [JDFTx package](https://jdftx.org) is a plane-wave density functional theory (DFT) code that calculates the electronic properties of optoelectronic and electrocatalytic systems, with a particular strength in describing solvated system under applied bias. JDFTx supports a range of exchange correlation functionals, dispersion corrections, several formats of norm-conserving and ultrasoft pseudopotentials that are pre-installed, and calculations of systems of any dimensionality from 0 to 3: molecules, wires, slabs / 2D materials and bulk.
The [QimPy package](https://qimpy.org) is the next iteration of JDFTx, rewritten from scratch in Python with PyTorch to more easily take advantage of a diverse set of accelerators and to further ease development. 
This workshop will cover exercises in both JDFTx and QimPy, leveraging JDFTx for mature features and introducing QimPy for its greater scalability and future ease of use.
The [BerkeleyGW Package](https://berkeleygw.org) calculates the electronic structure and total energies of electrocatalytic systems at the RPA level in this context.
The Workshop will introduce the basic theory of solvation, GC-DFT and RPA, standard and new features of the JDFTx and BerkeleyGW packages, with detailed examples of using the JDFTx and BerkeleyGW packages.
Finally, we will also introduce development in the new QimPy code and solicit community involvement in it's continued development.
