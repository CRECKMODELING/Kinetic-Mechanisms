# PE kinetic Mechanisms

In this folder are present the CHEMKIN format files.
The folders are labelled polymer_Nspecies_Nreactions. For instance HDPE_42_500 
is the folder of the mechanism with 42 species and 500 reactions.
The mechanism proposed for HDPE are:
- [HDPE_120_2500](HDPE_120_2500) the updated published mechanism cantera and 
    opensmoke compatible 
- [HDPE_42_500](HDPE_42_500) a further lumped version with lower computational cost.
- [HDPE_10_10](HDPE_10_10) a skeletal model with significantly lower computational cost.

For LDPE only the [lumpest version](LDPE_42_500), a [chemkin compatible version](LDPE_120_3200)
and the [skeletal model](LDPE_10_10) are proposed. 

To cite the Semi-detailed Kinetic Mechanisms refer to the following publication:
- **Locaspi, Andrea et al.** "Towards a lumped approach for solid plastic waste gasification: Polyethylene and polypropylene pyrolysis." Waste Management 156 (2023): 107-117 [DOI](https://doi.org/10.1016/j.wasman.2022.11.028)

To cite the Skeletal Kinetic Mechanisms refer to the following publication:
- **Locaspi, Andrea et al.** "A skeletal condensed-phase kinetic model for polyethylene thermal degradation", under review at Proceeding of The Combustion Institue
  
## Mechanism description

The starting polymer at room temperature is described by the species
P-CnH2n-P_S and P-CnH2n-P which represent the crystalline and amorphous polymer
If the simulation starts above the melting point (130C), the polymer is 
described only by P-CnH2n-P. Polymer species in OpenSMOKE are required to be 
defined in gas-phase as well.

With respect to the published mechanism [(Locaspi et al. (2022)](https://doi.org/10.1016/j.wasman.2022.11.028), 
the improvements are:
- better agreement with ethylene formation
- a species representative of the crystalline polymer is introduced
- stable short chain species are formed directly in gas-phase, while for longer
   compounds able to evaporate evaporation reactions are introduced, see [Locaspi et al. (2023)](https://doi.org/10.1016/j.jaap.2023.105960)  
- thermochemistry evaluated with group contributions and van Krevelen phase-change
   data. The difference in enthalpy between gas and liquid species is the 
   evaporation enthalpy, above the critical temperature liquid species share
   the thermodynamic properties of gas-species. *Manuscript under review*
- transport properties are evaluated with a simplified approach based on critical
   properties, see [Holley et al. (2009)](http://dx.doi.org/10.1016/j.proci.2008.05.067).

In each folder are present the standard CHEMKIN files (gas kinetics, liquid kinetics, 
thermodynamics, transport) and a sub-folder of LiquidProperties.
The latter is required by OpenSMOKE but reports only *FAKE* liquid properties of
all the chemical species included in the mechanism. These are required for the 
1D microgravity model available in OpenSMOKE, but they have not yet been addressed 
for polymers outside of 0D systems.
  
 



