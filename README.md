# Coffee Bean Classification Project

This project aims to classify coffee beans using various machine learning techniques and image processing algorithms. It consists of two main components: feature extraction from coffee bean images and classification using these extracted features.

## Features

### Feature Extraction (`ml-feature-extraction.ipynb`)
- Extracts various features from coffee bean images including:
  - Texture features (LBP, GLCM, HOG, Gabor)
  - Color features (Color moments, histograms, coherence vectors, color name histograms)
  - Shape features (Hu moments, morphological features, Fourier descriptors, Zernike moments)
- Supports image preprocessing including resizing and optional denoising
- Implements data augmentation through horizontal flipping
- Processes images in batches to manage memory usage
- Saves extracted features to CSV files

### Classification (`ml-classifier.ipynb`)
- Implements various classification algorithms:
  - Random Forest
  - K-Nearest Neighbors
  - Decision Tree
  - Gradient Boosting
  - Extra Trees
  - XGBoost
- Performs model evaluation using metrics such as accuracy, precision, recall, F1 score, and MSE
- Supports k-fold cross-validation
- Compares performance of different feature sets and classifiers
- Saves results to an Excel file for easy analysis

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/coffee-bean-classification.git
   cd coffee-bean-classification
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Feature Extraction:
   - Open `ml-feature-extraction.ipynb` in Jupyter Notebook or JupyterLab
   - Adjust the `root_path` variable to point to your dataset directory
   - Run all cells to extract features and save them to CSV files

2. Classification:
   - Open `ml-classifier.ipynb` in Jupyter Notebook or JupyterLab
   - Ensure the paths to the CSV files generated in the feature extraction step are correct
   - Run all cells to perform classification and generate results

## Results

The classification results, including performance metrics for different models and feature sets, will be saved in an Excel file named `classification_results.xlsx`.

## Contributing

Contributions to improve the project are welcome. Please feel free to submit a Pull Request.