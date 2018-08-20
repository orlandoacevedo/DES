Deep eutectic solvent force field parameters (OPLS-DES)
=================================================

[Orlando Acevedo](http://www.acevedoresearch.com), University of Miami

This repository holds a set of OPLS-AA parameters for use in deep eutectic solvent simulations. 

**OPLS-AA force field parameters (OPLS-DES).**
Please see the following references for technical details:
1. [doi:10.1021/acs.jpcb.8b06647](http://pubs.acs.org/doi/abs/10.1021/acs.jpcb.8b06647)

**IMPORTANT**: Hydrogen bond donor (HBD) parameters should NOT be used for pure organic liquid simulations! HBD parameters were specifically parameterized to work exclusively with the provided choline chloride ion pair in a DES environment.

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
* **Hydrogen bond donors**
    * urea
    * glycerol
    * phenol
    * ethylene glycol
    * levulinic acid
    * oxalic acid
    * malonic acid
    
* **DES** - OPLS-DES bonded and nonbonded parameters
    * itp, top, and pdb folders

Tutorial
--------
A brief tutorial is coming soon.


References
----------
Doherty, B.; Acevedo, O. "OPLS Force Field for Choline Chloride-Based Deep Eutectic Solvents" *J. Phys. Chem. B*, **2018**, *122*, (in press). [doi:10.1021/acs.jpcb.8b06647](http://pubs.acs.org/doi/abs/10.1021/acs.jpcb.8b06647)

About
-----
**Contributing Authors**: Brian Doherty and Orlando Acevedo*

**Funding**: Gratitude is expressed to the National Science Foundation (NSF CHE-1562205) for funding the project.

**Software License**:
OPLS-DES.
Copyright (C) 2018 Orlando Acevedo

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details. <http://www.gnu.org/licenses/>
