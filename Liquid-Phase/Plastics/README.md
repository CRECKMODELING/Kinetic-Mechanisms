# Polymers-Kinetic-Mechanisms

Condensed-phase polymer degradation kinetic Mechanisms. Evaluation of gas-phase
pyrolytic and gasification reactivity are underway at CRECK modelling POLIMI.
The kinetic mechanisms are reported also on the [creckmodelling website](https://creckmodeling.chem.polimi.it/)

The folders are organized by polymer type. The available polymer mechanisms are:
- **Polyethylene (PE)**: different mechanisms are available for HDPE and LDPE
    according to the degree of detail involved in products and radicals description.
    Specifically, for HDPE the [published](PE/HDPE_120_2500), [reduced](PE/HDPE_42_500) 
    and [skeletal](PE/HDPE_10_10) versions are availble. For LDPE the [chemkin-compatible](PE/LDPE_120_3200), 
    [reduced](PE/LDPE_42_500) and [skeletal](PE/LDPE_10_10) mechanism are reported.
- **Polypropylene (PP)**: a [single mechanism](PP) is reported.
- **Polystyrene (PS)**: the proposed mechanisms account for all structural differences. 
    The [published](PS/PS_54_550) mechanism and both a [reduced](PS/PS_44_330) 
    and [skeletal](PS/PS_7_6) version are currently available. 
- **Poly(vinyl chloride) (PVC)**: the proposed [mechanism](PVC) accounts for the pure polymer degradation.
- Further work will address development of models for **PET, PA, PMMA, and PU** and condensed-phase interactions

## Kinetic Mechanism Description
The kinetic mechanism proposed are of the semi-detailed kind employing a
functional group approach:
- Long polymer chains are described with functional groups characteristic of
    the polymer moieties (mid- and end-chain groups) recognized by the "P-" in
    their name
- Short chains, i.e. compounds of interest, are described with real species as
    C2H4, C15H30, etc
    
Thermochemistry has been validated for PE, while for PS it has been implemented
but without quantitative validation yet.
Transport parameters are evaluated with a simplified approach based on critical
temperatures and pressures, see [Holley et al. (2009)](http://dx.doi.org/10.1016/j.proci.2008.05.067).
The present models cannot be directly coupled to the creck gas-phase mechanism, 
but further work is underway to assess the secondary gas-phase reactivity.

