# SAR-Flood-Detection
Overview

This project implements a deep learning pipeline to detect flooded areas from Synthetic Aperture Radar (SAR) imagery. The goal is to segment flood regions from pre- and post-flood SAR images, which can help in disaster monitoring and management.

The model is based on a 2-channel U-Net architecture, using pre-flood and post-flood SAR images as input. The pipeline includes data preprocessing, speckle noise filtering, model training, evaluation, and visualization of predictions.

Features

SAR-specific preprocessing: Lee filter to reduce speckle noise.

U-Net segmentation model: Predicts flood masks from pre- and post-flood images.

Train/validation split: Ensures proper model evaluation.

Metrics: Binary cross-entropy loss, validation accuracy, Dice score.

Visualization:

Side-by-side comparison of SAR images, ground truth, and predictions.

Overlay predictions on SAR images for intuitive understanding.

Extensible: Can be extended to UNet++ or Attention U-Net for improved performance.

Dataset

The dataset contains SAR pre-flood (A), post-flood (B) images, and corresponding flood masks (Label).

Images are grayscale PNGs, organized as:

/A     -> Pre-flood images
/B     -> Post-flood images
/Label -> Ground truth masks

