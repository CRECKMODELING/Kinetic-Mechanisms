# Char Kinetic Mechanisms

Kinetic mechanism for char oxidation. The model has been validated for chars
obtained from biomass pyrolysis, but with appropriate characterizations the model
can be extended to coal and plastic chars.
To predict the biochar chemical composition, the [biomass pyrolysis kinetic model](../../Solid-Phase/Biomass) can 
be employed.  

The oxidation CHEMKIN-like surface reaction mechanism is in the subfolders.
As the chemical evolution of char cannot be decoupled from the physical one,
the kinetic mechanism requires specific solvers able to enforce the
consistency of the chemical and physical evolution of the particle.

To this aim, two versions of the mechanism are presented:
- [CharOxidation_chemkinlike](CharOxidation_chemkinlike), which reports simply all the reactions involved in the model
- [CharOxidation_kinetics4opensmoke](CharOxidation_kinetics4opensmoke), which reports the kinetic mechanism in a format suitable for opensmoke.
    Specifically, several fake species are introduced to identify the reaction classes and
    modify the reaction rates such that site density conservation is ensured. A suitable 
    solver has been developed based on the OpenSMOKE++ framework which however is not 
    in the current suite.
Further work is underway at CRECK modelling POLIMI to better assess secondary gasification 
reactions.

To cite the Kinetic Mechanism refer to the following publications:
- **Locaspi, Andrea et al.** "A predictive physico-chemical model of biochar oxidation." Energy&Fuels 35 (2021): 14894–14912. [DOI](https://doi.org/10.1021/acs.energyfuels.1c01559)

