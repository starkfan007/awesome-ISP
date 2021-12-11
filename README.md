# Awesome-ISP
A curated list of ISP good stuff. This list can contain anything related to the ISP and welcome pull requests.

## Content
- [Courses, books & examples](#tutorials--books---examples)
  * [Courses](#Courses)
  * [Books](#books) 
  * [Examples](#examples)
- [Open Source Camera Driver](#open-source-camera-driver)
- [Camera Pipeline](#camera-pipeline)
  * [End to End Piepeline](#end-to-end-pipeline)
  * [Raw data decoder](#raw-data-decoder)
  * [BLC](#blc)
  * [LSC](#lsc)
  * [DPC](#dpc)
  * [AWB](#awb)
  * [Demosaic](#demosaic)
  * [CCM](#ccm)
  * [CSC](#csc)
  * [NR](#nr)
  * [HDR/Tone Mapping](#hdr-tone-mapping)
- [Color Science](#color-science)
- [Image Quality Tuning](#image-quality-tuning)

## Courses, books & examples
### Courses
Stanford CS448A -- Computational photography [[Project Page]](http://graphics.stanford.edu/courses/cs448a-10/)  
### Books
[Image sensors and signal processing for digital still cameras -- Junichi Nakamura](https://last.hit.bme.hu/download/firtha/video/Sensors/Junichi%20Nakamura%20Image%20sensors%20and%20signal%20processing%20for%20digital%20still%20cameras%20%202006.pdf)  
[Image Processing for Embedded Devices -- Sebastiano Battiato](https://books.google.com/books/about/Image_Processing_for_Embedded_Devices.html?id=K5aOhnvGJToC)  
[Theory and Applications of Smart Cameras -- Kyung Chong-Min](https://www.springer.com/gp/book/9789401799867)  
### Examples
openISP -- Open Image Signal Processor [[code]](https://github.com/cruxopen/openISP)  
fast-openISP -- Fast Open Image Signal Processor [[code]](https://github.com/QiuJueqin/fast-openISP)  
camera-pipeline -- A Software Platform for Manipulating the Camera Imaging Pipeline [[code]](https://karaimer.github.io/camera-pipeline/)  
ISP Pipeline -- Algorithms of ISP Pipeline [[code]](https://gitee.com/wtzhu13/ISPAlgorithmStudy)  
## Open Source Camera Driver
V4L2 -- Video4Linux (V4L for short) is a collection of device drivers and an API for supporting realtime video capture on Linux systems [[code]](https://www.kernel.org/doc/html/v4.9/media/uapi/v4l/v4l2.html)  
HAL -- Android's camera hardware abstraction layer [[code]](https://source.android.com/devices/camera)  
libcamera -- A complex camera support library for Linux, Android, and ChromeOS [[code]](https://github.com/kbingham/libcamera)  
## Camera Pipeline
### End to End Pipeline
CycleISP -- Real Image Restoration via Improved Data Synthesis [[code]](https://github.com/swz30/CycleISP)  
### Raw data decoder
MatRaw -- Read and Process Camera Raw Data with MATLAB [[code]](https://github.com/QiuJueqin/MatRaw)   
dcraw -- Decoding raw digital photos in Linux [[code]](https://github.com/ncruces/dcraw)  
LibRaw -- Library for reading and processing of RAW digicam images [[code]](https://github.com/LibRaw/LibRaw)  
Adobe DNG SDK -- The Adobe DNG SDK provides support for reading and writing DNG files as well as support for converting DNG data into a format easily displayed or processed by imaging applications [[code]](https://helpx.adobe.com/security/products/dng-sdk.html#Version15)
### BLC
### LSC
lens_shading -- Lens shading analysis tool [[code]](https://github.com/6by9/lens_shading)  
lens_shading_editor -- Raspberry Pi camera lens shading table editor [[code]](https://github.com/dridri/lens_shading_editor)   
### DPC
### AWB
A comparison of computational color constancy algorithms [[Project Page]](http://kobus.ca/research/programs/colour_constancy/)  
Computational Color Constancy: Survey and Experiments [[Paper]](https://staff.fnwi.uva.nl/th.gevers/pub/GeversTIP11.pdf)  
Illumination Chromaticity Estimation using Inverse-intensity Chromaticity Space [[Code]](https://tanrobby.github.io/code/iic.zip) [[Project Page]](https://tanrobby.github.io/research/lightchroma/results.html)  
Edge-Based Color Constancy [[code]](https://github.com/lynnprosper/Edge-Based-Color-Constancy) [[Project Page]](https://ivi.fnwi.uva.nl/isis/publications/bibtexbrowser.php?key=vandeWeijerTIP2007&bib=all.bib)  
### Demosaic
High-Quality Linear Interpolation for Demosaicing of Bayer-Patterned Color Images [[code]](https://www.microsoft.com/en-us/research/publication/high-quality-linear-interpolation-for-demosaicing-of-bayer-patterned-color-images/)  
Residual Interpolation for Color Image Demosaicking [[code]](http://www.ok.sc.e.titech.ac.jp/res/DM/RI.html)  
A Python package implementing various CFA (Colour Filter Array) demosaicing algorithms and related utilities. [[code]](https://github.com/colour-science/colour-demosaicing)  
### CCM
Camera Color Correction Toolbox [[code]](https://github.com/QiuJueqin/color-correction-toolbox)  
Colour Correction Toolbox for AIC 2017 submission [[code]](https://github.com/fangfufu/Colour_Correction_Toolbox)  
Compute color correction matrix [[code]](https://github.com/lighttransport/colorcorrectionmatrix)  
### NR
#### Filtering
- Bilatral filter
    - A Gentle Introduction to Bilateral Filtering and its Applications. Paris et al. SIGGRAPH 2008 Course Notes  
    - A Fast Approximation of the Bilateral Filter using a Signal Processing Approach. Paris and Durand. MIT Tech Report 2006 (extends their ECCV 2006 paper)
- Guided filter
    - Guided image filtering(ECCV 2010).  Kaiming He et al.  
    - Fast Guided Filter.  Kaiming He et al.
- NLM
    - A non-local algorithm for image denoising (CVPR 05), Buades et al.  
    - Image denoising based on non-local means filter and its method noise thresholding (SIVP2013), B. Kumar
- BM3D
    - Image restoration by sparse 3D transform-domain collaborative filtering (SPIE Electronic Imaging 2008), Dabov et al.
#### Deep denoising
- DnCNN 
    - Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising (TIP2017), Zhang et al.
### HDR/Tone Mapping
HDR Toolbox is a MATLAB/Octave toolbox for processing High Dynamic Range (HDR) content [[code]](https://github.com/banterle/HDR_Toolbox)  
