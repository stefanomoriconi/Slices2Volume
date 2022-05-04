# Slices2Volume
Concatenate a sequence of 2D images (slices) e.g. jpeg into a 3D stack (volume) e.g. Nifti (ITK-based)

The executable requires ITK (https://itk.org/) to be compiled and can be configured with CMake (https://cmake.org/)

Test the executable on the available testing data (TestData.zip)
- Decompress the archive
- After compilation, run in the terminal: ./Slices2Volume /TestData/slice%03d.jpg 0 149 /TestData/volume.nii.gz
