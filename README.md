# AI Internship - Week 4 & Week 5

This repository has my work for the 6-Week AI Internship. **Week 4** is about classic Machine Learning models and how to evaluate them. **Week 5** is about Deep Learning and Neural Networks.

**Tools used:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras, Jupyter Notebook

## Repository Structure
```
AI-Internship
├── README.md
├── Week 4 - AI/
│   ├── Task1_Algorithms_Report/      (PDF report)
│   ├── Task2_Classification/         (notebook, iris.csv, predictions, screenshots)
│   ├── Task3_Regression/             (notebook, student_marks.csv, predictions, screenshots)
│   ├── Task4_Evaluation/             (notebook, comparison tables, screenshots)
│   ├── Task5_Mini_Project/           (notebook, dataset, predictions, screenshots)
│   ├── Project_Report.pdf  Week4_ML_Project.ipynb  Dataset.csv  Screenshots/  README.md
└── Week 5 - AI/
    ├── Task1_Fundamentals_Report/    (PDF report with diagrams)
    ├── Task2_Basic_Neural_Network/   (notebook, iris.csv, saved model, screenshots)
    ├── Task3_Train_and_Visualize/    (notebook, training history, graphs)
    ├── Task4_Evaluation_and_Prediction/ (notebook, predictions, confusion matrix)
    ├── Task5_Mini_Project/           (notebook, digits.csv, predictions, screenshots)
    ├── Project_Report.pdf  Week5_NN_Project.ipynb  Dataset.csv  Screenshots/
```

---

# Week 4 - Machine Learning Algorithms & Model Evaluation

| Task | What I did | File |
|---|---|---|
| 1. ML Algorithms | 2-page PDF explaining Logistic Regression, Decision Tree, KNN and Linear Regression | `Task1_Algorithms_Report/Project_Report.pdf` |
| 2. Classification | Iris dataset, Logistic Regression and Decision Tree (both 96.67% test accuracy) | `Task2_Classification/` |
| 3. Regression | Linear Regression on a student marks dataset to predict final marks, with plots | `Task3_Regression/` |
| 4. Evaluation | Accuracy, precision, recall, confusion matrix, MAE, MSE, RMSE, R2 and a comparison table | `Task4_Evaluation/` |
| 5. Mini Project | Breast cancer classification with 3 models and 7 plots. **KNN was best** (95.61% accuracy, 97.22% recall) | `Task5_Mini_Project/` |

Regression result: MAE 3.058, MSE 18.966, RMSE 4.355, R2 0.839.

---

# Week 5 - Deep Learning & Neural Networks

| Task | What I did | File |
|---|---|---|
| 1. Fundamentals | 2-page PDF: deep learning, AI vs ML vs DL, neuron, layers, weights and bias, activation functions, epoch, loss, optimizer, training flow, with network diagrams | `Task1_Fundamentals_Report/` |
| 2. Basic Neural Network | Keras ANN on Iris: 4 inputs, hidden layers of 16 and 8 neurons, 3 outputs. Includes model summary and architecture diagram | `Task2_Basic_Neural_Network/` |
| 3. Train & Visualize | Trained for 100 epochs, accuracy and loss graphs for training vs validation, with a written explanation | `Task3_Train_and_Visualize/` |
| 4. Evaluation & Prediction | Test accuracy **96.67%** (29 of 30), actual vs predicted table, confusion matrix, explanation of the 1 wrong prediction | `Task4_Evaluation_and_Prediction/` |
| 5. Mini Project | Handwritten digit recognition (0-9) with a neural network. **97.50% test accuracy** (351 of 360), graphs, confusion matrix, 250-400 word report | `Task5_Mini_Project/` |

**Mini project architecture:** Input (64) -> Dense 128 (ReLU) -> Dropout 0.2 -> Dense 64 (ReLU) -> Dense 10 (Softmax), Adam optimizer, 40 epochs.

## How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
jupyter notebook
```
Open a notebook and run all cells. Each notebook reads the CSV in its own folder.
For Week 5, run Task 3 before Task 4, because Task 4 loads the model saved by Task 3.

## What I Learned
- The full ML workflow: clean data, split, train, predict, evaluate
- Why accuracy alone is not enough, and how precision, recall and the confusion matrix help
- How a neural network learns: forward pass, loss, backpropagation and optimizer
- How to read training and validation curves to check for overfitting
- Why inputs should be scaled before training a neural network

## Dataset Sources
- Iris and Breast Cancer: UCI Machine Learning Repository via scikit-learn
- Handwritten Digits (8x8 images): UCI Machine Learning Repository via scikit-learn
- Student marks (Week 4): practice data generated with NumPy
