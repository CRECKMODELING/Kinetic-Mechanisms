# PVC kinetic Mechanisms

In this folder are present the CHEMKIN format files.
They are divided by the kinetic mechanism prepared:
The folders are labelled polymer_Nspecies_Nreactions. For instance PVC_85_200 
is the folder of the mechanism with 65 species and 550 reactions.
The mechanism proposed are:
- PVC_85_200 the published mechanism [10.1016/S0165-2370(03)00024-X](https://doi.org/10.1016/S0165-2370(03)00024-X) 

No improvement has been currently made. Further work will address:
- Study of the thermodynamic properties of compounds
- Modifying the description of the solid residue to be in-line with the biomass 
   mechanism and PET (under development currently)

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only FAKE liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.  
 
