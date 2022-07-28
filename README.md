Deep eutectic solvent force field parameters (OPLS-DES)
=================================================

[Orlando Acevedo](http://www.acevedoresearch.com), University of Miami

This repository holds a set of OPLS-AA parameters for use in deep eutectic solvent simulations. 

**OPLS-AA force field parameters (OPLS-DES).**
Please see the following references for technical details:
1. [doi:10.1021/acs.jpcb.8b06647](http://pubs.acs.org/doi/abs/10.1021/acs.jpcb.8b06647)
2. [doi:10.1021/acs.jctc.1c00047](http://pubs.acs.org/doi/abs/10.1021/acs.jctc.1c00047)

**IMPORTANT**: Hydrogen bond donor (HBD) parameters should NOT be used for pure organic liquid simulations! HBD parameters were specifically parameterized to work exclusively with the provided ion pairs in a DES environment.

Requirements
------------
* [Gromacs 5.0.7](http://www.gromacs.org/Downloads)
    * Tested with CUDA 7.5/8.0 and on CentOS 6.5/7.0
    * Heat capacity DoS calculations (g_dos) requires Gromacs 5.1.4 due to a known bug in version 5.0.7
    
Download
-----
```
git clone git://github.com/orlandoacevedo/DES.git
```

Parameters Available
--------------------
* **Ions**
    * choline
    * chloride
    * ethylammonium
    * N,N-diethylethanolammonium
    * N-ethyl-N,N-dimethylethanolammonium
* **Hydrogen bond donors**
    * urea
    * glycerol
    * phenol
    * ethylene glycol
    * levulinic acid
    * oxalic acid
    * malonic acid
    * acetamide
    * 2,2,2-trifluoroacetamide
    
* **DES** - OPLS-DES bonded and nonbonded parameters
    * itp, top, and pdb folders

Tutorial
--------
A brief tutorial is provided in the CCU-Tutorial directory. A README file will guide the user through the contruction of a CCU (reline) box using the OPLS-DES parameter set and a subsequent MD simulation. GROMACS input and output files are provided. The user is guided on how to compute the density of the deep eutetic solvent system.

References
----------
Doherty, B.; Acevedo, O. "OPLS Force Field for Choline Chloride-Based Deep Eutectic Solvents" *J. Phys. Chem. B*, **2018**, *122*, 9982-9993. [doi:10.1021/acs.jpcb.8b06647](http://pubs.acs.org/doi/abs/10.1021/acs.jpcb.8b06647)
* Featured on the journal cover [Nov. 1, 2018 issue](https://pubs.acs.org/toc/jpcbfk/122/43)

Zhong, X.; Velez, C.; Acevedo, O. "Partial Charges Optimized by Genetic Algorithms for Deep Eutectic Solvent Simulations" *J. Chem. Theory Comput.*, **2021**, *17*, 3078–3087. [doi:10.1021/acs.jctc.1c00047](https://pubs.acs.org/doi/abs/10.1021/acs.jctc.1c00047)

Velez, C.; Acevedo, O. "Simulation of Deep Eutectic Solvents: Progress to Promises" *WIREs Comput. Mol. Sci.*, **2022**, *12*, e1598. [doi:10.1002/wcms.1598](https://doi.org/10.1002/wcms.1598)

Rukmani, S.J.; Doherty, B.; Acevedo, O.; Colina, C.M. "Molecular simulations of deep eutetic solvents: A perspective on structure, dynamics, and physical properties" *Rev. Comput. Chem.*, **2022**, *32*, 135-216. [doi:doi.org/10.1002/9781119625933.ch4](https://doi.org/10.1002/9781119625933.ch4)

About
-----
**Contributing Authors**: Brian Doherty, Caroline Velez, Xiang Zhong, and Orlando Acevedo*

**Funding**: Gratitude is expressed to the National Science Foundation (NSF CHE-1562205 and CHE-2102038) for funding the project.

**Software License**:
OPLS-DES.
Copyright (C) 2021 Orlando Acevedo

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details. <http://www.gnu.org/licenses/>
