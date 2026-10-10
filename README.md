# Advanced-CNNs-and-Transfer-Learning

This project compares CNN training strategies and transfer learning methods for a 10-class image classification task using the Oxford-IIIT Pet dataset.

## Experiments
- **B1:** ResNet-18 from scratch
- **B2:** Feature extraction (ResNet-18)
- **B3:** Progressive fine-tuning (ResNet-18)
- **B4:** Fine-tuning with and without data augmentation (ResNet-18)
- **B5:** MobileNetV3-Small

## Evaluation
Models are evaluated using training and validation metrics, test Macro F1-score, and training duration.

## Requirements
Python, PyTorch, Torchvision, NumPy, Pandas, Matplotlib, scikit-learn, and Pillow.

## How to Run
1. Open the `.ipynb` notebook in Google Colab.
2. Select a runtime environment (T4-GPU).
3. Run the notebook cells in order.

## Files
- `.ipynb` => Experiment code and outputs
- `.pdf` => Technical report
- `raw_training_epoch_logs.csv` => Training metrics recorded per epoch
- `raw_metrics.csv` => All metrics from B1 - B5

## Dataset Note
The official trainval and test partitions were combined before creating internal stratified train, validation, and test splits. Therefore, the resulting test set is not the original official test set.
