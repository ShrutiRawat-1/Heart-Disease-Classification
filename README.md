# Heart Disease Classification

Predicts whether a patient has heart disease from 13 clinical measurements using logistic regression on the 303-patient Cleveland heart disease dataset.


## Results

| Metric | Value |
|---|---|
| Baseline (always guess the larger class) | 54.5% |
| Training accuracy | 84.7% |
| Test accuracy (61 patients) | 78.7% |
| 5-fold cross-validated accuracy | 81.9% (± 5.4%) |
| Recall, heart disease class (test set) | 79% |

The test set is small so the cross-validated figure is the more reliable one. The notebook includes a confusion matrix and a full classification report.

## Note

- **Feature scaling was needed.** Unscaled logistic regression failed to converge, so the model uses a `StandardScaler`.


## Files

```
heart_disease_classification.ipynb   the full analysis
data/heart_disease_data.csv          dataset (303 rows, 13 features + target)
requirements.txt
```

