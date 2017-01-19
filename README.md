# Converge
CONVERGE study notes
***
## Introduction
### 1. This study is focusing on the Internal Combustion Engine modeling.

### 2. WHAT is CONVERGE: 

CONVERGE is a computational fluid dynamics (CFD) modeling program. CFD uses numerical methods and algorithms to solve and analyze problems involving fluid flow.

### 3. Advantages: 

1. Auto meshing.

2. User-friendly pre- and post- processor.
  
3. Automated geometry or parameter optimization.
  
4. Accurate physical models.
  
5. Detailed chemistry with large mechanisms.
  
### 4. What can CONVERGE do?
  
1. Customize, repair, or edit surface geometry
  
2. Steady-state or transient simulations
  
3. Simulations with large, moving/changing, and complex surface geometries

4. Advanced spray models
  
5. Conjugate heat transfer (CHT)
  
6. Combustion (multi-component fuel, non-premixed, fuel injection)
  
7. Detailed chemistry (SAGE)
  
8. Simplified combustion models (G-Equation, ECFM3Z, etc.)
  
9. Chemistry mechanism reduction
  
10. GT-SUITE coupling
  
11. 2-stroke and rotary engines
  
12. Engine knock analysis
  
13. Multi-phase flow simulations (Cavitation | Incompressible/compressible flows | Condensation/evaporation)
  
14. Complex mixing simulations (realistic turbulence)
  
15. Fluid-structure interaction (FSI)
  
16. User-defined functions (UDFs)
  
### 5. HOW to set up a case in CONVERGE Studio:

1. Import *.dat or *.stl geometry file
  
2. Import input (*.in) and data (*.dat) files if available
  
3. Repair and prepare geometry
  
4. Configure input files in ***Case Setup***
  
5. Export input and data files
  
### 6. What post-processing tasks can I do in CONVERGE Studio?

1. Create and export 2D plots
  
2. Calculate values such as apparent heat release and engine work

3. Post-convert data for 3D visualization
  
4. Launch EnSight for 3D visualization

***

## CONVERGE Studio Overview

### 1. The case setup module

1. Use the Case Setup module to set up and repair the surface geometry and to configure the input files

2. Because the CONVERGE solver creates the mesh automatically at runtime, you do not need to create a mesh

3. Save your project in this module as a \*.cvg file (a CONVERGE Studio- specific format)
   
  Note: CONVERGE and other programs are unable to open *.cvg files
   
4. Use the tools in the Geometry dock to prepare the geometry

  a. Create or delete entities
   
  b. Resize or move portions of the surface
  
  c. Repair surface defects 
  
  d. Flag boundaries
  
  e. Etc.
  
5. Work through the ***Case Setup*** dock to set up the case
  
  a. Select physical models
  
  b. Define boundary conditions
  
  c. Set up grid control options
  
  d. Specify post-processing parameters
  
  e. Etc.

6. Export input files, including the geometry file, to your ***Case Directory***

7. The CONVERGE solver will read the input files

### 2. The Line Plotting Module

1. Use the Line Plotting module to create and export 2D plots of simulation data

2. This module reads data from the CONVERGE \*.out files or any other columnbased text files

3. Save your work in this module as a \*.psp file

4. The Line Plotting module contains helpful features you can initiate

  a. Updates a plot with new data while the simulation is running

  b. Creates multi-directory plots to compare data sets from different simulations on the same plot

  c. Combines data sets from multiple output files (e.g., from several restarts) to create plots

  d. Calculates the FFT, apparent heat release rate, and engine work
  
### 3. The Post-Processing 3D Module

1. Use the Convert button to post convert binary output files 

2. Launch EnSight from Post-Processing 3D module

  Note: you can use other 3D visualization programs such as GMV, FieldView, Tecplot, or Paraview
   
***

## CONVERGE Studio Workflow

### 1. Case Setup Module

#### 1.1 Begin a project

* Begin a project

  Open a new project or an existing \*.cvg project

* View docks

  Geometry dock: Manipulate geometry

  Diagnosis dock: Identify problems with the geometry

  Case Setup dock: Configure physical models, initial conditions, and other parameters

  Coordinate Cache dock: Store coordinates and vectors from the geometry

  View Options dock: Change the view of the geometry
  
* View a Log
  
  Message log: Displays information regarding the status of each operation
  
  Import log: Displays information regarding the imported *.in and *.dat files except surface.dat

  Case setup issues: Displays warnings and errors, each accompanied by a link, regarding case setup

#### 1.2 Import the surface geometry

***The following notes will neglect detailed process, but only state the topic of the ppt.***

* Import the surface geometry file

* Mouse control

* How to select an entity with the *Objects Toolbar*

#### 1.3 Prepare the surface

1. Flag triangles to boundaries

  * How to flag boundaries (Mark Fence and Flag)
  
  * How to hide/show flagged triangles
  
2. Translate, rotate, and scale geometry

3. Find and repair surface defects

  * Intersections
  
  * Nonmanifold edges
  
  * Normal orientation
  
  * Open edges
  
  * Overlapping triangles
  
  * Isolated triangles
  
  * Aspect ratio
  
  * Small area
  
  * Small angle
  
  * Repair surface defects options using geometry dock and diagnosis dock
  
4. Save project (\*.cvg) and export surface.dat

#### 1.4 Configure case setup

#### 1.5 Export input and data files to the Case Directory

### 2. Run CONVERGE simulation

### 3. Line Plotting module

### 4. Post-Processing 3D module

***

## Questions:

### 1. 'Automated geometry or parameter optimization'. Does this mean that CONVERGE will automatically change the geometry of the model?

### 2. 'Import input (\*.in) and data (\*.dat) files if available'. What are these files?

### 3. Configure input files in *Case Setup*

### 4. 'Export input files, including the geometry file, to your ***Case Directory***'. What is Case Directory?

### 5. Do we have any Mac version of CONVERGE?
