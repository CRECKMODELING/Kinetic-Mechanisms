# Diesel-Biodisel-Kinetic-Mechanisms (v. 2003)

Diesel and Biodiesel kinetic mechanisms for different fuels with different levels of accuracy.
Current version 2003.
Most of the mechanisms are available with or without NOx and soot submodules.
Please contact us at creckmodeling-dcmc@polimi.it for questions and comments. 

All the mechanisms are freely available in CHEMKIN format (compatible with version 3.6.2 and above).
Please contact us at creckmodeling-dcmc@polimi.it for reduced mechanisms and specific fuels
(e.g. butanoic acid, DME, MTBE, TAME, methyl-butanoate with NOx and soot, ...).

## Choice of Kinetic Mechanism
Several mechanisms are proposed according to the fuel, operating conditions and level of detail in products distribution.
The full mechanism accounting for High and Low temperatures, Soot and NOx formation for most fuels is [TOT_HT_LT_SOOT_NOX](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829).
Simpler mechanisms are available as well, refer to the Table below to choose the appropriate one.
For reduced mechanisms and specific fuels, please contact us at creckmodeling-dcmc@polimi.it

<details open>
<summary>Mechanism choice</summary>
The following abbreviations are employed:
*HT = high-temperature mechanism
*LT = low-temperature mechanism
*NOx = sub-module for nitrogen-oxides
*Soot = sub-module for soot particles (based on the Discrete Sectional model)

|Fuel component	|Real Fuel	|HT	|HT+LT	|HT+NOx	|HT+LT+NOx	|HT+SOOT	|HT+LT+SOOT	|HT+NOx+SOOT	|HT+LT+NOx+SOOT	|
|-----------------------	|-----------------------	|-----------------------	|-----------------------	|-----------------------	|-----------------------	|-----------------------	|-----------------------	|-----------------------	|-----------------------	|
|**nC10H22**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**nC12H26**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**nC16H34**	|*Diesel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**iC12H26**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**iC16H34**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Xylene**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**n-propyl-benzene**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Tri-methyl-benzene**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Cyclo-hexane**	|*Gasoline/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Methyl-cyclo-hexane**	|*Gasoline/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Decalin**	|*JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Methyl-Naphtalene**	|*Diesel/JetFuel*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Methyl-butanoate**	|*Biodiesel*	|[*HT*](TOT_HT_ME_402_16118)	|[*HT+LT*](TOT_HT_LT_ME_582_21174)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Methyl-decanoate**	|*Biodiesel*	|[*HT*](TOT_HT_ME_402_16118)	|[*HT+LT*](TOT_HT_LT_ME_582_21174)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Methyl-palmitate**	|*Biodiesel*	|[*HT*](TOT_HT_ME_402_16118)	|[*HT+LT*](TOT_HT_LT_ME_582_21174)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Methyl-stearate**	|*Biodiesel*	|[*HT*](TOT_HT_ME_402_16118)	|[*HT+LT*](TOT_HT_LT_ME_582_21174)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Methyl-linoleate**	|*Biodiesel*	|[*HT*](TOT_HT_ME_402_16118)	|[*HT+LT*](TOT_HT_LT_ME_582_21174)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Methyl-linolenate**	|*Biodiesel*	|[*HT*](TOT_HT_ME_402_16118)	|[*HT+LT*](TOT_HT_LT_ME_582_21174)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Phenol**	|*Bio-oil*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Anisole**	|*Bio-oil*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Guaiacol**	|*Bio-oil*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Catechol**	|*Bio-oil*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Vanillin**	|*Bio-oil*	|[*HT*](TOT_HT_368_14462)	|[*HT+LT*](TOT_HT_LT_492_17790)	|[*HT+NOx*](Soot-NOx/TOT_HT_NOX_413_14922)	|[*HT+LT+NOx*](Soot-NOx/TOT_HT_LT_NOX_537_18250)	|[*HT+SOOT*](Soot-NOx/TOT_HT_SOOT_452_24041)	|[*HT+LT+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	|[*HT+NOx+SOOT*](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)	|[*HT+LT+NOx+SOOT*](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	|
|**Butanoic Acid**	|*Bio-oil*	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|
|**Pentanoic Acid**	|*Bio-oil*	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|[mail us](mailto:creckmodeling-dcmc@polimi.it)	|

</details>

## Kinetic Mechanism Description
To *cite each Kinetic Mechanism* refer to the README.md in the corresponding subfolder.
The mechanisms available are summarized in the following table. To choose the 
proper mechanism according to the desired fuel and accuracy, please refer to the
[Table above](#choice-of-kinetic-mechanism).

<details open>
<summary>Mechanism description</summary>

The following abbreviations are employed:
*HT = high-temperature mechanism
*LT = low-temperature mechanism
*NOX = sub-module for nitrogen-oxides
*Soot = sub-module for soot particles (based on the Discrete Sectional model)


|Name	                          |Species	|Reactions	|Notes         |
|---------------------------------|---------|-----------|--------------|
|[TOT_HT](TOT_HT_368_14462)	                  |368	    |14462	    |C1-C16 high temperature (HT)       |
|[TOT_HT_LT](TOT_HT_LT_492_17790)	          |492	    |17790	    |C1-C16 high and low temperature (HT+LT)|
|[TOT_HT_LT_ETHERS](TOT_HT_LT_ETHERS_509_18288)	       |509	    |182880	    |C1-C16 high and low temperature (HT+LT) and Ethers|
|[TOT_HT_ME](TOT_HT_ME_402_16118)	          |402	    |16118	    |C1-C16 high temperature (HT) and Methyl-Esters (ME)|
|[TOT_HT_LT_ME](TOT_HT_LT_ME_582_21174)	      |582	    |21174	    |C1-C16 high and low temperature (HT+LT) and Methyl-Esters (ME)|
|[TOT_HT_NOX](Soot-NOx/TOT_HT_NOX_413_14922)	          |413	    |14922	    |C1-C16 high temperature (HT) and NOx|
|[TOT_HT_LT_NOX](Soot-NOx/TOT_HT_LT_NOX_537_18250)	  |537	    |18250	    |C1-C16 high and low temperature (HT+LT) and NOx|
|[TOT_HT_SOOT](Soot-NOx/TOT_HT_SOOT_452_24041)	      |452	    |24041      |C1-C16 high temperature (HT) and soot|
|[TOT_HT_LT_SOOT](Soot-NOx/TOT_HT_LT_SOOT_576_27369)	  |571	    |26349	    |C1-C16 high and low temperature (HT+LT) and soot!
|[TOT_HT_SOOT_NOX](Soot-NOx/TOT_HT_SOOT_NOX_497_24501)  |497	    |24501	    |C1-C16 high temperature (HT), soot and NOx|
|[TOT_HT_LT_SOOT_NOX](Soot-NOx/TOT_HT_LT_SOOT_NOX_621_27829)	  |621	    |27369	    |C1-C16 high and low temperature (HT+LT), soot and NOx|

</details>
