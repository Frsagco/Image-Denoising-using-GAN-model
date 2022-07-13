# Image Denoising using GAN model
This code is developed as a master degree course project (Machine Learning for Vision and Multimedia) at Politecnico di Torino. \
Contributors:
- *Aglieco Francesco*.
- *Comparetto Alessandra*.
- *Gagliardi Giuseppe*.

Gan model based on:
- **Generator**: simplified U-Net structure.
- **Discriminator**: image classification CNN.

Noise used are *gaussian*, *salt and pepper* and *spackle*. 

Losses used on training step: 
- Discriminator loss: binary cross-entropy.
- Generator loss: content loss, using a VGG19 pre-trained model as feature extractor. 

Images are cropped in 256x256x3 dimension, cropping window is randomly seated.\
**COCO** dataset is used as train/test set.\
**BSD300** dataset is used as second test set.\ 

Main features: 
- Efficient loading of dataset on Drive folders after previous download. 
- Saving and loading on Drive folders of model trained epoch by epoch (in order to deal with low resource allocated by Google Colab).
- Content Loss enforces performance results. 

Details are written on pdf files located in this repo. 

![Alt text](https://github.com/Frsagco/Image-Denoising-using-GAN-model/blob/main/noise_image.png?raw=true "Title")
![Alt text](https://github.com/Frsagco/Image-Denoising-using-GAN-model/blob/main/denoised_image.png?raw=true "Title")
