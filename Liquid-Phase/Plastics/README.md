# Polymers-Kinetic-Mechanisms

Condensed-phase polymer degradation kinetic Mechanisms. Evaluation of gas-phase
pyrolytic and gasification reactivity are underway at CRECK modelling POLIMI.

The folders are organized by polymer type. In general semi-detailed, reduced, 
and skeletal mechanisms are available. Specifically:
- **Polybutadiene** ([PB](PB)): a single semi-detailed [mechanism](PB) accounts 
    for the pure polymer degradation, but thermodynamics and transport 
    have not been studied currently.
- **Polyethylene** ([PE](PE)): different models are available for HDPE and LDPE
    according to the degree of detail involved in products and radicals description.
    For HDPE both [semi-detailed](PE/HDPE_semidetailed), [reduced](PE/HDPE_reduced) 
    and [multi-step](PE/HDPE_multistep) versions are availble. The same holds for LDPE with
    the [semi-detailed](PE/LDPE_semidetailed), [reduced](PE/LDPE_reduced) and 
    [multi-step](PE/LDPE_multistep) mechanisms are reported. Thermodynamics and transport
    have been assessed as well. **The multi-step mechanisms have also the complementary gas-phase!**
- **Poly(ethylene terephthalate)** ([PET](PET)): has a [semi-detailed](PET/PET_semidetailed) and
    a [multi-step](PET/PET_multistep) mechanism, but thermodynamics and transport 
    have not been studied currently.
- **Polypropylene** ([PP](PP)): has a [semi-detailed](PP/PP_semidetailed), [reduced](PP/PP_reduced)
    and [multi-step](PP/PP_multistep) mechanism available as well. Thermodynamics and transport
    have been validated. The mechanism for APP has not been reported due to the lower importance
    of APP in general wastes.
- **Polystyrene** ([PS](PS)): the proposed mechanisms account for all structural differences. 
    The [semi-detailed](PS/PS_semidetailed) mechanism and both a [reduced](PS/PS_reduced) 
    and [multi-step](PS/PS_multistep) version are currently available with validated
    thermodynamic properties. 
- **Poly(vinyl chloride)** ([PVC](PVC)): the proposed semi-detailed [mechanism](PVC) accounts for the pure polymer degradation.
- Currently underway are models for **PA, PMMA, and PU** and condensed-phase interactions

## Kinetic Mechanism Description
The kinetic mechanism proposed are of the semi-detailed kind employing a
functional group approach:
- Long polymer chains are described with functional groups characteristic of
    the polymer moieties (mid- and end-chain groups) recognized by the "P-" in
    their name
- Short chains, i.e. compounds of interest, are described with real species as
    C2H4, C15H30, etc
    
Thermochemistry has been validated for PE, PP, and PS.
Transport parameters are evaluated with a simplified approach based on critical
temperatures and pressures, see [Holley et al. (2009)](http://dx.doi.org/10.1016/j.proci.2008.05.067).
The present models cannot be directly coupled to the creck gas-phase mechanism, 
but further work is underway to assess the secondary gas-phase reactivity.

