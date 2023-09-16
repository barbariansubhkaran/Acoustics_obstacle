# Acoustics_obstacle
## Modeling of sound waves around an obstacle using OpenFOAM.

### This is an OpenFOAM case to model soundwaves using rhoPimpleFoam, compressible solver. 

Use the following commands:- 
```
  blockMesh
```

 
 The command creates the mesh using Hex elements. 
 ```
 decomposePar -force 
 ```
 This command divides the case into smaller chunks to make it run parallel on multiple cores. 
 ```
 mpirun -np 4 rhoPimpleFoam -parallel 
 ```
 This command runs the solver, a compressible sovler. 
 ```
  recontructPar
 ```
 This command reconstructs the case, ready for post processing. 
