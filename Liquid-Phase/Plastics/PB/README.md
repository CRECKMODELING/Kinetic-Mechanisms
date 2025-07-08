# PB kinetic Mechanisms

In this folder are present the CHEMKIN format files of the mechanism.
Only the semi-detailed mechanism is available currently, and its labelled as
labelled polymer_Nspecies_Nreactions:
- PB_50_415 the semi-detailed PB mechanism, currently under review  

The **thermodynamic properties have not been investigated** but currently under work.

To cite the semi-detailed mechanism refer to the following publication:
- **Creadore, Lauren T. et al.** "A semi-detailed chemical kinetic model of polybutadiene pyrolysis", Fuel (2025), **under review**

## Mechanism description

For all mechanisms, only the amorphous polymer is considered currently. The starting 
polymer is described by "P-PB-P" for 1,4-microstructures (cis/trans) and "P-PBv-P" 
for 1,2-microstructures (vinyl). The "v" in the species names refers to species
with 1,2 structures, while the "x" in the label refers to the cross-linked one.
The 1,2 and 1,4 distinction is lost for volatiles to reduce the number of species.
Analogously to the mechanisms for the other polymers, phase-change is considered 
through pseudo-reaction. In OpenSMOKE++, polymer and char species species must be 
defined in gas-phase as well, but do not have physical meaning.

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only *FAKE* liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.