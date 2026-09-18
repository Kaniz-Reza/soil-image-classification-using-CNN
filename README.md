# Soil Classification Using Convolutional Neural Networks

A deep learning-based soil classification system using Convolutional Neural Networks (CNNs)
to classify soil types from images. The project compares two pre-trained models (ResNet50,
VGG19) against two custom-built CNN architectures across two Kaggle soil-image datasets.

## Results

**Dataset 1** (alluvial, black, clay, red soil):

| Model | Test Accuracy |
|---|---|
| ResNet50 | 98.08% |
| VGG19 | 94.87% |
| Custom Model 1 | 88.46% |
| Custom Model 2 | 83.97% |

**Dataset 2** (black, cinder, laterite, peat, yellow soil):

| Model | Test Accuracy |
|---|---|
| ResNet50 | 98.81% |
| VGG19 | 97.86% |
| Custom Model 1 | 76.72% |
| Custom Model 2 | 71.73% |

## Models

- **ResNet50** - pre-trained, transfer learning
- **VGG19** - pre-trained, transfer learning
- **Custom Model 1** - 4-layer CNN built from scratch
- **Custom Model 2** - 5-layer CNN with Batch Normalization, built from scratch

## Project Structure

```text
soil-image-classification-using-CNN/
|-- README.md
|-- .gitignore
|-- requirements.txt
|-- notebooks/
|   |-- dataset1_predictions.ipynb
|   |-- dataset2_predictions.ipynb
|-- report/
|   |-- soil-classification-report.pdf
|   |-- latex/              (LaTeX source: main.tex, references.bib, figures/)
|-- data/
|   |-- README.md           (dataset sources, not included due to size)
|-- results/
    |-- figures/             (confusion matrices, accuracy/loss curves)
```

## Technologies

- Python
- PyTorch, torchvision
- Jupyter Notebook
- NumPy, Pandas
- Matplotlib
- Scikit-learn

## Dataset

Two Kaggle soil-image datasets:
- **Dataset 1**: 1,550+ images across four soil types.
- **Dataset 2**: 4,200+ images across five soil types.

See `data/README.md` for details. Datasets themselves are not included in
this repo due to size - refer to the notebooks and report for sources and preprocessing steps.

## Report

The full research paper (with methodology, literature review, and complete results) is available at
`report/soil-classification-report.pdf`.

## Author

**Kaniz Reza Mithila**
Department of Computer Science, East West University, Dhaka, Bangladesh
(CSE475 course project)