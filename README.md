## AV_PRAT: ADFR Vina - Prepare Run Analyze Tool
AV_PRAT is a Windows app that provides a GUI for working with AutoDock Suite. 

### Pre-requisites
* Operating system: Windows 10 onwards.
* ADFR suite must be installed.
* Vina needs to be installed, if you would like to run Vina.

### Quick start
**Prep**: Preparation of input for docking. 
* ADFR path refers to the installation path of the ADFR suite. On Windows, e.g., this would be "c:\Program Files (x86)\ADFRsuite-1.0".
* Receptor PDB refers to the path of the protein PDB file. Once this file is selected, the Receptor PDBQT field would get auto filled. You may change the PDBQT file path, if required.
* Once the Receptor PDB and PDBQT file names are correctly specified, click prepare receptor to prepare the PDBQT file using the default options. 
* Ligand mol2 refers to the folder having the mol2 file(s). Once this folder is selected, the Ligand PDBQT field would get auto filled. You may change the PDBQT folder path, if required.
* Once the receptor and ligand preparation is done, click Launch AGFR to launch the AGFRgui for the docking grid set-up and preparation of the .trg file. 

**Dock ADFR**: Docking using ADFR
* This tab has options to dock ligands using the ADFR program available in the ADFR suite. 
* ADFR path refers to the installation path of the ADFR suite. On Windows, e.g., this would be "c:\Program Files (x86)\ADFRsuite-1.0".
* Ligand PDBQT refers to the path of the ligand PDBQT file(s) prepared in the previous step.
* Enter .trg file path which was prepared using the AGFRgui tool.
* Specify the Reference ligand (_optional_).
* Enter docking parameters; for details about these please refer to the ADFR manual.
* Confirm the path of the ADFR config file and click Generate config. Review the option in the newly created config file. This file would be used to run the docking calculations. This config file can be manually edited as well to change or add parameters, if required. 
* Once you are satisfied with the options in the config file, click Run ADFR to start the docking calculations. 

**Dock Vina**: Docking using Vina
* In the Enter Vina path field enter the path of the Vina executable. 
* ADFR path refers to the installation path of the ADFR suite. On Windows, e.g., this would be "c:\Program Files (x86)\ADFRsuite-1.0".
* Enter .trg file path which was prepared using the AGFRgui tool.
* Ligand PDBQT refers to the path of the ligand PDBQT file(s) prepared in the previous step.
* Enter the docking parameters for Vina, for details about these please refer to the Vina manual.
* Confirm the path of the Vina config file and click Generate config. Review the option in the newly created config file. This file would be used to run the docking calculations. This config file can be manually edited as well to change or add parameters, if required.
 * Once you are satisfied with the options in the config file, click Run Vina to start the docking calculations. 

**Analyze**: Analysis of the log files (.dlg) created by docking calculations. 
* Select the program that was used to run docking calculations. 
* In the Enter .dlg file enter the .dlg file created on running Vina OR enter the folder having .dlg files created using ADFR. 
* Confirm the output file name (.csv) and click Run.
