<h1 align="center">
  MDS-pVT
</h1>

<p>
MDS-pVT is a system designed for conducting Molecular Dynamics Simulations (MDS) to study peptides in Variable fractions of Trifluoroethanol (pVT).  
The system enables the generation of trajectories for peptides within aqueous or membrane-like environments.<br>
  The system is composed by three Notebooks:
<ol>
  <li>The first one results in installing the open source software GROMACS and to adds parameters of trifluoroethanol into the OPLS-aa force field;</li>
  <li>The second one is responsible to produce the trajectory of a molecular system using the functionality provided by GROMACS; </li>
  <li>The third one is dedicated to analyzing the conformational changes of the peptide throughout the trajectory obtained from the simulation.</li>
</ol>
The advantage of using this system is that it does not slow down the user's PC because the GROMACS is installed on the Google Drive and the calculations are carried out with the T4 GPUs made available to Google with Colaboratoory.<br> 
Furthermore, it is not necessary for the user to have in-depth knowledge of computational chemistry to use this system, the only thing he has to do is enter the pdb identification code of the peptide and enter the percentage of trifluoroethanol in which he wants to simulate.
</p>

<p align="center">
  <img src="https://github.com/GuerrSim96/MDS-PVT/blob/main/other/logo/basic_MDS-pVT.png"/>
</p>

---
<body font-family="serif">
<h2 align="center">
  TUTORIAL
</h2>

<p align="center">
On this section we are going to see how easy it is to use the MDS-pVT system! 
<table align ="center"> 
  <tr>
    <th> </th>
    <th> Notebook </th>
    <th> Description </th>
  </tr>
  <tr>
    <td>
      <a href="https://github.com/GuerrSim96/MDS-pVT/blob/main/GROMACS_installation.ipynb">
        <img src="https://img.shields.io/badge/Take_a_look-dodgerblue?logo=github&labelColor=gray"/>
      </a>
    </td>
    <td> GROMACS_Installation.ipynb </td>
    <td> Install GROMACS on your Drive </td>
  <tr>
    <td>
      <a href="https://github.com/GuerrSim96/MDS-pVT/blob/main/Molecular_Dynamics_Simulation_with_Trifluoroethanol.ipynb">
        <img src="https://img.shields.io/badge/Take_a_look-dodgerblue?logo=github&labelColor=gray">
      </a>
    </td>
    <td> Molecular_Dynamics_Simulation_with_Trifluoroethanol.ipynb </td>
    <td> Run MD simulations on Colab </td>
  </tr>
  <tr>
    <td>
      <a href="https://github.com/GuerrSim96/MDS-pVT/blob/main/trajectory_analysis.ipynb">
        <img src="https://img.shields.io/badge/Take_a_look-dodgerblue?logo=github&labelColor=gray">
      </a>
    </td>
    <td> trajectory_analysis.ipynb </td>
    <td> Analyze the trajectory on Colab </td>
  </tr>
</table> 
</p>

---

<h3>
  GROMACS_Installation.ipynb
  <a href="https://colab.research.google.com/github/GuerrSim96/Molecular_Dynamics_Simulation_with_Trifluoroethanol/blob/main/GROMACS_installation.ipynb">
    <img src="https://img.shields.io/badge/Open_it-goldenrod?logo=googlecolab&labelColor=gray"/>
  </a>
</h3>

<p>
Once you open the notebook you need to change the "runtime" type by choosing the T4 GPU option, as shown in the GIF below.  
</p>


<!-- CAPIRE COME CONVERTIRE IN HTML DA QUI -->
> [!IMPORTANT]
> Before using this notebook, ensure you're logged into an account with ample free storage space.
> The MDS-pVT system requires approximately 1.95 GB for installation on the drive, and each simulation saves on the drive from 0.37 GB to 1.82 GB of data size.

> [!TIP]
> It's recommended to use an account specifically generated for this system, as GROMACS will be installed on it, and later, the produced simulation trajectories will be saved there.
<!-- A QUI -->

