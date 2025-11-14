# [Installing ModelMuse, MODFLOW and PEST](https://aselshall.github.io/gwh/hw/install-modflow)

## Introduction 

ModelMuse is a graphical user interface (GUI) for the family of MODFLOW-related programs: [Link](https://www.usgs.gov/software/modelmuse-a-graphical-user-interface-groundwater-models)

MODFLOW is the USGS's modular hydrologic model. MODFLOW is considered an international standard for simulating and predicting groundwater conditions and groundwater/surface-water interactions. The family of MODFLOW-related programs includes capabilities to simulate coupled groundwater/surface-water systems, solute transport, variable-density flow (including saltwater), aquifer-system compaction and land subsidence, parameter estimation, and groundwater management: [Link](https://www.usgs.gov/mission-areas/water-resources/science/modflow-and-related-programs)

PEST automates calibration, and uncertainty analysis of any numerical model: [Link](https://pesthomepage.org/)

## Tutorial

This tutorial will guide you through the installation of ModelMuse GUI, MODFLOW 2005 for groundwater flow simulation, and PEST for model calibration. 

### 1. Install ModelMuse
If you are using your personal laptop, install ModelMuse current release (e.g., v.5.1.1.0.): [Link](https://www.usgs.gov/software/modelmuse-a-graphical-user-interface-groundwater-models)

Alternatively, you can launch ModelMuse from appsanywhere. If ModelMuse (or any other program in general) is not working for you on appsanywhere, check out this Appsanywhere Troubleshooting document: [Link](https://docs.google.com/document/d/17gtyg7qrX9wtrEDqDxq8aKzqPHUJXndhRl_jwJ415Ao/edit?usp=sharing)
 
### 2. Download MODFLOW and related programs 

1) MODFLOW-2005
    - https://water.usgs.gov/water-resources/software/MODFLOW-2005/MF2005.1_12.zip
2) ModelMate
    - https://water.usgs.gov/water-resources/software/ModelMate/ModelMate_1_0_3.exe
3) PEST (Check PEST website for new version of PEST if the link to current version is not working) 
    - Current version (e.g., Version 18) of the PEST suite: https://s3.amazonaws.com/docs.pesthomepage.org/software/pest18.zip
    - 64-bit versions of some PEST-suite programs: https://s3.amazonaws.com/docs.pesthomepage.org/software/i64execs.zip
    - Groundwater Utilities: https://s3.amazonaws.com/docs.pesthomepage.org/software/gwutils.zip
    - PLPROC: https://s3.amazonaws.com/docs.pesthomepage.org/software/plproc.zip

### 3. Install ModelMate
Click on the executable file to install ModelMate at the selected location (e.g., C:/WRDAPP/)

### 4. Place programs in one folder 
Unzip the downloaded files and keep them together (e.g., C:/WRDAPP/). See the screenshot below as an example. 
<br>
<img width="724" height="679" alt="image" src="https://github.com/user-attachments/assets/1ec37fad-d5ca-4356-b51e-3b1e0b22539f" />
<br>
This screenshot shows additional MODFLOW related programs that you will not need for this project. For this project you only need MF2005.1_*, ModelMate_*, and pest17.
<b>
For PEST you need to have all PEST related programs under one folder (e.g., e.g., C:/WRDAPP/pest17). Keep all the executable files under pest17. 
<b>
<img width="910" height="658" alt="image" src="https://github.com/user-attachments/assets/f463f59d-48f2-47dd-84f6-521fc887dc44" />
<br>

**Error Message**
> Cannot find plproc
For plproc, make sure that plproc executable is under pest17 `\pest17\plproc.exe` (i.e., not under `\pest17\plproc\plproc.exe`). Otherwise, when you activate PEST, it will give you an error that `plproc` does not exist.

**Error Message** 
> A dot exist in file name or file path 
A dot “.” in your file path or file name will give you an error. Make sure that the file path to the model or PEST executables, as well as your project name do not contain a dot.

For example, with this file path you will get an error: 
> C:\Users\aelshall\CWR4540C.Fall2023\GW_Project\mc1.gpt
because your path has a dot in “CWR4540C.Fall2023”

With this file name you will get an error:
> C:\Users\aelshall\CWR4540C.Fall2023\GW_Project\mc.1.gpt
because your file name has a dot “mc.1”

This will work
> C:\Users\aelshall\CWR4540C_Fall2023\GW_Project\mc_1.gpt
By replacing the dot with underscore

### 5. Link MODFLOW and related programs to ModelMuse
Launch ModelMuse and link ModelMuse to the executables as follows. 
 
From `Model` -> `MODFLOW program locations`, make sure that ModelMuse knows your MODFLOW executable location (e.g., C:\WRDAPP\MF2005.1_12\bin\mf2005.exe) 

From `Model` -> `MODFLOW program locations`, make sure that ModelMuse knows your ModelMate executable location (e.g., C:\WRDAPP\ModelMate_1_0_3\Bin\ModelMate.exe) 

From `Model` -> `PEST Properties’ -> ‘PEST Directory’, make sure that ModelMuse knows the location of PEST executables (e.g., C:\WRDAPP\pest17)

This tutorial contains the installation instructions:
- https://www.youtube.com/live/47eb-QP6QqA

One thing missing from this video:
- Make sure that plproc executable is under pest17 `\pest17\plproc.exe` (i.e., not under `\pest17\plproc\plproc.exe`)

  
