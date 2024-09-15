# iTransformer: Time-Series Forecasting with Electricity Consumption Data

## Project Overview
The **iTransformer** project implements a time-series forecasting model based on transformer architecture. It utilizes historical electricity consumption data to predict future trends using self-attention mechanisms to capture temporal dependencies.

## Table of Contents
1. [Introduction](#introduction)
2. [Repository Structure](#repository-structure)
3. [Setup and Installation](#setup-and-installation)
4. [Dataset](#dataset)
5. [Script Usage](#script-usage)
6. [Usage](#usage)
7. [Model Overview](#model-overview)
8. [Results](#results)

## Introduction
The **iTransformer** model is tailored for time-series forecasting tasks, specifically for predicting electricity consumption data. The use of self-attention mechanisms allows the model to handle long-range temporal dependencies effectively.

## Repository Structure

. ├── download-data.sh
├── iTransformer.ipynb
└── README.md

- **download-data.sh**: A bash script that downloads the `electricity.npy` dataset from Google Drive.
- **iTransformer.ipynb**: Jupyter Notebook implementing the iTransformer model for time-series forecasting.
- **README.md**: This file.

## Setup and Installation

### Prerequisites
- Python 3.x
- Jupyter Notebook
- NumPy
- Pandas
- TensorFlow (or PyTorch)
- `curl` for running the bash script

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/iTransformer.git
    cd iTransformer
    ```

2. Install the required dependencies:
    ```bash
    pip install numpy pandas tensorflow jupyter
    ```

3. Run the `download-data.sh` script to download the dataset:
    ```bash
    bash download-data.sh
    ```

## Dataset

### Electricity Dataset
The dataset (`electricity.npy`) contains historical electricity consumption data and is sourced from the paper ["Predicting Electricity and Traffic from Smart Meter and Traffic Data"](https://arxiv.org/abs/1910.03002).

## Script Usage

### Google Drive File Downloader Script
The provided script allows downloading files from Google Drive using file IDs.

For example, to download the electricity dataset:
bash
gdrive-get 1uJDqW4u2shjbA_Y27oIcq-QM2jgW4c9g electricity.npy



Usage
Open the Jupyter Notebook:
jupyter notebook iTransformer.ipynb

Model Overview
The iTransformer is built using a transformer architecture, which leverages self-attention to model long-range dependencies in time-series data.

Results
The notebook includes visualizations and performance metrics to evaluate the iTransformer model's predictions and accuracy.
