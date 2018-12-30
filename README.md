This is the project repository of Nikhil Sardana, Jerry Jiang, and Nathan Dalal, for the fall 2018 course [CS 236](https://deepgenerativemodels.github.io/). The final report is available [here](https://github.com/nikhilsardana/GANcompression/finalreport.pdf).

Forked from [nvidia/pix2pixhd](https://github.com/nvidia/pix2pixhd).

# Overview

Our original project goal was to improve the inference time of the Extreme Learned Image Compression model (open-source implementation available [here](https://github.com/Justin-Tan/generative-compression)). Since the encoder and decoder architecture of the [Agustsson et al.](https://arxiv.org/abs/1804.02958) model was based on the global generator network from pix2pixHD, we focused our efforts on trying to improve the image generation time of pix2pixHD without decreasing image quality.

Our modifications to the pix2pixHD generator included:
- Reducing/Adding upsampling/downsampling layers
- Replacing the Residual blocks with Dense blocks
- Varying the growth rate of the Dense blocks
- Varying the number of Dense blocks
- Adding spectral normalization to the Discriminator

Results are available in the final report pdf.
