# Polymers-Kinetic-Mechanisms

Condensed-phase polymer degradation kinetic Mechanisms. Evaluation of gas-phase
pyrolytic and gasification reactivity are underway at CRECK modelling POLIMI.
The kinetic mechanisms are reported also on the [creckmodelling website](https://creckmodeling.chem.polimi.it/)

The folders are organized by polymer type.
The kinetic mechanism proposed are of the semi-detailed kind employing a
functional group approach:
- Long polymer chains are described with functional groups characteristic of
    the polymer moieties (mid- and end-chain groups) recognized by the "P-" in
    their name
- Short chains, i.e. compounds of interest, are described with real species as
    C2H4, C15H30, etc

The available polymer mechanisms are:
- **Polyethylene (PE)**: different mechanisms are available for [HDPE](PE/HDPE) and [LDPE](PE/LDPE)
    according to the degree of detail involved in products and radicals description.
- **Polypropylene (PP)**: different mechanisms for [isotactic PP](PP/isoPP) and [atactic PP](PP/aPP)
- **Polystyrene (PS)**: the [proposed mechanism](PS) accounts for all structural differences 
- **Poly(vinyl chloride) (PVC)**: the [proposed mechanism](PVC) accounts for the pure polymer degradation.
- Further work will address development of models for **PET, PA, PMMA, and PU** and condensed-phase interactions

Thermochemistry has been validated for PE, while for PS it has been implemented
but without quantitative validation yet.
Transport parameters are evaluated with a simplified approach based on critical
temperatures and pressures (see [Holley et al. 2009](http://dx.doi.org/10.1016/j.proci.2008.05.067)).
The present models cannot be directly coupled to the creck gas-phase mechanism, 
but further work is underway to assess the secondary gas-phase reactivity.

