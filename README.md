# ArcaneGAN by [Alex Spirin](https://twitter.com/devdef)

[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1r1hhciakk5wHaUn1eJk7TP58fV9mjy_W)

**Changelog**
* 2021-12-09 Thanks to [ak92501](https://twitter.com/ak92501) we now have a [huggingface demo](https://huggingface.co/spaces/akhaliq/ArcaneGAN)

## ArcaneGAN v0.3 

Videos processed by the huggingface video inference colab.


https://user-images.githubusercontent.com/11751592/145702737-c02b8b00-ad30-4358-98bf-97c8ad7fefdf.mp4



https://user-images.githubusercontent.com/11751592/145702740-afd3377d-d117-467d-96ca-045e25d85ac6.mp4






## ArcaneGAN v0.2
The release is [live](https://github.com/Sxela/ArcaneGAN/releases/tag/v0.2)
![image](https://user-images.githubusercontent.com/11751592/144801598-3196be69-c462-4637-a267-f246a4460204.png)
![photo_2021-12-04_08-05-34](https://user-images.githubusercontent.com/11751592/144984175-0b063911-4654-499d-a98c-d2e12622dd31.jpg)
![photo_2021-12-04_07-23-17](https://user-images.githubusercontent.com/11751592/144984187-d1679d94-dcd4-43fc-9626-869380410a9b.jpg)
![weewq](https://user-images.githubusercontent.com/11751592/144984243-6387263b-0827-478a-ac1e-1ee93f9ddec6.jpg)

## Implementation Details 

It does something, but not much at the moment. 

The model is a pytroch *.jit of a fastai v1 flavored [u-net](https://fastai1.fast.ai/vision.models.unet.html) trained on a paired dataset, generated via a blended stylegan2. You can see the blending colab I've used [here](https://github.com/Sxela/stylegan3_blending). 

