# PS kinetic Mechanisms

In this folder are present the CHEMKIN format files.
They are divided by the kinetic mechanism prepared:
The folders are labelled polymer_Nspecies_Nreactions. For instance PS_65_550 
is the folder of the mechanism with 65 species and 550 reactions.
The mechanism proposed are:
- PS_65_550 the published mechanism (10.1016/j.jaap.2023.105960) 

With respect to the published mechanism, the improvements are:
- thermochemistry evaluated with group contributions and van Krevelen phase-change
   data. The difference in enthalpy between gas and liquid species is the 
   evaporation enthalpy, above the critical temperature liquid species share
   the thermodynamic properties of gas-species
- transport properties are evaluated with a simplified approach based on critical
   properties (see RMG mit)

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only FAKE liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.  
 
