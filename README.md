#  DNA Classifier using Deep Learning

This project builds a deep learning model to classify synthetic DNA sequences as either **human** or **non-human** using k-mer frequency encoding.

## Project Structure

notebook/      → Jupyter Notebook with full pipeline
data/          → Generated synthetic dataset (CSV)
models/        → Trained Keras model (.keras) + scaler (Pickle)

## Model Summary

- Data: 1000 synthetic DNA sequences (500 human, 500 non-human)
- Encoding: 3-mer frequency vector (64 features)
- Model: Feedforward Neural Network using TensorFlow/Keras
- Accuracy: 100% test accuracy on clearly separated synthetic data

##  How to Run

```bash
# Create virtual environment
conda create -n dnaenv python=3.10
conda activate dnaenv

# Install libraries
pip install -r requirements.txt

# Run the notebook
jupyter notebook notebook/dna_classifier_final.ipynb
