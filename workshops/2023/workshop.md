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

[Register here](https://forms.gle/RjRBjWBvpH18BB977).

## Announcement

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

## Tentative Agenda

### Day 1: Thursday, August 17, 2023

+ **9:00 am PDT** Welcome, introduction to BEAST
+ **9:10 am PDT** Introduction to Joint Density-Functional Theory (JDFT)
+ **9:45 am PDT** JDFT calculations in practice with JDFTx code
+ **10:00 am PDT** Introduction to the QimPy code
+ **10:15 am PDT** Practical DFT session I: molecules and solids (JDFTx/QimPy options)
+ **12:00 pm PDT** Break for lunch
+ **1:00 pm PDT**  Practical DFT session II: surfaces and adsorbates (JDFTx/QimPy options)
+ **3:00 pm PDT**  Practical DFT session III: transition states (JDFTx/QimPy options)
+ **5:00 pm PDT** Adjourn

### Day 2: Friday, August 18, 2023

+ **9:00 am PDT** Introduction to JDFT+RPA: Theory and applications
+ **9:30 am PDT** JDFT+RPA calculations in practice with JDFTx+BGW
+ **10:00 am PDT**
   - **Option 1**: Continue Practical DFT sessions II and III
   - **Option 2**: Practical JDFTx+BGW session for adsorption energies
   - **Option 3**: Introduction to QimPy for developers
+ **12:00 pm PDT** Break for lunch
+ **1:00 pm PDT** BEAST DB: preview and opportunity for community contributions
+ **2:00 pm PDT** 
   - **Option 1**: Using BEAST DB for electrocatalysis
   - **Option 2**: Continue JDFTx+BGW session for adsorption energies
   - **Option 3**: Continue QimPy developer's session
+ **4:00 pm PDT** Panel discussions, Q&amp;A, feature requests
+ **5:00 pm PDT** Adjourn 
