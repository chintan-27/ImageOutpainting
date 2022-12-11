# ImageOutpainting

This project uses Deep learning to outpaint an image. Image outpainting is one of the topics of research that still has a lot to work on. It is a process of making an AI model learn to imagine what lies beyond the boundary of the image. This project proposes solutions to the problem of image outpainting using GANs, generative adversarial networks. The project proposes 3 GANs with different layouts and approaches, of which 2 GANs give promising results.

## 1. DC-GAN

C-GAN is an extension of standard GAN. In DC-GAN the generator and discriminator models have convolutional layers and transposed convolutional layers respectively.

## 2. GAN-2

The GAN-2 uses one generator, one global discriminator, four local discriminators, and one concatenator. The generator inputs a 256x256x4 masked and preprocessed image and outputs a 256x256x3 outpainted image.

### Plots

<img src="https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/DCGAN2/ValLoss.png" alt="Generator Loss" width="400"/>

### Results

![GAN-2 Result 1](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/DCGAN2/dcgan2-2.gif) ![GAN-2 Result 1](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/DCGAN2/dcgan2-3.gif)

## 3. GAN-3

The third GAN uses a single generator and discriminator but uses weighted adversarial loss.

### Results

![GAN-3 Result input](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/GAN3/images/train_0_masked.jpg) ![GAN-3 Result Output](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/GAN3/images/train_0_result.jpg) ![GAN-3 GT](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/GAN3/images/train_0_truth.jpg)
## 
![GAN-3 Result input](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/GAN3/images/val_1_masked.jpg) ![GAN-3 Result Output](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/GAN3/images/val_1_result.jpg) ![GAN-3 Result GT](https://github.com/chintan-27/ImageOutpainting/blob/main/Submission/Results/GAN3/images/val_1_truth.jpg)

## Conclusion

In this project, we successfully solved the problem of image outpainting using GANs. The GANs really proved to be true to their properties of generating data similar to the training set. The results can be improved using the whole dataset for training.

The detailed Report is available here - [Report]()
