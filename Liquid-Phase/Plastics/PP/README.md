# PP kinetic Mechanisms

In this folder are present the CHEMKIN format files.
Each mechanism is labelled as polymer_Nspecies_Nreactions. For instance PP_10_10 
is the mechanism with 10 species and 10 reactions.
The mechanism proposed for PS are:
- [PP_240_13000](PP_semidetailed) which is the updated published mechanism [(Locaspi et al. (2022))](https://doi.org/10.1016/j.wasman.2022.11.028)
- [PP_130_2500](PP_reduced) a reduced version with lower computational cost
- [PP_10_12](PP_multistep) a "global" mechanism with significantly lower computational cost. 
The reduction is performed with the approach proposed by [Pegurri et al. (2023)](https://doi.org/10.1016/j.combustflame.2023.113202).


To cite the semi-detailed Kinetic Mechanism refer to the following publications:
- **Locaspi, Andrea et al.** "Towards a lumped approach for solid plastic waste gasification: Polyethylene and polypropylene pyrolysis." Waste Management 156 (2023): 107-117 [DOI](https://doi.org/10.1016/j.wasman.2022.11.028)

To cite the **Reduced** and the **multistep** Kinetic Mechanisms refer to the following publication:
- **Locaspi, Andrea et al.** "Reduced-order condensed-phase kinetic models for plastic waste thermochemical recycling: polyethylene, polypropylene, and polystyrene", under review at Chemical Engineering Journal

All mechanisms are described in detail in the PhD thesis:
- **Locaspi Andrea**, "A lumped condensed-phase kinetic model for plastic waste thermochemical recycling", Politecnico di Milano, 2024

## Mechanism description

For all mechanisms the starting polymer at room temperature is described by the species
P-IC30H60-P_S and P-IC30H60-P which represent the crystalline and amorphous polymer respectively.
If the simulation starts above the melting point (170C), the polymer is 
described only by P-IC30H60-P. Polymer species in OpenSMOKE++ are required to be 
defined in gas-phase as well but do not have physical meaning.

With respect to the published mechanism [(Locaspi et al. (2022)](https://doi.org/10.1016/j.wasman.2022.11.028), 
the improvements are:
- better agreement with propylene and trimer formation
- a species representative of the crystalline polymer is introduced
- stable short chain species are formed directly in gas-phase, while for longer
   compounds able to evaporate evaporation reactions are introduced, see [Locaspi et al. (2023)](https://doi.org/10.1016/j.jaap.2023.105960)  
- thermochemistry evaluated with group contributions and Prausnitz phase-change
   data. The difference in enthalpy between gas and liquid species is the 
   evaporation enthalpy, above the critical temperature liquid species share
   the thermodynamic properties of gas-species. *Manuscript under review*.
   For the semi-detailed and reduced models, the thermodynamic properties of 
   head and tail configurations are assumed equale
- transport properties are evaluated with a simplified approach based on critical
   properties, see [Holley et al. (2009)](http://dx.doi.org/10.1016/j.proci.2008.05.067).

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only *FAKE* liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.

## Model Performances
All mechanisms are validated with ~70 of data from the scientific literature.
Here are reported few validation comparisons in terms of parity plots of mass-loss profiles 
and gas-phase yields. At T>600°C secondary gas-phase reactions occur which will be 
addressed in further studies.
The detailed model of [Ranzi et al. (1997)](https://doi.org/10.1016/S0165-2370(97)00032-6) is also reported for comparison.

<img src="../.images/PPvalidation/Parity_dynamic.svg" width="10000" >

