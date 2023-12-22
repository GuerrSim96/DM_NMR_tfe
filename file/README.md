# Description:
This folder contains the files needed to add trifluoroethanol (TFE) parameters within the OPLS-aa force field, and also the .pdb files needed to build the system to simulate in a mixture of TFE and water.
### atomtypes.atp 
![Static Badge](https://img.shields.io/badge/GROMACS%20customized%20file%20-%20%236495ED)  
In this file the identification codes of the atoms are associated with the corresponding atomic masses.  
The data is associated with the OPLS-aa force field.
### ffbonded.itp 
![Static Badge](https://img.shields.io/badge/GROMACS%20customized%20file%20-%20%236495ED)  
This file contains information related to bond lengths, bond angles, dihedrals, and force constants.  
The data is associated with the OPLS-aa force field.
### ffnonbonded.itp 
![Static Badge](https://img.shields.io/badge/GROMACS%20customized%20file%20-%20%236495ED)  
This file contains information on the chemical-physical properties of atoms, which are fundamental for non-bonded interactions.  
The data is associated with the OPLS-aa force field.
### residuetypes.dat ![Static Badge](https://img.shields.io/badge/GROMACS%20customized%20file%20-%20%236495ED)  
This input file presents a list of residues identified with a variable-length code.  
Each identifier is accompanied by a description specifying the nature of the compound.
### tip3p_added.pdb <sup> ![Static Badge](https://img.shields.io/badge/Custom--written%20file%20-%20%23B8860B) </sup>
This file presents the coordinates of a single water molecule.
### trifluoroethanol.itp
![Static Badge](https://img.shields.io/badge/Custom--written%20file%20-%20%23B8860B)  
This files are described respectively in the file chemical-physical properties of TFE molecule.  
The data is associated with the OPLS-aa force field.
### trifluoroethanol.pdb
![Static Badge](https://img.shields.io/badge/Custom--written%20file%20-%20%23B8860B)  
This files contains the three-dimensional arrangement of the atoms of TFE molecule.
