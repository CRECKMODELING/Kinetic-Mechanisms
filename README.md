# Kinetic-Mechanisms
![Logo](.images/intro.svg)

Kinetic Mechanisms for gas, liquid and solid fuels, current version CRECK_2003.
All the mechanisms are freely available in CHEMKIN format (compatible with version 3.6.2 and above) and 
are self-consistent, i.e. they contain smaller subsets and can be coupled together. 
Most of the mechanisms are available with or without NOx and soot submodules.
Please contact us at creckmodeling-dcmc@polimi.it for questions and comments. 
In-depth descriptions of each mechanism are available on the [creck website](http://creckmodeling.chem.polimi.it/),
while briefy summaries are reported in each subfolder.

## Choice of Kinetic Mechanism
The kinetic mechanism are organized according to the reactant-phase:
- [Homogeneous Gas-Phase](Gas-Phase) mechanisms address the reactivity of compounds reacting in gas-phase (e.g., hydrogen, gasolines). 
    These mechanisms can be also coupled to the other phase kinetics to study secondary gas-phase reactions.
    To choose the proper kinetic mechanism, refer to the gas-phase [readme subsection](Gas-Phase/README.md#choice-of-kinetic-mechanism).
    In general, kinetic models including pollutants formations are available for:
     - Carbon Free fuels (e.g., [Hydrogen](Gas-Phase/CarbonFreeFuels_H2-NH3/NH3_31_202) and [Ammonia](Gas-Phase/CarbonFreeFuels_H2-NH3/NH3_31_202)) 
        and eFuels (e.g., [methanol](Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_NOX_497_24501) and [DME](Gas-Phase/Gasoline-Biogasoline/TPRF_HT_LT_ALC_ETHERS_356_10171))
     - [Syngas](Gas-Phase/CoreMechanism_C0-C4/SYNGAS_21_62) and [Natural Gas](Gas-Phase/CoreMechanism_C0-C4/Soot-NOx/C1_C3_HT_NOX_159_2459)
     - Gasolines and Biogasoline (refer to the [readme subsection](Gas-Phase/README.md#choice-of-kinetic-mechanism))
     - Diesels and Biodiesels (refer to the [readme subsection](Gas-Phase/README.md#choice-of-kinetic-mechanism))
- [Liquid-Phase](Liquid-Phase) mechanisms address decompositio of heavy fuels which thermally decompose before evaporating to gas-phase.
    The main classes of compounds are:
     - [Plastics](Liquid-Phase/Plastics), which are considered as liquids as their degradation occurs in the molten state.
        Kinetic models are currently available for the main polymers ([polyethylene](Liquid-Phase/Plastics/PE), [polypropylene](Liquid-Phase/Plastics/PP),
        [polystyrene](Liquid-Phase/Plastics/PS), and [poly(vinyl chloride)](Liquid-Phase/Plastics/PVC)) but further work to expand the polymer palette is under-way.
    - Heavy Fuel Oils [(HFO)](Liquid-Phase/HeavyFuelOil), which are further categorized as SARA or resins.     
- [Solid-Phase](Solid-Phase) mechanisms address decomposition of solid fuels. The main fuels are:
     - [Biomass](Solid-Phase/Biomass), accounting also for secondary gas-phase reactions of volatiles. As discussed in the readme file, the biomass model can be coupled to other gas-phase subsets.
     - [Coal](Solid-Phase/Coal), accounting for detailed release of nitrogen and sulphur pollutants and hetereogeneous char reactivity. 
        Secondary gas-phase sulphur reactivity will be included in the next releases of the gas-phase mechanism. 
- [Heterogeneous-Surface](Heterogeneous-Mechanisms) mechanisms are heterogeneous surface models for a broad range of applications. Currently the mechanism reported involve:
     - [pyrocarbon deposition](Heterogeneous-Mechanisms/CVI-CVD), accounting both Chemical Vapour Infiltration and Deposition and methane pyrolysis.   
     - [biochar oxidation](Heterogeneous-Mechanisms/Char) accounting for secondary heterogeneous reactions of char obtained from biomass   
    
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
