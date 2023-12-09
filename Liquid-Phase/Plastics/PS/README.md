# PS kinetic Mechanisms

In this folder are present the CHEMKIN format files.
Each mechanism is labelled as polymer_Nspecies_Nreactions. For instance PS_44_330 
is the folder of the mechanism with 44 species and 330 reactions.
The mechanism proposed for PS are:
- [PS_65_550](PS_54_550) which is the updated published mechanism [(Locaspi et al., (2023)](https://doi.org/10.1016/j.jaap.2023.105960)
- [PS_42_330](PS_44_330) a reduced version with lower computational cost
- [PS_7_6](PS_7_6) a skeletal mechanism with significantly lower computational cost. 
The reduction is performed with the approach proposed by [Pegurri et al. (2023)](https://doi.org/10.1016/j.combustflame.2023.113202).
Both the reduced and skeletal models are developed as with PE (Locaspi and Faravelli 2024, under review). 

With respect to the published mechanism, the improvements are:
- thermochemistry evaluated with group contributions and van Krevelen phase-change
   data. The difference in enthalpy between gas and liquid species is the 
   evaporation enthalpy, above the critical temperature liquid species share
   the thermodynamic properties of gas-species. *Manuscript in preparation* for PE,
   requires further validation for PS but few TG/DSC data are available
- transport properties are evaluated with a simplified approach based on critical
   properties, see [Holley et al. (2009)](http://dx.doi.org/10.1016/j.proci.2008.05.067).

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only FAKE liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.  
 
