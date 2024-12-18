# PET kinetic Mechanisms

In this folder are present the CHEMKIN format files.
The mechanism is labelled polymer_Nspecies_Nreactions. For instance PET_85_700 
is the mechanism with 85 species and 700 reactions.
For PET degradation a single kinetic mechanism is reported.
The thermodynamic properties have not been investigated due to lack of data and
theoretical approaches for aromatic esters.

To cite the Kinetic Mechanisms refer to the following publication:
- **Locaspi, Andrea et al.** "A lumped kinetic model and experimental investigation of Poly(Ethylene Terephthalate) condensed-phase pyrolysis", Chemical Engineering Journal 500 (2024): 156955. [DOI](https://doi.org/10.1016/j.cej.2024.156955) 
  
## Mechanism description

For all mechanisms, the starting polymer at room temperature is described by the species
P-COPhCO-P and P-OCCO-P, which represent the terephthalic and glycol moieties of the amorphous polymer
(present in equimolar ratios). The present mechanism considers a single condensed pseudo-phase
and models char as liquid-phase species. Mechanisms considering two condensed phases
can be provided upon request. Compared to the mechanisms for the other polymers, 
phase-change is considered separatedly and not pseudo-reaction is introduced.
Polymer and char species species in OpenSMOKE++ are required to be defined in 
gas-phase as well but do not have physical meaning.

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only *FAKE* liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.

## Model Performances
All mechanisms are validated with ~50 of data from the scientific literature.
Here are reported few validation comparisons in terms of parity plots of mass-loss profiles 
and gas-phase yields. 

<img src="../../../.images/PETvalidation/Parity_dynamic.svg" width="10000" >

<img src="../../../.images/PETvalidation/yields.svg" width="10000" >

  
 



