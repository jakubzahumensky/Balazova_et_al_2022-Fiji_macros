# Isc1_paper
FIJI macros used for automatic image analysis in Balazova et al., 2022

Cell segmetnation is performed using Cellpose (https://github.com/MouseLand/cellpose/blob/master/README.md)

You can use maro "1. export" to batch export your raw data to tiff format, as Cellpose works only with tiff/png.
Use macro "2. ROI_prep" to concert masks created by Cellpose to ROIs and save them through ROI manager
Run the macro again to check the created ROIs frame by frame. They can be removed or adjusted. Additional ROIs can be added manually. All changes are saved automatically when "OK" is pressed in the prompt window
Run "3. Quant" to run the quantification. Does not work in batch mode. After it is finished, a Summary table is saved in the directory specified when macro is run. The user is informed about successful finish with a window saying "Finito!"

Notes:
It is advisable to run all macros from parent folder, not directly from the data folder.
The macros are case-sensitive. The folder with cell segmentation masks need to have a capital M (historical reasons)
For the Quant macro to work, the folder with data needs to finish with "data"
