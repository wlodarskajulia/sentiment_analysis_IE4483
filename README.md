# Product Review Sentiment Classification

## Project Overview

This project implements sentiment classification of product reviews using three machine learning approaches:

- **Logistic Regression** – a baseline classifier using TF-IDF features.
- **Multi-Layer Perceptron (MLP)** – a neural network using TF-IDF features.
- **DistilBERT** – a pretrained transformer model fine-tuned for sentiment classification.

The models classify reviews as either negative (0) or positive (1).

## Project Structure

```text
.
├── data/
│   ├── train.json
│   └── test.json
├── notebooks/
│   ├── data_analysis.ipynb
│   ├── baseline_models.ipynb
│   ├── distilbert.ipynb
│   └── model_comparison_and_error_analysis.ipynb
├── requirements.txt
└── README.md
```

## Installation

1. Download and extract the ZIP file.
2. (Optional) Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

On Linux/macOS:

```bash
source .venv/bin/activate
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

## How to Run

Open the `notebooks` folder and execute the notebooks in the following order:

1. **data_analysis.ipynb** – explores the dataset and its characteristics.
2. **baseline_models.ipynb** – preprocesses the reviews, trains Logistic Regression and MLP, and saves the trained models.
3. **distilbert.ipynb** – tokenises the reviews, fine-tunes DistilBERT and saves the best-performing model.
4. **model_comparison_and_error_analysis.ipynb** – compares the models and analyses their classification errors.

The first three notebooks must be executed before the final comparison notebook, as it uses the models and files generated during training.

## AI Usage Declaration
AI tool (Claude) was used for stylistic improvements to the code, debugging assistance, and support with generating printed outputs and visualisations, including graphs, tables, LaTeX tables and confusion matrices. The code itself was written entirely by the group members. All experiments, result analyses, and conclusions were conducted and reviewed by the group.