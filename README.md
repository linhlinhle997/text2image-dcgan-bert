# Text to Image Synthesis using DCGAN-BERTs

## Introduction

This project explores text-to-image generation using Deep Convolutional Generative Adversarial Networks (DCGAN) combined with BERT-based text embeddings. It includes three main notebooks:

- **Base Model**: Uses a word-based tokenizer and Flickr8k dataset.

- **DCGAN-BERT**: Uses the Flowers dataset with BERT embeddings.

- **DCGAN-BERT with Wrong Image**: Extends DCGAN-BERT by incorporating incorrect image-caption pairs for training.

##  Datasets

**1. Flickr8k Dataset** (Used in `text2image_base_model.ipynb`)

- Contains 8,000 images with captions for training word-based text embeddings.

**2. Flowers Dataset** (Used in `text2image_dcgan_berts.ipynb` and `text2image_dcgan_berts_improve.ipynb`)

- Each image has multiple textual descriptions, encoded using BERT.

## Setup

### Run the Notebooks

1. Open and run the respective notebook in Jupyter or Colab.
2. The required dependencies will be installed automatically within the notebook.
3. The dataset will be downloaded and extracted within the notebook cells.
4. Execute all cells sequentially to train the model.

## Model Architecture

**Generator**

- Takes a combination of random noise and text embeddings to generate an image.

**Discriminator**

- Evaluates if an image is real or generated, using both image data and text embeddings.

## Results

- The model can generate images from text descriptions with good quality.
- Using BERT-based embeddings improves performance compared to a word-based tokenizer.
- Including incorrect images enhances the Discriminator’s ability to differentiate real vs. fake images.

