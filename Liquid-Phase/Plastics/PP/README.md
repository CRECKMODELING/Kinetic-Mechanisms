# PP kinetic Mechanisms

In this folder are present the CHEMKIN format files.
They are divided by the kinetic mechanism prepared:
The folders are labelled polymer_Nspecies_Nreactions. For instance PP_250_13000 
is the folder of the mechanism with 250 species (gas+liquid) and 13000 reactions.
The mechanism proposed are:
- PP_250_13000 the published mechanism (10.1016/j.wasman.2022.11.02) 

No modification has been introduced and the thermodynamic and transport 
properties are fake values.

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only FAKE liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.  
 