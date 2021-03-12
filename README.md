# VesselGen

Please cite the following paper in which VesselGen is described:

Shen, J., Faruqi, A. H., Jiang, Y., & Maftoon, N. (2021). Mathematical Reconstruction of Patient-Specific Vascular Networks Based on Clinical Images and Global Optimization. IEEE Access, 9, 20648–20661. 
https://doi.org/10.1109/ACCESS.2021.3052501
https://ieeexplore.ieee.org/document/9328247 

This package reconstructs patient-specific vascular networks based on patient priors obtained through MR angiograms. It accepts clinical image in the `.nii.gz` format and outputs a network configuration file (`.npy`) as well as the generated mesh (`.stl`). It also supports 3-D rendering of the generated network with [Autodesk CAD](https://www.autodesk.in/) (package *Fusion 360*).

The package consists of a complete reconstruction pipeline that includes image processing, root and leaf node selection, multi-tree global constructive optimization, network model generation (3-D rendering), and network model analysis. Most of the scripts are written in python, with the optimization algorithm implemented in C.

To run the reconstruction process, the following additional software/packages are required:
* vesseg
* bin2mesh
* vmtk
* binvox
* thinvox

Then, follow the instructions in `VesselGen/pipeline.txt` step by step.
