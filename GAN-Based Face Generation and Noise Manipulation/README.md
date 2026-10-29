# GAN-Based Face Generation and Noise Manipulation

## 📌 Project Overview

This project explores Generative Adversarial Networks (GANs) for synthetic face image generation using TensorFlow and Keras. It consists of two notebooks: one for building and training a GAN, and another for generating images using a pretrained generator and experimenting with different noise inputs.

The project demonstrates the fundamentals of generative deep learning, model training, image generation, and latent noise manipulation through visual experiments.

## 🎯 Objectives

- Understand the generator and discriminator components of a GAN.
- Build a convolutional GAN architecture using TensorFlow and Keras.
- Preprocess and normalize image data for model training.
- Generate synthetic images from random noise vectors.
- Experiment with noise offsets and nonlinear noise transformations.
- Compare generated images using visualizations.

## 🛠️ Technologies Used

- **Language:** Python
- **Deep Learning:** TensorFlow, Keras
- **Numerical Computing:** NumPy
- **Visualization:** Matplotlib
- **Techniques:** Generative Adversarial Networks (GANs), Convolutional Neural Networks (CNNs), Image Generation, Noise Manipulation

## 📂 Project Structure

```text
GAN-Based-Face-Generation/
├── 10_Creative_AI_Generating_Art_with_Neural_Style_Transfer___Training.ipynb
├── 10_Creative_AI_Generating_Art_with_Neural_Style_Transfer___Inference.ipynb
└── README.md
```

## 📓 Project Notebooks

### 1. Training Notebook

**Purpose:** Build and train a GAN to generate synthetic images.

Key components:
- Load and preprocess image data.
- Define the generator and discriminator neural networks.
- Implement binary cross-entropy loss functions and Adam optimizers.
- Train the networks using gradient-based optimization.
- Configure distributed training using TensorFlow's `MirroredStrategy`.
- Visualize generated images during training.
- Save the generator model for later use.

### 2. Inference Notebook

**Purpose:** Generate synthetic face images using a pretrained generator.

Key components:
- Load a pretrained generator from `generator_700.h5`.
- Generate images using 100-dimensional random noise vectors.
- Explore different noise offsets to observe output variations.
- Compare original and manipulated noise inputs.
- Generate image grids using random noise samples.
- Apply sinusoidal and exponential transformations to explore nonlinear noise variations.
- Visualize the generated outputs using Matplotlib.

## ⚙️ How It Works

1. **Input Noise:** Random noise vectors are sampled from a normal distribution.
2. **Image Generation:** The generator transforms each noise vector into a synthetic image.
3. **Training Feedback:** During GAN training, the discriminator evaluates real and generated images, and both networks update their weights.
4. **Noise Manipulation:** During inference, changes to the noise vectors produce different generated outputs.
5. **Visualization:** Generated images are displayed in individual plots and image grids.

## 📊 Experiments

The inference notebook explores the following experiments:

- **Random Image Generation:** Generate individual synthetic face images.
- **Noise Offset Variations:** Add different offsets to a base noise vector and compare the resulting images.
- **Original vs. Manipulated Noise:** Add a shared random noise vector to input samples and visualize the outputs alongside the originals.
- **Nonlinear Noise Variations:** Combine sinusoidal and exponential transformations to create variations in the input noise.
- **Image Grid Generation:** Display multiple generated samples for visual comparison.

## 🚀 Setup and Execution

### Prerequisites

- Python 3.x
- TensorFlow
- NumPy
- Matplotlib
- Jupyter Notebook or Google Colab
- GPU support for the configured two-GPU distributed training setup

### Install Dependencies

```bash
pip install tensorflow numpy matplotlib tqdm
```

### Run the Project

1. Open the training notebook in an appropriate environment.
2. Configure the image dataset path and execute the preprocessing and training cells.
3. Save the trained generator checkpoint.
4. Open the inference notebook.
5. Clone the pretrained generator repository and load the available checkpoint.
6. Run the generation and noise-manipulation experiments.

**Note:** The training notebook saves `generator_800.h5`, while the inference notebook loads `generator_700.h5` from a separate repository. These are different checkpoints, so the inference workflow does not automatically use the model saved by the training notebook.

The training code also explicitly configures two GPUs; the environment must provide both devices for that configuration to work as written.

## 💡 Key Learnings

- Understanding the roles of generators and discriminators in GANs.
- Building convolutional neural networks for image generation.
- Understanding loss functions and gradient-based model optimization.
- Using random noise vectors as inputs to a pretrained generator.
- Exploring how input perturbations affect generated images.
- Visualizing synthetic image outputs using Python libraries.

## 🔮 Future Improvements

- Connect the training and inference notebooks using the same saved checkpoint.
- Evaluate generated image quality using suitable quantitative metrics.
- Experiment with different GAN architectures and training parameters.
- Explore structured latent-space interpolation and more controlled image variations.
- Improve training stability and compare generated samples across training epochs.

## 👩‍💻 Author

**Nandini Gupta**

- GitHub: [nandini17404](https://github.com/nandini17404)
- LinkedIn: [Nandini Gupta](https://www.linkedin.com/in/nandini-gupta-976aab275/)

---

⭐ If you find this project useful, consider giving the repository a star.
