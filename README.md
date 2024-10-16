# Multitask-Movie-Recommendation-System

## Overview
This repository hosts the implementation of a multitask learning approach for movie recommendations as part of the XCS330 course at Stanford University. The project investigates the impact of parameter sharing between different tasks within a movie recommendation model to enhance recommendation quality.

## Project Description
The goal of this project is to compare the performance of separate models against models with shared parameters under different configurations of factorization and regularization parameters. We implement and evaluate models based on matrix factorization and neural collaborative filtering techniques to predict user-movie interactions.

## Experimental Setup
The experiments focus on two main configurations:

- Lambda F = 0.99 and Lambda R = 0.01: Evaluates the impact of high regularization on model performance, particularly how it affects overfitting and generalization across tasks.
- Lambda F = 0.5 and Lambda R = 0.5: Examines a balanced approach to factorization and regularization to assess overall performance.

## Results
Experimental results demonstrate:

- Models without parameter sharing generally perform better on both training and test datasets, indicating possible overfitting when parameters are shared.
- The balanced approach (Lambda F = 0.5 and Lambda R = 0.5) tends to generalize better on unseen data, suggesting its effectiveness in managing overfitting compared to highly skewed regularization settings.

## Files and Directories
- `src/`: Source code including implementations and utility scripts.
- `data/`: Contains datasets used in training and evaluating the models.
- `results/`: Stores output results, including performance metrics and visualizations.

## Dependencies
- Python 3.8+
- PyTorch 1.7+
- NumPy
- Pandas

## Running the Experiments
To run the experiments, navigate to the `src/` directory and execute:

python run_experiments.py

## Citation
If you use this project or find it helpful, please cite it as:
Alevtyna Mozolyuk, "Multitask Movie Recommendation System," XCS330 Stanford University, 2023.

## Honor Code Notice
This project contains coursework from Stanford University. Users and contributors are advised that all work submitted in this course is expected to be the result of individual effort and independent thinking. Collaboration or reference to past solutions from other students or sources is discouraged and should adhere to Stanford University's honor code. For more information, please visit [Stanford's Community Standards](https://communitystandards.stanford.edu/policies-and-guidance/honor-code).

## Acknowledgments
Special thanks to the instructors and peers at Stanford University's XCS330 course for their guidance and support throughout this project.