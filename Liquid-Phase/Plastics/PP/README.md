# PP kinetic Mechanisms

In this folder are present the CHEMKIN format files of the mechanism:
- PP_250_13000 the updated published mechanism cantera and 
    opensmoke compatible [(Locaspi et al. (2022))](https://doi.org/10.1016/j.wasman.2022.11.028)

To cite the Kinetic Mechanism refer to the following publications:
- **Locaspi, Andrea et al.** "Towards a lumped approach for solid plastic waste gasification: Polyethylene and polypropylene pyrolysis." Waste Management 156 (2023): 107-117 [DOI](https://doi.org/10.1016/j.wasman.2022.11.028)

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
Gas kinetics, thermodynamics, transport properties and LiquidProperties are currently **FAKE**.
The latter is required by OpenSMOKE for the 1D microgravity model, but they have not yet been addressed 
for polymers outside of 0D systems.  
 


