# Kinetic-Mechanisms
<p align="center">
    <img src=".images/intro.svg" alt="Logo" width="600"/>
</p>


Kinetic Mechanisms for **gas**, **liquid** and **solid** fuels, current version CRECK_2003.
All the mechanisms are freely available in CHEMKIN format (compatible with version 3.6.2 and above) and 
are self-consistent, i.e. they contain smaller subsets and can be coupled together. 
<Most of the mechanisms are available with or without NOx and soot submodules.>
Please contact us at creckmodeling-dcmc@polimi.it for questions and comments. 

## Choice of Kinetic Mechanisms
The kinetic mechanism are organized according to the reactive-phase:
- [Homogeneous Gas-Phase](Gas-Phase) mechanisms address compounds reacting in gas-phase (e.g., **H2**, **gasolines**, **diesel**). 
    These mechanisms can be also coupled to the other phase kinetics to study secondary gas-phase reactions.

    **For a detailed list of gas-phase kinetic mechanism** &rarr; **[Click here](Gas-Phase/README.md#choice-of-kinetic-mechanism)**.
    &nbsp; <a href="mailto:creckmodeling-dcmc@polimi.it"> Mail us </a> for other mechanisms!
    <details>
    <summary><ins>Quick choice of gas kinetic mechanism</ins></summary>
    &nbsp; HT = <i>High-Temperature</i>, LT = <i>Low-Temperature</i>, NOx = <i>sub-module for nitrogen-oxides and ammonia</i>, Soot = <i>sub-module for soot particles</i>
    <ul>
        <li> <b>Hydrogen</b> (H<sub>2</sub>): &nbsp; <a href="Gas-Phase/CarbonFreeFuels_H2-NH3/HYDROGEN_11_20"> HT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/CarbonFreeFuels_H2-NH3/NH3_31_202"> HT+NOx </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_452_24041"> HT+SOOT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_NOX_497_24501"> HT+NOx+SOOT</a> </li>
        <li> <b>Ammonia</b> (NH<sub>3</sub>): &nbsp; <a href="Gas-Phase/CarbonFreeFuels_H2-NH3/NH3_31_202"> HT </a> &nbsp; &bull; &nbsp;  <a href="Gas-Phase/CarbonFreeFuels_H2-NH3/NH3_31_202">HT+NOx</a>  &nbsp; &bull; &nbsp;  <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_452_24041">HT+SOOT</a>  &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_NOX_497_24501">HT+NOx+SOOT</a> </li>
        <li> <b>Methane</b> (CH<sub>4</sub>): &nbsp;<a href="Gas-Phase/CoreMechanism_C0-C4/C1_C3_HT_114_1999"> HT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/CoreMechanism_C0-C4/Soot-NOx/C1_C3_HT_NOX_159_2459"> HT+NOx </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_452_24041"> HT+SOOT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_NOX_497_24501"> HT+NOx+SOOT</a> <br>
        <li> <b>Natural Gas/LPG</b> (C<sub>1</sub>-C<sub>4</sub>): &nbsp;<a href="Gas-Phase/CoreMechanism_C0-C4/C1_C3_HT_114_1999"> HT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/CoreMechanism_C0-C4/Soot-NOx/C1_C3_HT_NOX_159_2459"> HT+NOx </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_452_24041"> HT+SOOT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_NOX_497_24501"> HT+NOx+SOOT</a> <br>
        <li> <b>Methanol</b> (CH<sub>3</sub>OH): &nbsp; <a href="Gas-Phase/CoreMechanism_C0-C4/C1_C3_HT_114_1999"> HT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/CoreMechanism_C0-C4/Soot-NOx/C1_C3_HT_NOX_159_2459"> HT+NOx </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_452_24041"> HT+SOOT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Diesel-Biodiesel/Soot-NOx/TOT_HT_SOOT_NOX_497_24501"> HT+NOx+SOOT</a> </li>
        <li> <b>DME</b> (CH<sub>3</sub>OCH<sub>3</sub>): &nbsp; <a href="Gas-Phase/Gasoline-Biogasoline/TPRF_HT_LT_ALC_ETHERS_356_10171"> HT </a> &nbsp; &bull; &nbsp; <a href="Gas-Phase/Gasoline-Biogasoline/TPRF_HT_LT_ALC_ETHERS_356_10171"> HT+LT </a> </li>
        <li><b>Gasoline/Biogasoline</b> &rarr; refer to this <a href="Gas-Phase/Gasoline-Biogasoline/README.md#choice-of-kinetic-mechanism"> readme subsection </a>  </li>
        <li><b>Jet-fuels</b> &rarr; refer to this <a href="Gas-Phase/Diesel-Biodiesel/README.md#choice-of-kinetic-mechanism"> readme subsection </a> </li>
        <li><b>Diesel/Biodiesel/Bio-oil</b> &rarr; refer to this <a href="Gas-Phase/Diesel-Biodiesel/README.md#choice-of-kinetic-mechanism"> readme subsection </a> </li>
    </ul>
    </details>

- [Liquid-Phase](Liquid-Phase) mechanisms address heavy fuels which decompose before evaporating (e.g., **Plastics**, **Heavy Fuel Oils**).
    <details>
    <summary><ins>Quick choice of <b> <a href="Liquid-Phase/Plastics/"> plastics </a> </b> condensed-phase kinetic mechanism</ins></summary>
    
    <ul>
        <li> <b>Polyethylene High-Density </b> (HDPE): &nbsp; <a href="Liquid-Phase/Plastics/PE/HDPE_semidetailed/"> semi-detailed </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PE/HDPE_reduced/"> reduced </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PE/HDPE_multistep/"> multi-step </a> </li>
        <li> <b>Polyethylene Low-Density </b> (LDPE): &nbsp; <a href="Liquid-Phase/Plastics/PE/LDPE_semidetailed/"> semi-detailed </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PE/LDPE_reduced/"> reduced </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PE/LDPE_multistep/"> multi-step </a> </li>
        <li> <b>Polypropylene </b> (PP): &nbsp; <a href="Liquid-Phase/Plastics/PP/PP_semidetailed/"> semi-detailed </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PP/PP_reduced/"> reduced </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PP/PP_multistep/"> multi-step </a> </li>
        <li> <b>Polystyrene </b> (PS): &nbsp; <a href="Liquid-Phase/Plastics/PS/PS_semidetailed/"> semi-detailed </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PS/PS_reduced/"> reduced </a> &nbsp; &bull; &nbsp; <a href="Liquid-Phase/Plastics/PS/PS_multistep/"> multi-step </a> </li>
        <li> <b>Poly(ethylene terephthalate) </b> (PET): &nbsp; <a href="Liquid-Phase/Plastics/PET"> semi-detailed </a>  </li>
        <li> <b>Poly(vinyl chloride) </b> (PVC): &nbsp; <a href="Liquid-Phase/Plastics/PVC"> semi-detailed </a>  </li>
    </ul>
    </details>    

    *HFO mechanisms will be published soon*

- [Solid-Phase](Solid-Phase) mechanisms address decomposition of solid fuels (e.g., **Biomass**, **Coal**). 
    <details open>
    <summary><ins>Quick choice of solid-phase kinetic mechanism</ins></summary>
    <ul>
        <li> <b> <a href="Solid-Phase/Biomass"> Biomass mechanism</a></b>, accounting also for secondary gas-phase reactions of volatiles. </li>
        <li> <b> <a href="Solid-Phase/Coal"> Coal mechanism</a></b>, accounting for detailed release of N and S pollutants and char reactivity. <i>Secondary gas-phase sulphur reactivity will be included in the next releases of the gas-phase mechanism. </i></li>        
    </ul>
    </details>    
    
- [Heterogeneous-Surface](Heterogeneous-Mechanisms) mechanisms are heterogeneous surface mechanisms (e.g., **CVI-CVD**, **Char**). 
    <details open>
    <summary><ins>Quick choice of surface kinetic mechanism</ins></summary>
    <ul>
        <li> <b> <a href="Heterogeneous-Mechanisms/CVI-CVD"> Pyrocarbon deposition mechanism</a></b>, accounting both Chemical Vapour Infiltration and Deposition and methane pyrolysis. </li>
        <li> <b> <a href="Heterogeneous-Mechanisms/Char"> Biochar oxidation mechanism</a></b>, accounting for secondary heterogeneous reactions of char obtained from biomass.</li>        
    </ul>
    </details>    
    
All the files reported are text-files with "fake" modifiable extensions. Nevertheless, the **following extensions are employed**:
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
