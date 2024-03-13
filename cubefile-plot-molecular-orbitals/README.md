# Plotting molecular orbitals from cube file data

![Isosurface of a localized molecular orbital representing one of the C-H bonds in the ethene molecule](example.png)

File orbitalplot-interactive.nb is a Mathematica notebook for plotting +/- isosurfaces of 
of a set of molecular orbitals. The image above shows +/-0.04 atomic units isosurfaces of a localized molecular orbital representing one of the C-H bonds in the ethene molecule, generated with the notebook.

*Notes: Mathematica Versions 12.x, 13.0, 13.3, and 14.0 are confirmed to work. In Mathematica 13.1, the combined rendering of molecules and isosurfaces based on cube file imports is broken; do not use. 13.2 works but the isosurfaces appear as if resulting from low-resolution data even if a high-resolution cube file is used. Updated versions will be made available as needed, as long as my research group and I continue to use the notebook for our research and educational projects.*

The notebook was used to generate the molecular orbital visualizations in my textbook *Quantum Theory for Chemical Applications* (https://global.oup.com/academic/product/quantum-theory-for-chemical-applications-9780190920807). The ethene orbital example is one of the isosurface plots shown in Figure 10.12 in the book. See also this article: https://doi.org/10.1021/ed200673w 

Numerical data for the orbitals must be provided in the form of data files in the commonly used 'cube' format (volume data + molecular frame).

![Screen shot of the interactive plotting panel in the notebook](screenshot.png)

The screenshot above shows the main interactive plotting panel of the notebook. The user can select different styles for plotting the molecular frame, select the isosurface values, rotate and scale the plot as desired, and there is a convenient button for saving the plot in its current orientation in PNG format. If the notebook's directory contains multiple cube files (they must all be for the same molecule, using the same grid for the volume data), it can be selected from a drop-down menu in the plot panel, preserving the viewpoint and other settings. This is very convenient when one wants to draw many different orbitals isosurfaces for the same molecule. 

There is additional code to save the current viewpoint, or to import it from a file saved during another interactive session. An accompanying notebook, multiple-cube-exports.nb, is also provided. You can use that notebook to generate images for a large set of cube files in one go. 

It happens occasionally (esp. for metal complexes, in my experience) that Mathematica generates too many or too few bond 'sticks' in the molecule drawing. In this case, please consult the instructions in `orbitalplot-interactive.nb` as well as the accessory notebook `import-molecule-modify.nb` (also provided in this repository) how to create a MOL format file with the desired bond connectivities and use this instead in the interactive plot program.

