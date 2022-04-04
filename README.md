# ArcaneGAN by [Alex Spirin](https://twitter.com/devdef)

Photos [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1r1hhciakk5wHaUn1eJk7TP58fV9mjy_W)

Videos [![Colab for videos](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ohKCiOwZrhM3pza4L93AHAfMkIkJ5YQF)

![visitors](https://visitor-badge.glitch.me/badge?page_id=sxela_arcanegan_repo)

**Changelog**
* 2022-04-04 Added a new image2image model training [url](https://github.com/aarcosg/fastai-course-v3-notes/blob/master/refactored_by_topics/CNN_L7_gan_feature-loss.md)
* 2021-12-27 Added [colab for videos](https://colab.research.google.com/drive/1ohKCiOwZrhM3pza4L93AHAfMkIkJ5YQF)
* 2021-12-25 ArcaneGAN v0.4 is [live](https://github.com/Sxela/ArcaneGAN/releases/tag/v0.4)
* 2021-12-14 Added [Video demo](https://huggingface.co/spaces/sxela/ArcaneGAN-video) on huggingface
* 2021-12-12 ArcaneGAN v0.3 is [live](https://github.com/Sxela/ArcaneGAN/releases/tag/v0.3)
* 2021-12-09 Thanks to [ak92501](https://twitter.com/ak92501) we now have a [huggingface demo](https://huggingface.co/spaces/akhaliq/ArcaneGAN)

## ArcaneGAN v0.4

The main differences are: 
- lighter styling (closer to original input)
- sharper result
- happier faces 
- reduced childish eyes effect
- reduced stubble on feminine faces 
- increased temporal stability on videos
- reduced mouth\teeth artifacts

### Image samples 
v0.3 vs v0.4

![v3-4](https://user-images.githubusercontent.com/11751592/146965930-f66dfd00-e55b-4b84-be83-aed925c08e3a.jpg)

### Video samples


https://user-images.githubusercontent.com/11751592/146966428-f4e27929-19dd-423f-a772-8aee709d2116.mp4



https://user-images.githubusercontent.com/11751592/146966462-6511998e-77f5-4fd2-8ad9-5709bf0cd172.mp4





## ArcaneGAN v0.3 

Videos processed by the huggingface video inference colab.


https://user-images.githubusercontent.com/11751592/145702737-c02b8b00-ad30-4358-98bf-97c8ad7fefdf.mp4



https://user-images.githubusercontent.com/11751592/145702740-afd3377d-d117-467d-96ca-045e25d85ac6.mp4


# Image samples

![arcaneganv03](https://user-images.githubusercontent.com/11751592/145726820-19c77a0e-f5cf-4da8-98c1-7c7d59fa3dfa.jpg)


Faces were enhanced via [GPEN](https://github.com/yangxy/GPEN) before applying the ArcaneGAN v0.3 filter.



## ArcaneGAN v0.2
The release is [here](https://github.com/Sxela/ArcaneGAN/releases/tag/v0.2)
![image](https://user-images.githubusercontent.com/11751592/144801598-3196be69-c462-4637-a267-f246a4460204.png)
![photo_2021-12-04_08-05-34](https://user-images.githubusercontent.com/11751592/144984175-0b063911-4654-499d-a98c-d2e12622dd31.jpg)
![photo_2021-12-04_07-23-17](https://user-images.githubusercontent.com/11751592/144984187-d1679d94-dcd4-43fc-9626-869380410a9b.jpg)
![weewq](https://user-images.githubusercontent.com/11751592/144984243-6387263b-0827-478a-ac1e-1ee93f9ddec6.jpg)

## Implementation Details 

The model is a pytroch *.jit of a fastai v1 flavored u-net trained on a paired dataset, generated via a blended stylegan2.

- Model architecture: [fastai v1 u-net](https://fastai1.fast.ai/vision.models.unet.html)
- Stylegan2 implementation used: [stylegan3 repo](https://github.com/NVlabs/stylegan3)
- Stylegan blending example: [stylegan3 blending](https://github.com/Sxela/stylegan3_blending)
- Paired image2image training: [fastai v1 superres notebook](https://github.com/aarcosg/fastai-course-v3-notes/blob/master/refactored_by_topics/CNN_L7_gan_feature-loss.md)

