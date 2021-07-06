# Visualization of Blood Vessels in *in-vitro* Raw Speckle Images Using an Energy-based on DWT Coefficients

This repository has the functions to implement the methods described in the conference article: [*Visualization of Blood Vessels  in in-vitro Raw Speckle Images Using an Energy-based on DWT Coefficients*](https://www.sciencedirect.com/science/article/pii/S1746809421004894), developed as part of the project *"Visualization and localization of blood vessels"* at [INAOE](https://www.inaoep.mx). 


## Abstract
The visualization and localization of blood vessels is an important task to determine the presence and the health status of microvasculature in the biological tissue. Laser Speckle Contrast Imaging is one of the most widely employed techniques to study blood vessels; even so, it has some drawbacks in analyzing deep blood vessels (>100 µm) since the image noise level increases.
The Wavelet Approach is a model of automatic denoising for contrasted *in-vitro* Raw Speckle images using an energy criterion. The criterion selects the more suitable denoising level from the Discrete Wavelet Transform decomposition using the detail coefficients. Then, the segmentation of low-noise images by mathematical morphology techniques establish the blood vessel and biological tissue location. Finally, the region corresponding to the blood vessel and the low-noise images are used to improve the visualization of blood vessels.
Results show that a Wavelet Approach improves the visualization of blood vessels up to a depth of 400 µm. Furthermore, the proposed model demonstrates that the automatic denoising criterion improves the localization of superficial (>100 µm) and deep (>100 µm) blood vessels.

[[Paper]](https://www.sciencedirect.com/science/article/pii/S1746809421004894)

---

## Contents

* [`f_WA.m`](https://github.com/friscolt/elsevier-wavelet/blob/main/f_WA.m) -  Matlab script. The script  `f_WA.m` contains **1 main function (`f_WA`) and 8 auxiliary functions (`f_skavg`, `f_denoising`, `f_energy`, `f_thresholding`, `f_resize`, `f_segmenting`, `f_ratio`, `f_improving`)** to implement the methods described in [this paper](https://github.com/friscolt/elsevier-wavelet/blob/main/preprint.pdf). 

* [`data.mat`](https://github.com/friscolt/elsevier-wavelet/blob/main/data.mat) - MAT file. It contains three variables. 
  *  `im_raw`, contains a package of 30 *in-vitro* speckle images of a bifurcated vessel at a depth of 0µm. The image is a 288x280x30 pixels.
  *  `im_gt`, contains the ground truth of the *in-vitro* speckle image of a bifurcated vessel. The image is a 288x280 pixel logical type matrix.
 
* [`demo.mlx`](https://github.com/friscolt/elsevier-wavelet/blob/main/demo.mlx) - Matlab live script. It contains an example of the image processing available in [`data.mat`](https://github.com/friscolt/elsevier-wavelet/blob/main/data.mat). This live script describes step by step the use of the auxiliary functions described in [`f_WA.m`](https://github.com/friscolt/elsevier-wavelet/blob/main/f_WA.m). 

 
## Organization

No additional content directories are declared. 


## Contributors

Code for algorithms, applications and tools contributed by:

[Francisco Javier Lopez-Tiro](https://scholar.google.es/citations?user=IlG06bYAAAAJ&hl=es), [Hayde Peregrina-Barreto](https://scholar.google.es/citations?user=Wh2blp0AAAAJ&hl=es), [Jose de Jesus Rangel-Magdaleno](https://scholar.google.es/citations?user=aBNkfEsAAAAJ&hl=es), and [Julio Cesar Ramirez-San-Juan](https://scholar.google.es/citations?user=xN03bqgAAAAJ&hl=es)

Please email us your comments, criticism, and questions at [`francisco.lopez@inaoe.mx`](mailto:francisco.lopez@inaoe.com?subject=[GitHub]%20elsevier-wavelet%20repository)


## Reference

If you use functions from this script in your work, please use the BibTex entry below for citation.

[[Paper]](https://www.sciencedirect.com/science/article/pii/S1746809421004894)

```

```
