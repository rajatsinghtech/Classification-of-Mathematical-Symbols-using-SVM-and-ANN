> Written manually, without AI assistance.

# Classification of Mathematical Symbols using SVM and ANN

## What this does

Presents and compares two classifier families â€” Support Vector Machines and
Artificial Neural Networks â€” on mathematical-symbol image classification,
trained on three feature types: Histogram of Oriented Gradients (HOG), Local
Binary Patterns (LBP), and raw pixel values.

## Business process

Symbol images go in; a predicted symbol class comes out. The report walks
the full arc: why feature extraction matters for image classification, how
HOG/LBP/pixels differ, how SVM and ANN work on these features, then measured
results per feature type so the reader can see which combination wins.

## Technical flow

`image_preprocessing.py` builds the HOG/LBP/pixel feature sets;
`svm_model.ipynb` and `ANN.ipynb` train and evaluate each classifier (HTML
exports alongside for reading without Jupyter). Dependencies are pinned in
`requirements.txt` (scikit-learn, TensorFlow/Keras, OpenCV, PyTorch
ecosystem).

## Repository structure

- [`svm_model.ipynb`](svm_model.ipynb) / [`svm_model.html`](svm_model.html)
  â€” SVM experiments
- [`ANN.ipynb`](ANN.ipynb) / [`ANN.html`](ANN.html) â€” neural-network
  experiments
- [`image_preprocessing.py`](image_preprocessing.py) â€” feature extraction
- [`requirements.txt`](requirements.txt) â€” pinned dependencies

## How to run

Install `requirements.txt`, then open the notebooks in order: preprocessing
first then either model notebook.
