# PS kinetic Mechanisms

In this folder are present the CHEMKIN format files.
Each mechanism is labelled as polymer_Nspecies_Nreactions. For instance PS_44_330 
is the mechanism with 44 species and 330 reactions.
The mechanism proposed for PS are:
- [PS_55_500](PS_semidetailed) which is the updated published mechanism [(Locaspi et al., (2023)](https://doi.org/10.1016/j.jaap.2023.105960)
- [PS_42_300](PS_reduced) a reduced version with lower computational cost
- [PS_7_6](PS_multistep) a "global" mechanism with significantly lower computational cost. 
The reduction is performed with the approach proposed by [Pegurri et al. (2023)](https://doi.org/10.1016/j.combustflame.2023.113202).

To cite the **Semi-detailed** Kinetic Mechanisms refer to the following publication:
- **Locaspi, Andrea et al.** "Towards a lumped approach for solid plastic waste gasification: Polystyrene pyrolysis."Journal of Analytical and Applied Pyrolysis 171 (2023): 105960 [DOI](https://doi.org/10.1016/j.jaap.2023.105960)

To cite the **Reduced** and the **multistep** Kinetic Mechanisms refer to the following publication:
- **Locaspi, Andrea et al.** "Reduced-order condensed-phase kinetic models for plastic waste thermochemical recycling: polyethylene, polypropylene, and polystyrene", under review at Chemical Engineering Journal

All mechanisms are described in detail in the PhD thesis:
- **Locaspi Andrea**, "A lumped condensed-phase kinetic model for plastic waste thermochemical recycling", Politecnico di Milano, 2024


## Mechanism description

For all mechanisms, the starting polymer at room temperature is described by the 
species P-C16H16-P. Since the glass transition involves small heat fluxes, the 
initial species represents also the solid-phase polymer. 
Polymer species in OpenSMOKE++ are required to be 
defined in gas-phase as well but do not have physical meaning.

With respect to the published mechanism, the improvements are:
- thermochemistry evaluated with group contributions and Prausnitz phase-change
   data. The difference in enthalpy between gas and liquid species is the 
   evaporation enthalpy, above the critical temperature liquid species share
   the thermodynamic properties of gas-species. *Manuscript in preparation* for PE,   
- transport properties are evaluated with a simplified approach based on critical
   properties, see [Holley et al. (2009)](http://dx.doi.org/10.1016/j.proci.2008.05.067).

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only FAKE liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.  

## Model performances

All mechanisms are validated with ~100 of data from the scientific literature.
Here are reported few validation comparisons in terms of parity plots of mass-loss profiles 
and gas-phase yields. At T>700°C secondary gas-phase reactions occur which will be 
addressed in further studies.
The skeletal model is able to reproduce the characteristic degradation times,
but has significant uncertainties in yields predictions.

<img src="../.images/PSvalidation/Parity_dynamic.svg" width="10000" >

<img src="../.images/PSvalidation/Parity_yields.svg" width="10000" >

 
  
 
 