<p>
<img src="other/gif/change_runtime.gif"/>
Then, simply press the <kbd>Ctrl</kbd>+<kbd>F9</kbd> keys to run all the cells in the notebook. Just wait a few minutes (approximately 90 minutes), and the notebook will have completed its job. <br>
Perfect, you have just installed GROMACS on your drive!  
</p>

<!-- CAPIRE COME CONVERTIRE IN HTML DA QUI -->
> [!WARNING]
> Before proceeding with the second notebook, ensure that the entire 1.95 GB of GROMACS files has been successfully loaded onto the drive.  
<!-- A QUI -->

---

<h3>
  Molecular_Dynamics_Simulation_with_Trifluoroethanol.ipynb
  <a href="https://colab.research.google.com/github/GuerrSim96/Molecular_Dynamics_Simulation_with_Trifluoroethanol/blob/main/Molecular_Dynamics_Simulation_with_Trifluoroethanol.ipynb">
    <img src="https://img.shields.io/badge/Open_it-goldenrod?logo=googlecolab&labelColor=gray"/>   
  </a>
</h3>

<p>
With this notebook, we will generate a simulation based on a few inputs that you need to enter! Now, I'll guide you through it in five simple steps: 
<ol>
 <li> Enter the alphanumeric PDB identification code of the peptide;<br>
   <img src="other/gif/insert_pdb_id.gif"/>
 </li>
 <li>Specify the percentage of TFE to be inserted into the system for simulation;<br>
    <img src="other/gif/tfe_percentage.gif"/>
 </li>
 <li> If you have a Colab subscription, check the "extended_simulation" box to extend the simulation time (optional);<br>
   <img src="other/gif/optional.gif"/>
 </li>
 <li> Ensure that the "runtime" is set to "T4 GPU," then press <kbd>Ctrl</kbd>+<kbd>F9</kbd> to run all cells;<br>
   <img src="other/gif/set_runtime.gif"/>
 </li>
 <li> Click on the URL that appears as the last row output from the "Mount the Drive" cell. A new window will open, where you need to select the account on which you installed GROMACS with the previous notebook. Afterward, click on the 'allow' button.<br>
   <img src="other/gif/drive_mounted.gif"/>
 </li>
</ol>
</p>

---

<h3> 
  trajectory_analysis.ipynb 
  <a href="https://colab.research.google.com/github/GuerrSim96/Molecular_Dynamics_Simulation_with_Trifluoroethanol/blob/main/trajectory_analysis.ipynb">
    <img src="https://img.shields.io/badge/Open_it-goldenrod?logo=googlecolab&labelColor=gray"/>
  </a>
</h3>

<p>
  This last notebook will allow you to extrapolate structural information about the peptide during its trajectory. To upload the simulation files to Colab to proceed with the analysis, follow the example shown in the GIF below.
  <img src="other/gif/upload.gif">
</p>

<!-- CAPIRE COME CONVERTIRE IN HTML DA QUI -->
> [!WARNING]
> If there is no subfolder, simply press <kbd>Enter</kbd>.
<!-- A QUI -->

With this Notebook you can:

<h4>
  Analyze Compactness and Flexibility:
</h4>
<p>
<ul>
  <li>Radius of inertia;</li>
  <li>Root Mean Square Deviation (RMSD);</li>
  <li>Root Mean Square Fluctuation (RMSF);</li>
  <li>Solvent-accessible surface area (SASA).</li>
</ul>
</p>

<h4>
  Analyze Secondary Structure:
</h4>
<p>
<ul>
  <li>Ramachandran angle analysis;</li>
  <li>Secondary structure assignment using the DSSP algorithm.</li>
</ul>
</p>

<h4>
  Analyze Trajectory:
</h4>
<p>
<ul>
  <li>PCA to visualize the trajectory.</li>
</ul>
</p>

<h2 align="center">
  Coming soon
</h2>
<p>
  In the future, a Docker file will be implemented to facilitate the simulation of larger protein systems on high-performance computers using this system.  
</p>

<h2 align="center">
  Reporting Issues or Requesting Analysis
</h2>
<p>
  If you encounter any issues with the system or wish to request an analysis on another aspect of the trajectory, we encourage you to send us an email at <b>GuerrSim96@gmail.com</b>. We will be happy to assist you and continually improve this project.
</p>
</body>
