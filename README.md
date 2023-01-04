# Acoustics_obstacle
Modeling of sound waves around an obstacle using OpenFOAM.

This is an OpenFOAM case to model soundwaves using rhoPimpleFoam, compressible solver. 

Use the following commands:- 

 1. blockMesh 
 
 The command creates the mesh using Hex elements. 
 
 2. decomposePar -force 
 
 This command divides the case into smaller chunks to make it run parallel on multiple cores. 
 
 3. mpirun -np 4 rhoPimpleFoam -parallel 
 
 This command runs the solver, a compressible sovler. 
 
 4. recontructPar
 
 This command reconstructs the case, ready for post processing. 
