# Kinetic-Mechanisms
![Logo](.images/intro.svg)

Kinetic Mechanisms for gas, liquid and solid fuels, current version CRECK_2003.
All the mechanisms are freely available in CHEMKIN format (compatible with version 3.6.2 and above) and 
are self-consistent, i.e. they contain smaller subsets and can be coupled together. 
Most of the mechanisms are available with or without NOx and soot submodules.
Please contact us at creckmodeling-dcmc@polimi.it for questions and comments. 
In-depth descriptions of each mechanisms are available on the [creck website](http://creckmodeling.chem.polimi.it/),
while briefy summaries are reported in each subfolder.

## Choice of Kinetic Mechanism
The kinetic mechanism are organized according to the reactant-phase:
- [Homogeneous Gas-Phase](Gas-Phase) mechanisms address the reactivity of hydrogen, ammonia, gasolines, diesel, etc. 
    Each of them can be also coupled to the other phase kinetics to study secondary gas-phase reactions. 
    To aid in choosing the proper kinetic mechanism, refer to the gas-phase [readme subsection](Gas-Phase/README.md#Choice-Kinetic-Mechanism)
- [Liquid-Phase](Liquid-Phase) mechanisms address decompositio of heavy fuels which degrade before evaporating (e.g. [HFO](Liquid-Phase/HeavyFuelOil)). 
    [Plastics](Liquid-Phase/Plastics) are considered as liquids as their degradation occurs in the molten state. 
- [Solid-Phase](Solid-Phase) mechanisms address decomposition of solid fuels, i.e. [Biomass](Solid-Phase/Biomass) and [Coal](Solid-Phase/Coal). 
    As discussed in the readme file, the biomass model can be coupled to gas-phase subsets.
- [Heterogeneous-Surface](Heterogeneous-Mechanisms) mechanisms are heterogeneous surface models for a broad range of applications, 
    e.g. [pyrocarbon deposition](Surface-Mechanisms/CVI-CVD) and [biochar oxidation](Surface-Mechanisms/Char)  
    
All the files reported are text-files with "fake" modifiable extensions. Nevertheless, the following extensions are employed:
- gas kinetics are identified either by ".CKI" or ".gas" 
- liquid kinetics are identified by ".liquid"
- solid kinetics are identified by ".solid"
- surface kinetics are identified by ".surface"
- thermodynamic files are identified by ".CKT", "thermo", or ".dat"
- transport files are identified by ".tra" or ".TRAN" 

## OpenSMOKE++ Suite: numerical simulations of kinetic mechanisms
Do you need to simulate ideal reactors or laminar 1D flames? 
Why don't you try the [OpenSMOKE++ Suite](https://www.opensmokepp.polimi.it/) from CRECK Modeling Lab? 
The OpenSMOKE++ Suite is a collection of standard solvers for modeling the typical 
systems of interest in developing and testing detailed kinetic mechanisms 
(including thousands of species and reactions).
The software is user-friendly, fast and free for academic users.
Contact us at creckmodeling-dcmc@polimi.it if you are interested.

OpenSMOKE++ is a general framework developed by the CRECK Modeling Lab for 
numerical simulations of reacting systems with detailed kinetic mechanisms, 
including thousands of chemical species and reactions.
OpenSMOKE++ can handle simulations of ideal reactors, shock-tubes, rapid compression machines, 
1D laminar flames and multidimensional reacting systems, and it provides useful numerical tools 
such as the sensitivity and rate of production analyses.
OpenSMOKE++ is distributed in three main packages:
- [OpenSMOKE++ Suite](https://www.opensmokepp.polimi.it/index.php?option=com_content&view=article&id=299:article-ospp&catid=106&Itemid=765): 
    simulation of ideal reactors (batch, plug-flow, perfectly stirred reactors), 
    shock-tubes, rapid compression machines, laminar 1D flames (freely propagating 
    and burner stabilized flames, counter-flow diffusion flames)
- [OpenSMOKE++4OpenFOAM](https://www.opensmokepp.polimi.it/index.php?option=com_content&view=article&id=301:article-ospp4of&catid=106&Itemid=766):
    solvers for steady-state and unsteady reacting flows in arbitrarly complex 
    multidimensional geometries with detailed kinetic mechanisms (based on OpenFOAM)
- [DoctorSMOKE++](https://www.opensmokepp.polimi.it/index.php?option=com_content&view=article&id=300:article-doctorsmokepp&catid=106&Itemid=767):
    automatic reduction of detailed kinetic mechansims to a skeletal level, to 
    allow their use in large scale CFD simulations.
