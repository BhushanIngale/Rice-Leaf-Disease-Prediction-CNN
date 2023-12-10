
# Rice Leaf Disease Prediction using CNN

## Project Overview

### Business Problem

Create a model which can classify the three major attacking diseases of Rice plants like Leaf blast, Bacterial blight and Brown spot.

### Approach

This is a Image Classification problem which can be solved using Artificial Neural Networks.

## Installation & Setup

### Resources Used

- Editor/IDE: iPython Notebook on Google Colab
- Environment/Backend: TensorFlow Backend
- Python Version: 3.9

### Python Packages Used

- General Purpose: warnings, os, google.colab
- Data Wrangling: splitfolders, numpy
- Data Visualization: matplotlib
- Deep Learning: tensorflow, keras

## Data
- The Dataset consists of 120 jpg images of disease-infected Rice leaves.

- The images are grouped into 3 classes (Leaf Blast, Bacterial Blight and Brown Spot), based on the type of disease. There are 40 images in each class.

## Code Structure
```
├── data
│   ├── Bacterial leaf blight
│   ├── Brown spot
│   └── Leaf smut
├── model
│   └── model.h5
├── report
│   ├── Project-Report-Rice-Leaf-CNN.pptx
│   ├── Rice-Leaf-CNN-Report.pdf
│   └── model.png
├── src
│   ├── image_data
│   │   ├── Bacterial leaf blight
│   │   ├── Brown spot
│   │   └── Leaf smut
│   ├── output
│   │   ├── test
│   │   ├── train
│   │   └── val
│   └── Rice-Leaf-CNN.ipynb
├── .gitignore
└── README.md
```

## Results & Evaluation

### Model Comparison:

|  | Train Accuracy | Validation Accuracy | Test Accuracy | Epochs |
| --- | --- | --- | --- | --- |
| CNN with Sequential | 76.52 | 89.47 | 80.77 | 35 |
| `CNN with DenseNet201` | 97.39 | 100 | `96.15` | 5 |

### Challenges Faced:
- In order to improve accuracy, the Images had to be Augmented.
- Deciding the Number of Convolution Layers and Epochs for the Baseline Model was challenging.
- Small training dataset.
- Studied the concepts of Data Augmentation, Transfer Learning and Splitting the Image Data in Train-Val-Test-Split.

### Conclusion

We built a model that was able to identify Rice Leaf Disease Classes with 96% Accuracy. We selected the model that was based on the DenseNet201 since it provided a near perfect Accuracy and had a relatively lower time of execution.

## Future Work
Using Transfer Learning, different pre-trained models can be tested to further improve the accuracy.

## License

[MIT](https://choosealicense.com/licenses/mit/)

