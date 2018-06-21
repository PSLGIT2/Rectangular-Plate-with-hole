# APDL - Rectangular Plate with Hole

The following data was used to perform the (non)-linear FEM-Analysis.

  - Wide : 100 mm 
  - Thickness : 10 mm
  - Hole : 20 mm diameter 

#  Element Data
Element-type Plane183 is used
"PLANE183 is a higher order 2-D, 8-node or 6-node element. PLANE183 has quadratic displacement behavior and is well suited to modeling irregular meshes (such as those produced by various CAD/CAM systems)." [Ansys-Help]

# Material Data
  - Youngs-Module : 210000 N/mm^2 
  - Poisson-Ratio : 0.3
  - Hole : 20 mm diameter 

# Mesh
  - For the mesh a mapped mesh is used to reduce the element number
```sh
LESIZE,5,,,14                
LESIZE,1,,,7                 
LESIZE,8,,,14,0.2            
LESIZE,10,,,14,0.2           
LCCAT,7,11                   
MSHKEY,1                     
AMESH,All  
```
# Boundary Conditions
- 100 N/mm² Pressure on the right side


# Solution
