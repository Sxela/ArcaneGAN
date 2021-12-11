# ArcaneGAN by [Alex Spirin](https://twitter.com/devdef)

[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1r1hhciakk5wHaUn1eJk7TP58fV9mjy_W)

**Changelog**
* 2021-12-09 Thanks to [ak92501](https://twitter.com/ak92501) we now have a [huggingface demo](https://huggingface.co/spaces/akhaliq/ArcaneGAN)

## ArcaneGAN v0.3 

https://user-images.githubusercontent.com/11751592/145682185-363e7d07-54dd-4f39-ba96-4b71a2605bf2.mp4



## ArcaneGAN v0.2
The release is [live](https://github.com/Sxela/ArcaneGAN/releases/tag/v0.2)
![image](https://user-images.githubusercontent.com/11751592/144801598-3196be69-c462-4637-a267-f246a4460204.png)
![photo_2021-12-04_08-05-34](https://user-images.githubusercontent.com/11751592/144984175-0b063911-4654-499d-a98c-d2e12622dd31.jpg)
![photo_2021-12-04_07-23-17](https://user-images.githubusercontent.com/11751592/144984187-d1679d94-dcd4-43fc-9626-869380410a9b.jpg)
![weewq](https://user-images.githubusercontent.com/11751592/144984243-6387263b-0827-478a-ac1e-1ee93f9ddec6.jpg)


## ArcaneGAN v0.1 

This is a proof of concept release. 
The model is in beta (which means it's beta than nothin')

Here are some image pairs. I've specifically picked various images to see how the model performs in the wild, not on aligned and cropped faces.

![0_256_](https://user-images.githubusercontent.com/11751592/144793668-be43ba18-a8c3-4b37-ba95-fc7bf56c5648.jpg)
![258c27bcb658a86765361c1faca7b749fa3a36aaf07e975b408281c0a9c76513](https://user-images.githubusercontent.com/11751592/144793712-11f7438f-0f14-4a50-bae6-673a1461ba71.jpg)
![e42](https://user-images.githubusercontent.com/11751592/144793847-121d6c17-f2a2-484d-a2ed-35f53f27197c.jpg)
![ewewe](https://user-images.githubusercontent.com/11751592/144793886-e3063e9c-fcb7-4570-82cb-0bcc3bc42b58.jpg)

## Implementation Details 

It does something, but not much at the moment. 

The model is a pytroch *.jit of a fastai v1 flavored [u-net](https://fastai1.fast.ai/vision.models.unet.html) trained on a paired dataset, generated via a blended stylegan2. You can see the blending colab I've used [here](https://github.com/Sxela/stylegan3_blending). 

