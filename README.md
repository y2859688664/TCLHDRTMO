# High Dynamic Range Imaging & Tone Mapping: A Survey

> **[A Survey on High Dynamic Range Imaging and Tone Mapping Operators](https://arxiv.org/your-paper-link)**
>
> *<sup>1</sup>Your Lab, <sup>2</sup>University A, <sup>2</sup>University B*

**⚡We will actively maintain this repository and incorporate new research as it emerges. If you have any questions, please contact [your_email@domain.com]. Welcome to collaborate on academic research and writing papers together.**

## 📌 What is This Survey About?

<p align="center">
    <img src="TMO.png" width="100%" alt="Luminance Range and Human Vision">
</p>

<p align="center">
    <b>Figure 1: The Physical Basis of HDR.</b> <br>
    The real world exhibits a vast dynamic range of luminance, from starlight ($10^{-6} cd/m^2$) to sunlight ($10^{9} cd/m^2$). However, standard displays (CRT/LCD) cover a much narrower range. <b>Tone Mapping Operators (TMOs)</b> serve as the critical bridge, mimicking the human visual system's adaptive capabilities to compress this wide dynamic range into the visible gamut of display devices.
</p>

<br>

<p align="center">
    <img src="TMOpipline.jpg" width="100%" alt="HDR Imaging Pipeline">
</p>

<p align="center">
    <b>Figure 2: The Modern HDR Processing Pipeline.</b> <br>
    A comprehensive view of the image processing workflow:
    (1) <b>Acquisition</b>: Capturing raw data via Professional Cameras (RAW/Log) or Exposure Fusion.
    (2) <b>Processing</b>: Converting signals using transfer functions like <b>PQ (Perceptual Quantizer)</b> and <b>HLG (Hybrid Log-Gamma)</b>.
    (3) <b>LTM Core</b>: The central tone mapping stage, categorizing algorithms into Global, Local, and DNN-based methods to adapt content for both HDR (HDR10, Dolby Vision) and LDR displays.
</p>

<br>

High Dynamic Range (HDR) imaging is gaining increasing attention in both computer graphics and computational photography. Over the past few decades, significant efforts have been made to optimize the pipeline from capture to display. This paper presents a comprehensive review of the state-of-the-art methods, focusing on the evolution from traditional global operators to modern Deep Neural Network (DNN) approaches.

Finally, we discuss the limitations of current objective quality metrics (IQA) for tone-mapped images and explore promising future directions. Our key argument is that evaluation should be integrated into the design loop to better support the development of next-generation visual systems.

## HDR 数据集汇总

| Dataset | Years | Scene | Encode | Resolution | Public availability |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Narwaria** | | 10 | Linear | 1080×1920 | [Link](https://www.repository.cam.ac.uk/items/c2d00e29-07b5-4b67-bcfc-80893b17fa53) |
| **Korshunov** | | 20 | Linear | 1080×944 | [Link](https://www.repository.cam.ac.uk/items/c2d00e29-07b5-4b67-bcfc-80893b17fa53) |
| **Funt** | | 112 | ffmpeg-linear | 1421×2141 | [Link](https://www.cs.sfu.ca/~colour/data/funt_hdr/) |
| **HDRC** | | 80 | ffmpeg-linear | 1080×1920 | [Link](https://github.com/Yliu724/HDRC) |
| **MIT fiveK** | | 5000 | PQ | 3000×4000 | [Link](https://data.csail.mit.edu/graphics/fivek/) |
| **HDR-Eye** | | 46 | Linear | 512×512 | [Link](https://www.epfl.ch/labs/mmspg/downloads/hdr-eye/) |
| **HDR-gallery** | | 8 | ffmpeg-linear | 1536×2048 | [Link](https://pfstools.sourceforge.net/hdr_gallery.html) |
| **HDRQAD** | | 235 | ffmpeg-linear | 1080×944 | - |
| **HDRT** | | 10000 | Linear | 5120×3840 | [Link](https://huggingface.co/datasets/jingchao-peng/HDRTDataset) |
| **SJTU-HDR** | | 16 | PQ | 2160×3840 | [Link](https://medialab.sjtu.edu.cn/files/SJTU%20HDR%20Video%20Sequences/demo_images/) |
