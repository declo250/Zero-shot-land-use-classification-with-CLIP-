# Zero-Shot Land-Use Classification Using CLIP for Remote Sensing

## Overview

This project explores the application of a vision-language model (CLIP) for zero-shot land-use classification using satellite imagery. The goal is to investigate whether a pretrained model can recognize different land-use categories without task-specific training.

Unlike traditional supervised classification methods that require large amounts of labeled data, vision-language models learn relationships between images and text descriptions. This project investigates their potential for remote sensing applications where labeled datasets can be limited and expensive to create.

## Research Question

Can a pretrained vision-language model such as CLIP perform zero-shot classification of satellite images without additional fine-tuning?

## Dataset

The experiments use the **EuroSAT dataset**, which contains Sentinel-2 satellite images covering 10 land-use and land-cover classes:

- Annual Crop
- Forest
- Herbaceous Vegetation
- Highway
- Industrial
- Pasture
- Permanent Crop
- Residential
- River
- Sea/Lake

Dataset source:
https://github.com/phelber/EuroSAT

## Methodology

The project follows these steps:

1. Load a pretrained CLIP vision-language model.
2. Encode satellite images into visual embeddings.
3. Create text prompts representing possible land-use categories.
4. Compare image and text embeddings using cosine similarity.
5. Assign the class with the highest similarity score.
6. Evaluate classification performance.

## Technologies

- Python
- PyTorch
- Hugging Face Transformers
- OpenAI CLIP
- Google Colab
- NumPy
- Matplotlib

## Model

The main model used in this project:

- CLIP ViT-B/32

CLIP was selected because it learns a shared representation between images and natural language, allowing zero-shot prediction without additional training.

## Results

The project evaluates:

- Zero-shot classification accuracy
- Confusion between land-use categories
- Example predictions
- Comparison with traditional CNN-based approaches (planned)

## Future Work

Possible extensions include:

- Fine-tuning CLIP on remote sensing datasets
- Testing other vision-language models
- Comparing CLIP with CNN and Vision Transformer baselines
- Exploring image-text retrieval tasks
- Evaluating model performance across different geographic regions

## Motivation

This project was developed as part of my preparation for research in computer vision and remote sensing. It represents my exploration of how modern vision-language models can be applied to Earth observation problems.

## Author

Jean Claude Ntabanganyimana

Master's Degree in Computer Science  
University of Łódź, Poland

GitHub:
https://github.com/declo250

## Project Structure
