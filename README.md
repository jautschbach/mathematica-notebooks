# Mathematica notebooks

This repository provides a collection of Mathematica notebooks that
I developed for our research projects. If you use and adapt them for your
own research, I would appreciate it if you cite some of the references 
provided in the README files in the sub-directories or in the Mathematica notebooks themselves. 

The collection of notebooks includes the following (yes, I'm a chemist ... ;-): 

https://github.com/jautschbach/mathematica-notebooks/tree/main/crystal-field-hamiltonian : Given the coordinates and charges of the ligands surrounding a metal center in a complex, this notebook will calculate the one-electron crystal-field (CF) Hamiltonian, the spin-orbit (SO) Hamiltonian for a p-, d- or f-shell, and the eigenfunctions and eigenvalues for the combined CF and SO interaction. 

https://github.com/jautschbach/mathematica-notebooks/tree/main/cubefile-interpolate-then-plot : Explore data in a volume data file in CUBE format visually. This notebook has no specific visualization target; it can be used to visualize the volume data in many different ways.

https://github.com/jautschbach/mathematica-notebooks/tree/main/cubefile-plot-2D-slices : This notebook reads CUBE format volume data and creates visualizations in user-specified two-dimensional slices (cut-planes). The images can be rotated in 3D if so desired. Multiple cube files can be visualized in the same plot. 

https://github.com/jautschbach/mathematica-notebooks/tree/main/cubefile-plot-complex-orbitals : Given the real and the imaginary part of a complex molecular orbital (MO) in separate 'cube' format files, this notebook will visualize the complex MO by drawing an isosurface of the MO's absolute value and color it by the complex phase of the MO at the isosurface points. The molecular frame is visualized together with the isosurface. The notebook can also be used to find and save a suitable view of the molecule & orbitals, which can then be used in the non-interactive notebook `multiple-cube-exports.nb` from the same folder to generate a large number of images relatively quickly without further input.

https://github.com/jautschbach/mathematica-notebooks/tree/main/cubefile-plot-molecular-orbitals : Interactive plot and PNG export of molecular orbital volume data in the 'cube' file format. The interactive panel has a variety of options for the plot and allows the generation of many 'cube' file plots for the same molecule in a short time. I used the notebook to generate the MO visualizations for my textbook *Quantum Theory for Chemical Applications* 

https://github.com/jautschbach/mathematica-notebooks/tree/main/tensor-plots : Given a molecular structure in XYZ format, and a rank-2 tensor, this notebook visualizes the tensor in the form of a polar diagram along with the molecule. 
