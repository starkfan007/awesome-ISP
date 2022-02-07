# Awesome-ISP (in progress)
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
  * [AE](#ae)
  * [BLC](#blc)
  * [LSC](#lsc)
  * [DPC](#dpc)
  * [AWB](#awb)
  * [Demosaic](#demosaic)
  * [CCM](#ccm)
  * [CSC](#csc)
  * [NR](#nr)
  * [HDR/Tone Mapping](#hdr-tone-mapping)
- [Datasets](#datasets)


## Courses, books & examples
### Courses
Stanford CS448A -- Computational photography [[Project Page]](http://graphics.stanford.edu/courses/cs448a-10/)  
### Books
Image sensors and signal processing for digital still cameras -- Junichi Nakamura [[pdf]](https://last.hit.bme.hu/download/firtha/video/Sensors/Junichi%20Nakamura%20Image%20sensors%20and%20signal%20processing%20for%20digital%20still%20cameras%20%202006.pdf)  
### Examples
openISP -- Open Image Signal Processor [[code]](https://github.com/cruxopen/openISP)  
fast-openISP -- Fast Open Image Signal Processor [[code]](https://github.com/QiuJueqin/fast-openISP)  
camera-pipeline -- A Software Platform for Manipulating the Camera Imaging Pipeline [[code]](https://karaimer.github.io/camera-pipeline/)  
ISP Pipeline -- Algorithms of ISP Pipeline [[code]](https://gitee.com/wtzhu13/ISPAlgorithmStudy)  
ISP-pipeline-hdrplus -- An open source (C / C + +) image algorithm library [[code]](https://github.com/jhfmat/ISP-pipeline-hdrplus)
## Open Source Camera Driver
V4L2 -- Video4Linux (V4L for short) is a collection of device drivers and an API for supporting realtime video capture on Linux systems [[code]](https://www.kernel.org/doc/html/v4.9/media/uapi/v4l/v4l2.html)  
HAL -- Android's camera hardware abstraction layer [[code]](https://source.android.com/devices/camera)  
libcamera -- A complex camera support library for Linux, Android, and ChromeOS [[code]](https://github.com/kbingham/libcamera)  
### Raw data decoder
MatRaw -- Read and Process Camera Raw Data with MATLAB [[code]](https://github.com/QiuJueqin/MatRaw)   
dcraw -- Decoding raw digital photos in Linux [[code]](https://github.com/ncruces/dcraw)  
LibRaw -- Library for reading and processing of RAW digicam images [[code]](https://github.com/LibRaw/LibRaw)  
Adobe DNG SDK -- The Adobe DNG SDK provides support for reading and writing DNG files as well as support for converting DNG data into a format easily displayed or processed by imaging applications [[code]](https://helpx.adobe.com/security/products/dng-sdk.html#Version15)
## Camera Pipeline
### End to End Pipeline
| Model                  | Published                                                    | Code                                                         | Keywords                                                     |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| CycleISP               | [CVPR 20](https://arxiv.org/pdf/2003.07761.pdf)            | [Pytorch](https://github.com/swz30/CycleISP)              | converting sRGB images to RAW data, and then back to sRGB images      | 
| MW-ISPNet              | [AIM 20](https://www.researchgate.net/publication/348895624_AIM_2020_Challenge_on_Learned_Image_Signal_Processing_Pipeline)            | [Pytorch](https://github.com/cszhilu1998/MW-ISPNet)              | Multi-level Wavelet Network |
| PyNET               | [CVPR 20](https://arxiv.org/pdf/1910.06663.pdf)            | [Pytorch](https://github.com/aiff22/PyNET-PyTorch)              | Replacing Mobile Camera ISP with a Single Deep Learning Model      | 
### AE
Simatest -- Simatest is designed to simulate exposures of a 'scene' made with a virtual camera. [[code]](https://github.com/imatest/simatest)  
Automatic Camera Exposure Control. [[code]](https://github.com/alexzzhu/auto_exposure_control)
### LSC
| Model                  | Published                                                    | Code                                                         | Keywords                                                     |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
|               | [TPAMI 09](https://www.eecis.udel.edu/~jye/lab_research/09/JiUp.pdf)            | [C++/Matlab](https://github.com/GUOYI1/Vignetting_corrector)              | Single-Image Vignetting Correction      | 
|               |             | [C](https://github.com/6by9/lens_shading)              | Lens shading analysis tool      | 
|               |             | [Qt](https://github.com/dridri/lens_shading_editor)              | Raspberry Pi camera lens shading table editor      |  
### AWB
- Survey

| Published                                                    |  Keywords                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [TIP 11](https://staff.fnwi.uva.nl/th.gevers/pub/GeversTIP11.pdf)            | Computational Color Constancy Survey and Experiments |
- Low-Level Statistics-Based Methods

| Model                  | Published                                                    | Code                                                         | Keywords                                                     |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| | [TIP 02](https://ieeexplore.ieee.org/document/1036047) | [C++](http://kobus.ca/research/programs/colour_constancy/)              | A comparison of color constancy algorithms      |  
|Fast Fourier Color Constancy | [CVPR 17](https://arxiv.org/abs/1611.07596) | [Matlab](https://github.com/google/ffcc)              | The Fast Fourier Color Constancy (FFCC) Matlab Toolbox  | 

- Characterized-Based Methods
### Demosaic
| Model                  | Published                                                    | Code                                                         | Keywords                                                     |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Linear Interpolation | [ICASSP 04](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/Demosaicing_ICASSP04.pdf) |              | High-Quality Linear Interpolation      | 
| Residual Interpolation              | [ICIP 13](http://www.ok.sc.e.titech.ac.jp/res/DM/RI.html)            |  [matlab](http://www.ok.sc.e.titech.ac.jp/res/DM/RI.html)             |  | 
| Directional Filtering and a posteriori Decision              | [TIP 07](http://elynxsdk.free.fr/ext-docs/Demosaicing/todo/Menon_Andriani_IEEE_T_IP_2007.pdf)            |  [Python](https://github.com/colour-science/colour-demosaicing)             |  | 
### CCM
| Model                  | Published                                                    | Code                                                         | Keywords                                                     |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Root/Polynomial | [TIP 15](https://eprints.ncl.ac.uk/file_store/production/211896/56A5026C-F3B9-4CB9-9A51-10F304877B45.pdf) | [matlab](https://github.com/QiuJueqin/color-correction-toolbox)  |  | 
| Colour Correction Toolbox | [AIC 17](https://ueaeprints.uea.ac.uk/id/eprint/65098/4/Colour_Correction_Toolbox.pdf)            |  [matlab](https://github.com/fangfufu/Colour_Correction_Toolbox)             | Multi algorithm integration | 
### NR(Code coming soon...)
#### Benchmark and Dataset

#### Noise model and estimation
Noise, Dynamic Range and Bit Depth in Digital SLRs [[Web Page]](https://homes.psd.uchicago.edu/~ejmartin/pix/20d/tests/noise/)  
A blog of Camera Noise [[Web Page]](https://zhuanlan.zhihu.com/p/23868867)
#### Filtering
- Bilatral filter
    - A Gentle Introduction to Bilateral Filtering and its Applications. Paris et al. SIGGRAPH 2008 Course Notes. [[code]](https://people.csail.mit.edu/sparis/bf_survey/)  
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
| Model                  | Published                                                    | Code                                                         | Keywords                                                     |
| ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Local Laplacian Filters | [SIGGRAPH 11](http://people.csail.mit.edu/sparis/publi/2011/siggraph/) | [matlab](http://people.csail.mit.edu/sparis/publi/2011/siggraph/) |       | 
| Advanced High Dynamic Range Imaging | [Book 17](https://dl.acm.org/doi/10.5555/3165066) | [matlab](https://github.com/banterle/HDR_Toolbox) | HDR Toolbox | 

