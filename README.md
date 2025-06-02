# Hand-Gesture-Classification-Project
 Hand Gesture Classification Using MediaPipe Landmarks from the HaGRID Dataset
![image](https://github.com/user-attachments/assets/13fa3858-77c7-4578-9311-1d7bbcae3c17)
This repository contains the full pipeline for training a hand gesture classification model using XGBoost, tracking experiments with MLflow, and selecting the best-performing model.

## 🔬 Workflow

- Preprocessing and feature engineering
- Model training and fine-tuning using grid search
- Experiment tracking using MLflow (`mlruns/` directory included)
- Final model serialization (`model.pkl`, `encoder.pkl`)

## 🧪 Model Selection

After extensive experimentation and hyperparameter tuning, the best model was found with the following parameters:

Best Hyperparameters: {
  "colsample_bytree": 0.8,
  "learning_rate": 0.1,
  "max_depth": 7,
  "n_estimators": 300,
  "subsample": 0.5
}

Final Evaluation Metrics:
-Accuracy: 98.10%
-Precision: 98.08%
-Recall: 98.04%
-F1 Score: 98.05%

After training with the optimal hyperparameters and evaluating on the test set, we achieved:

✅ Test Accuracy: 98.36%
This result indicates excellent performance and strong generalization to unseen data.

