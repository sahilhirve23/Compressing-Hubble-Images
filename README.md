# Compressing-Hubble-Images
Autoencoder-based Compression and Reconstruction of Hubble Telescope Images
This project leverages deep learning, specifically autoencoder architectures, to perform efficient compression and high-fidelity reconstruction of images captured by the Hubble Space Telescope. The methodology begins with preprocessing raw image data by converting to grayscale, resizing to 128×128 pixels, and normalizing pixel values to a [0, 1] range. These standardized inputs are then fed into an autoencoder, comprising two main components: an encoder that compresses the input into a low-dimensional latent representation, and a decoder that reconstructs the original image from this representation.

The training objective is to minimize the difference between the original and reconstructed images using a composite loss function. This loss function integrates:

Mean Squared Error (MSE): Measures pixel-wise reconstruction error

![{B7AE0764-4C0F-4BD6-BBA0-5F0E41F634D3}](https://github.com/user-attachments/assets/bc6125b3-d018-4114-85b8-4e496ff792e7)

Structural Similarity Index Measure (SSIM): Evaluates perceptual similarity based on luminance, contrast, and structure.

Perceptual Loss: Utilizes a pre-trained VGG network to capture high-level semantic and texture information that is perceptually important to human vision.

By optimizing this combined loss function, the model effectively learns to retain both low-level pixel accuracy and high-level structural details, resulting in visually faithful reconstructions. The implementation showcases the potential of deep learning in addressing the challenge of astronomical image compression, promoting efficient storage, enhanced accessibility, and improved dissemination of Hubble’s large-scale image datasets.

This work contributes meaningfully to the field of astronomical data management, highlighting how AI can enable smarter storage solutions without compromising image quality.

Here are the results demonstrating the performance of the proposed autoencoder-based compression and reconstruction approach


![download](https://github.com/user-attachments/assets/75d5996b-a137-468e-9b72-8ecd99625d8f)
