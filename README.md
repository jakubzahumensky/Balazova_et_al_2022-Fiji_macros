# Isc1_paper
FIJI macros used for automatic image analysis in Balazova et al., 2022 (https://doi.org/10.1016/j.jbc.2021.101462)

Cell segmentation is performed using Cellpose (https://github.com/MouseLand/cellpose/blob/master/README.md)

You can use macro "1. export" to batch export your raw data to tiff format, as Cellpose works only with tiff/png.
Use macro "2. ROI_prep" to concert masks created by Cellpose to ROIs and save them through ROI manager
Run the macro again to check the created ROIs frame by frame. They can be removed or adjusted. Additional ROIs can be added manually. All changes are saved automatically when "OK" is pressed in the prompt window
Run "3. Quant" to run the quantification. Does not work in batch mode. After it is finished, a Summary table is saved in the directory specified when macro is run. The user is informed about successful finish with a window saying "Finito!"

Notes:
It is advisable to run all macros from parent folder, not directly from the data folder.
The macros are case-sensitive. The name of the folder folder with cell segmentation masks needs to be called 'Masks' (i.e., the 'M' has to be capital; historical reasons)
For the Quant macro to work, the folder with data needs to finish with 'data'
