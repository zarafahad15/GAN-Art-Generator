GAN Art Generator (DCGAN)

A PyTorch-based Deep Convolutional GAN (DCGAN) that generates abstract artwork from random noise. This project is designed for learning generative models and experimenting with AI-based image synthesis.

⸻

Features
	•	Fully implemented Generator and Discriminator
	•	Trains on CIFAR-10 or any custom image dataset
	•	Produces abstract, colorful images
	•	Uses PyTorch and torchvision
	•	Displays sample outputs during training

⸻

Architecture

Generator
	•	Takes a 100-dimensional noise vector
	•	Uses a series of ConvTranspose layers
	•	Produces 64×64 RGB images
	•	Follows the standard DCGAN generator structure

Discriminator
	•	Convolutional classifier
	•	Determines whether images are real or generated
	•	Uses LeakyReLU activations and BatchNorm
	•	Based on the original DCGAN design

⸻

Installation

git clone <your-repo-url>
cd gan-art-generator

pip install torch torchvision matplotlib


⸻

Usage

1. Run the training script

python train.py

2. During training
	•	Generated samples are displayed after each epoch
	•	Generator and discriminator loss values are printed

3. After training

Generated images will appear in the output window or can be saved manually within the script.

⸻

Sample Outputs

You may include outputs after training inside a samples/ directory, for example:

/samples
    epoch_1.png
    epoch_10.png
    epoch_50.png


⸻

Project Structure

.
├── train.py               # Main GAN training script
├── README.md              # Project documentation
└── data/                  # Dataset directory (created automatically)


⸻

Customization

You can modify the following parameters to suit your needs:
	•	Dataset (replace CIFAR-10 with your own images)
	•	Model depth and layer sizes
	•	Image resolution
	•	Number of training epochs
	•	Learning rate and optimizer parameters

If you want a customized model (anime generator, diffusion-based generator, or style-transfer version), I can provide an extended implementation.

⸻

License

This project is open-source. You may modify and reuse it for personal or educational purposes.

⸻
