# Image-Colorization-Using-GANs

This project implements Generative Adversarial Networks in order to colorize black and white images. In particular, I use a Conditional GAN on a Resnet U_Net generator backbone in order to train the model for a particular number of epochs. The original Pix2Pix paper doesn't use transfer learning in particular, rather just a UNet architecture that gets trained end to end along with the Discriminator. In this case, we remove the last 2 layers of a resnet Unet backbone and plug that in along with the discriminator.
If you wish to train or experiment with this notebook, just tweak the config class according to your needs. A detailed walkthrough is available in the notebook itself. Simply export it to colab, set it on a GPU and towards the end you can try your own image to see how well it produces the colors in comparison to the ground truth image


Dataset Used - COCO (10,000)

This notebook wouldn't have been possible without the resources mentioned below. These resources gave me key conceptual understandings of the loss functions, code, architectures as well as the paper implementations.

https://towardsdatascience.com/colorizing-black-white-images-with-u-net-and-conditional-gan-a-tutorial-81b2df111cd8
https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix
Paper : https://arxiv.org/abs/1611.07004

