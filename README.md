
# Coursework 2 – Data Science Project

## Project Overview

This project is an end-to-end data science and machine learning workflow completed as part of **Coursework 2**. The aim of the coursework is to demonstrate the ability to design, implement, document, and evaluate machine learning models using good software engineering and data science practices.

The project is fully version-controlled using GitHub and explores both traditional machine learning methods and neural networks on the same dataset. The final part of the project investigates a focused research question to gain deeper insight into neural network behaviour.

This repository is intended to be readable and reproducible, and the notebooks are written in a tutorial-style format aimed at progressively more advanced audiences.

## Dataset

The dataset used in this project is a **Spotify track popularity dataset**, sourced from **Kaggle**.

Each data point represents a Spotify track and includes a combination of:

* Numerical audio features such as danceability, energy, loudness, tempo, and acousticness
* Metadata features related to the track
* A target variable indicating whether a track is considered popular

This dataset was chosen because:

* It represents a real-world classification problem
* The feature–target relationships are likely to be non-linear
* It is well suited to both traditional machine learning models and neural networks
* It is large enough to train neural networks, while remaining interpretabl

## Research Questions

The coursework is structured around three questions:

### Q1 – Traditional Machine Learning

A traditional (non-neural network) machine learning approach is applied to the dataset. This provides a baseline model and allows comparison with more complex methods.

### Q2 – Neural Network Approach

A neural network model is developed and compared against the traditional approach from Q1, highlighting differences in performance and behaviour.

### Q3 – Research Question

How do training epochs and batch size affect the performance of a neural network?**

This research question explores whether commonly tuned training hyperparameters meaningfully impact neural network performance on this dataset. The investigation focuses on convergence behaviour, stability, and final test accuracy.

## Project Structure

The repository is organised as follows:

```
.
├── README.md                # Project overview and instructions
├── dependencies.txt         # Python dependencies and versions
├── py/
│   └── functions.py         # Shared helper functions (data loading, preprocessing, etc.)
├── Q1_folder/
│   └── Q1.ipynb             # Traditional ML approach (beginner audience)
├── Q2_folder/
│   └── Q2.ipynb             # Neural network approach (beginner audience)
├── Q3_folder/
│   └── Q3.ipynb             # Research question exploration (intermediate audience)
```

Each notebook is self-contained and can be run independently, while making use of shared helper functions where appropriate.

---

## Methodology Summary

* Data cleaning and preprocessing are applied consistently across all questions
* Numerical features are standardised
* Categorical features are encoded where required
* A fixed train–test split is used to allow fair comparisons

For Q3, the neural network architecture is kept constant while:

* The number of training epochs is varied
* The batch size is varied

This controlled approach ensures that observed performance differences can be attributed to training hyperparameters rather than architectural changes.

---

## Key Findings (Q3)

The results from Q3 show that:

* The neural network converges within a small number of epochs
* Increasing epochs beyond this point does not significantly improve test accuracy
* Changing batch size has minimal effect on final performance

These findings suggest that, for this relatively simple tabular dataset, training hyperparameters such as epochs and batch size are less influential than factors such as feature quality and model architecture.

---

3. Run notebooks in order:

* Start with `Q1_folder/Q1.ipynb`
* Then `Q2_folder/Q2.ipynb`
* Finally `Q3_folder/Q3.ipynb`

---

## Dependencies

All required Python libraries and versions are listed in `dependencies.txt`. The project was developed using standard data science and machine learning libraries including NumPy, pandas, scikit-learn, and TensorFlow / Keras.

---

## Notes on External Resources

External resources were used for learning and reference purposes only. Any ideas or code patterns inspired by external sources are appropriately adapted and referenced where relevant. No code was copied directly from Kaggle notebooks or other coursework submissions.

---

## Author

Up2119371
Brodey Evans

This project was completed as part of the MSc Data Science coursework and is intended for educational and portfolio purposes.
