# Mushroom Classification using Decision Trees and Random Forests

This project implements custom Decision Tree and Random Forest classifiers from scratch to classify mushrooms as **edible** or **poisonous**. It uses both real-world (primary) and synthetic (secondary) datasets and evaluates models using multiple splitting criteria and visualizations.

## Files

- `mushroom.ipynb` – Main Jupyter notebook with full code for data preprocessing, EDA, model implementation, and experiments.
- `Machine Learning And Statistical Learning.pdf` – Final project report summarizing methodology, results, and insights.

## Features

- Custom implementation of:
  - Decision Tree Classifier
  - Random Forest Classifier
- Three splitting criteria:
  - Gini impurity
  - Entropy
  - Scaled entropy
- Comprehensive preprocessing and normalization pipeline
- Exploratory Data Analysis (EDA) with plots
- Grid search for hyperparameter tuning
- Heatmaps and learning curves to assess performance
- Confusion matrices and feature usage analysis
- Evaluation on separate train/validation/test splits

## Datasets

- **Primary Dataset**: Real mushroom species with 23 features, including cap shape, color, gill type, habitat, and season.
- **Secondary Dataset**: Augmented/synthetic data derived from the primary set, used for training and validation.

## Experiments

- Hyperparameter tuning across:
  - `max_depth = [3, 5, 7]`
  - `min_samples_split = [2, 5, 10]`
- Evaluation of Gini, Entropy, and Scaled Entropy criteria
- Comparison of model performance and generalization
- Random Forest ensemble with bootstrapping and feature subsampling

## Key Takeaways

- Scaled entropy often yields better validation performance than traditional Gini or Entropy.
- Random Forests outperform single trees in accuracy and robustness.
- The model favors predicting **poisonous**, a conservative and desirable bias for this classification task.

## License

This project is part of a university coursework and is for educational purposes only.
