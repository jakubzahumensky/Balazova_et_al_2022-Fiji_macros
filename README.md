Fiji (ImageJ) macros used for automated image analysis in:

**Balazova et al., 2022 – Two Different Phospholipases C, Isc1 and Pgc1, Cooperate To Regulate Mitochondrial Function**\
*Microbiol Spectr* 10(6):e0248922\
doi: [10.1128/spectrum.02489-22](https://doi-org.d360prx.biomed.cas.cz/10.1128/spectrum.02489-22)

---

Cell segmentation is performed using [Cellpose](https://github.com/MouseLand/cellpose/blob/master/README.md)

## Workflow
1. Run macro `1. export.ijm` to batch export your raw data to tiff format, as Cellpose works only with tiff/png.
2. Run macro `2. ROI_prep.ijm` to convert masks created by Cellpose to ROIs and save them through ROI manager.
3. Run the macro again to check the created ROIs frame by frame. They can be removed or adjusted. Additional ROIs can be added manually. All changes are saved automatically when "OK" is pressed in the prompt window.
4. Run `3. Quant.ijm` to run the quantification. It does not work in batch mode. After it is finished, a `Summary table` is saved in the directory specified when macro is run. The user is informed about successful finish with a window saying ***"Finito!"***.

## Notes
- It is advisable to run all macros from parent folder, not directly from the data folder.
- The macros are case-sensitive. The name of the folder folder with cell segmentation masks needs to be called `Masks` (i.e., the 'M' has to be capital; historical reasons)
- For the Quant macro to work, the folder with data needs to finish with 'data'

---
# Updates
The users are strongly recommended to use updated versions of these macros available [here](https://github.com/jakubzahumensky/microscopy_analysis).
Their use is described in detail in:

**Zahumensky & Malinsky, 2024 – Live cell fluorescence microscopy-an end-to-end workflow for high-throughput image and data analysis**\
*Biol Methods Protoc* 9(1):bpae075\
doi: https://doi.org/10.1093/biomethods/bpae075
