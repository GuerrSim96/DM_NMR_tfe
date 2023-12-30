# MDS-PVT
MDS-PVT is a system designed for conducting Molecular Dynamics Simulations (MDS) to study Peptides in Variable fractions of Trifluoroethanol (PVT).
The system enables the generation of trajectories for peptides within aqueous or membrane-like environments.

The system is composed by three Notebooks:
1.  The first one needs to install the open source software GROMACS and to adds parameters of trifluoroethanol into the OPLS-aa force field;
1.  The second one is responsible to producing the trajectory of a molecular system using the functionality provided by GROMACS;
1.  The third one is dedicated to analyzing the conformational changes of the peptide throughout the trajectory obtained from the simulation.

The advantage of using this system is that it does not slow down the user's PC because the GROMACS is installed on the Google Drive and the calculations are carried out with the T4 GPUs made available to Google with Colaboratoory.

Furthermore, it is not necessary for the user to have in-depth knowledge of computational chemistry to use this system, the only thing he has to do is enter the pdb identification code of the peptide and enter the percentage of trifluoroethanol in which he wants to simulate.

## Tutorial
On this section we are going to see how easy it is to use the MDS-PVT system!
### GROMACS_Installation.ipynb
Before using this notebook, ensure you're logged into an account with ample free storage space. It's recommended to use an account specifically generated for this system, as GROMACS will be installed on it, and later, the produced simulation trajectories will be saved there.
