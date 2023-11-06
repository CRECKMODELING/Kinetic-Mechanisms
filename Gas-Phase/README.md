# GasPhase-Kinetic-Mechanisms (v. 2003)

Gas-phase kinetic mechanisms for different fuels with different levels of accuracy,
they are reported also on the [creckmodelling website](https://creckmodeling.chem.polimi.it/).
Current version 2003.

The mechanisms provided are hierarchically organized: moving from syngas 
up to large mechanisms for jet-fuels and diesel fuels. All the mechanisms are 
self consistent, i.e., they already include the previous sub-mechanisms. 
Most of the mechanisms are available with or without NOx and soot submodules.
Please contact us at creckmodeling-dcmc@polimi.it for questions and comments. 

All the mechanisms are freely available in CHEMKIN format (compatible with version 3.6.2 and above).
Please contact us at creckmodeling-dcmc@polimi.it for reduced mechanisms and specific fuels
(e.g. butanoic acid, DME, MTBE, TAME, methyl-butanoate with NOx and soot, ...).

## Kinetic Mechanism Description
To *cite each Kinetic Mechanism* refer to the README.md in the corresponding subfolder.
The mechanisms available are summarized in the following table. To choose the 
proper mechanism according to the desired fuel and accuracy, please refer to the
[Table available on the website](http://creckmodeling.chem.polimi.it/menu-kinetics/menu-kinetics-detailed-mechanisms).
The following abbreviations are employed:
*HT = high-temperature mechanism
*LT = low-temperature mechanism
*NOX = sub-module for nitrogen-oxides
*Soot = sub-module for soot particles (based on the Discrete Sectional model)

|Name	                          |Species	|Reactions	|Notes         |
|---------------------------------|---------|-----------|--------------|
|[HYDROGEN](HYDROGEN_11_20)	                  |11       |20	        |H2|
|[HYDROGEN_NOX](NH3_31_202)	                  |31       |202        |NH3/H2 mixtures|
|[SYNGAS](SYNGAS_21_62)	                      |21       |62	        |H2/CO mixtures|
|[AMMONIA](NH3_31_202)	                      |31       |202        |NH3/H2 mixtures|
|[C1_C3_HT](C1_C3_HT_114_1999)	              |114	    |1999	    |C1-C3 high-temperature (HT)|
|[C1_C3_HT_NOX](C1_C3_HT_NOX_159_2459)	      |159	    |2459	    |C1-C3 high-temperature (HT) and NOx|
|[TOT_HT](TOT_HT_368_14462)	                  |368	    |14462	    |C1-C16 high temperature (HT)       |
|[TOT_HT_LT](TOT_HT_LT_492_17790)	          |492	    |17790	    |C1-C16 high and low temperature (HT+LT)|
|[TOT_HT_LT_ETHERS](TOT_HT_LT_ETHERS_509_18288)	       |509	    |182880	    |C1-C16 high and low temperature (HT+LT) and Ethers|
|[TOT_HT_NOX](TOT_HT_NOX_413_14922)	          |413	    |14922	    |C1-C16 high temperature (HT) and NOx|
|[TOT_HT_LT_NOX](TOT_HT_LT_NOX_537_18250)	  |537	    |18250	    |C1-C16 high and low temperature (HT+LT) and NOx|
|[TOT_HT_SOOT](TOT_HT_SOOT_452_24041)	      |452	    |24041      |C1-C16 high temperature (HT) and soot|
|[TOT_HT_LT_SOOT](TOT_HT_LT_SOOT_576_27369)	  |571	    |26349	    |C1-C16 high and low temperature (HT+LT) and soot!
|[TOT_HT_ME](TOT_HT_ME_402_16118)	          |402	    |16118	    |C1-C16 high temperature (HT) and Methyl-Esters (ME)|
|[TOT_HT_LT_ME](TOT_HT_LT_ME_582_21174)	      |582	    |21174	    |C1-C16 high and low temperature (HT+LT) and Methyl-Esters (ME)|
|[TOT_HT_SOOT_NOX](TOT_HT_SOOT_NOX_497_24501)  |497	    |24501	    |C1-C16 high temperature (HT), soot and NOx|
|[TOT_HT_LT_SOOT_NOX](TOT_HT_LT_SOOT_NOX_621_27829)	  |621	    |27369	    |C1-C16 high and low temperature (HT+LT), soot and NOx|
|[TPRF_HT_ALC](TPRF_HT_ALC_254_7568)	          |254	    |7568	    |Toluene Primary Reference Fuels (TPRF) high temperature (HT) and Alcohols|
|[TPRF_HT_LT_ALC](TPRF_HT_LT_ALC_339_9781)	  |339	    |9781	    |Toluene Primary Reference Fuels (TPRF) high and low temperature (HT+LT) and Alcohols|
|[TPRF_HT_ALC_NOX](TPRF_HT_ALC_NOX_299_8028)	  |299	    |8028	    |Toluene Primary Reference Fuels (TPRF) high temperature (HT), Alcohols and NOx|
|[TPRF_HT_LT_ALC_ETHERS](TPRF_HT_LT_ALC_ETHERS_356_10171) |356	    |10171	    |Toluene Primary Reference Fuels (TPRF) high and low temperature (HT+LT), Alcohols and Esters|

