# A selection of State-ot-the-art, Open-source, Usable, and Pythonic techniques for Image Restoration

<p align="center">
<img src="https://github.com/titsitits/open-image-restoration/blob/master/Anne-Franck.png" width="800" />
</p>

## Description
This project gathers together and packages various image restoration techniques that follow various criteria:
* State-of-the-art (they are all based on Deep Learning; as of today (25/07/2019 at time of writing), NLRN and ESRGAN are leaders in various leaderboards maintained by paperswithcode.com, see [here](https://paperswithcode.com/paper/non-local-recurrent-network-for-image) and [here](https://paperswithcode.com/paper/esrgan-enhanced-super-resolution-generative) ).
* Open source (the selected implementations are under MIT or Apache licenses)
* Usable (a pretrained model is available, and the code does not need painfull<sup>1</sup> dependencies)
* Python implementation (easier to use together, to share, and especially to use in Google Colab).

## Demo
The project is a work in progress. However, it is already functional and **can be tested on your own images** through this **[demo in Google Colab](https://colab.research.google.com/github/titsitits/open-image-restoration/blob/master/ImageRestorationColab.ipynb)**.

## Technical details
The algorithms currently included in the packages are directly replicated or slightly adapted from external github repositories (see below). These methods were selected based on the above criteria, and after a comparison with other methods (comparison colab notebooks are coming soon). 

### 1. Denoising
NLRN - Liu et al. 2018. Non-Local Recurrent Network for Image Restoration (NeurIPS 2018) - MIT License

https://github.com/Ding-Liu/NLRN

https://paperswithcode.com/paper/non-local-recurrent-network-for-image

### 2. Colorization
DeOldify ("NoGAN" algorithm) - Jason Antic, 2019 - MIT License

https://github.com/jantic/DeOldify

(no leaderboard associated... yet).

### 3. Super-resolution
ESRGAN - Wang et al. 2018. ESRGAN: Enhanced super-resolution generative adversarial networks (ECCV 2018) - Apache-2.0 License

https://github.com/xinntao/ESRGAN

https://paperswithcode.com/paper/esrgan-enhanced-super-resolution-generative

Many thanks to the authors of these awesome contributions to image restoration research, and for sharing them as open-source projects. 

## More information

A more detailed comparison of State-of-the-art super-resolution algorithms can be found in this **[Google Colab Notebook](https://colab.research.google.com/drive/1x7wHaiJ-_rPfRqz1DcRJ_Hbq61t6lFKi)**.
A blog post (in french) presents an overview on the subject [here](https://titsitits.github.io/open-image-restoration/White%20paper%20-%20super-resolution%20(french)/Whitepapersuperresolution.html)

---

<sup>1</sup>: In my research of IR algorithms, I subjectively considered Matlab and Caffe as painfull dependencies. Matlab is simply not free (and simpy not usable in Google colab), and Caffe hard to install, especially in Google Colab. Both of these issues make the algorithms hard to share to the community.
