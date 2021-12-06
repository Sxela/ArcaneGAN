# ArcaneGAN
ArcaneGAN
ArcaneGAN v0.1 by [Alex Spirin](https://twitter.com/devdef)

This is a proof of concept release. 
The model is in beta (which means it's beta than nothin')

Here are some image pairs. I've specifically picked various images to see how the model performs in the wild, not on aligned and cropped faces.

![0_256_](https://user-images.githubusercontent.com/11751592/144793668-be43ba18-a8c3-4b37-ba95-fc7bf56c5648.jpg)
![258c27bcb658a86765361c1faca7b749fa3a36aaf07e975b408281c0a9c76513](https://user-images.githubusercontent.com/11751592/144793712-11f7438f-0f14-4a50-bae6-673a1461ba71.jpg)
![e42](https://user-images.githubusercontent.com/11751592/144793847-121d6c17-f2a2-484d-a2ed-35f53f27197c.jpg)
![ewewe](https://user-images.githubusercontent.com/11751592/144793886-e3063e9c-fcb7-4570-82cb-0bcc3bc42b58.jpg)
![maxresdefault](https://user-images.githubusercontent.com/11751592/144793912-c58ff819-1f13-4bf8-89da-643fe08889fa.jpg)
![photo_2021-11-16_19-32-15](https://user-images.githubusercontent.com/11751592/144793930-e85dcd44-3417-4bff-b170-e6b39a2f57ca.jpg)
![photo_2021-11-16_19-34-02](https://user-images.githubusercontent.com/11751592/144793943-63bdecf1-c5e0-4b05-8f31-0dd14fd8c124.jpg)
![photo_2021-11-16_19-34-33](https://user-images.githubusercontent.com/11751592/144793967-bdc73e78-abe9-4678-86cf-7fd71545963f.jpg)
![photo_2021-11-16_19-34-49](https://user-images.githubusercontent.com/11751592/144793979-c03216a1-414f-41c5-8f46-492d9be09d40.jpg)
![photo_2021-12-04_07-23-17](https://user-images.githubusercontent.com/11751592/144794058-1404130d-847b-4e3e-b66f-22e859c57666.jpg)
![photo_2021-12-04_07-48-29](https://user-images.githubusercontent.com/11751592/144794159-19d48ac0-79f2-4cc2-867b-fafb4acb9191.jpg)
![photo_2021-12-04_08-06-40](https://user-images.githubusercontent.com/11751592/144794243-b64b2cf9-2032-4022-9a34-94d65b283566.jpg)
![photo_2021-12-04_08-07-04](https://user-images.githubusercontent.com/11751592/144794253-600c0bc4-5176-4142-81d5-e389aaf1e917.jpg)
![photo_2021-12-04_11-26-27](https://user-images.githubusercontent.com/11751592/144794261-b6f868ca-8dfb-4ea2-9e60-66cf683b2569.jpg)


It does something, but not much at the moment. 

The model is a pytroch *.jit of a fastai v1 flavored [u-net](https://fastai1.fast.ai/vision.models.unet.html) trained on a paired dataset, generated via a blended stylegan2. You can see the blending colab I've used [here](https://github.com/Sxela/stylegan3_blending). 

Inference notebook is [here](https://colab.research.google.com/drive/1r1hhciakk5wHaUn1eJk7TP58fV9mjy_W?usp=sharing)
