# Final Experimental Results

## Model Performance

| Model | Input | Validation Accuracy | Test Accuracy |
|---|---|---:|---:|
| SVM-33 | 33 engineered features | 59.69% | 54.84% |
| SVM-447 | 414 tactile + 33 engineered | 76.17% | **76.08%** |
| Raw CNN | 414 raw tactile values | 66.59% | 63.63% |

## Key Results

- Best model: SVM-447
- Test accuracy: 76.08%
- Improvement over SVM-33: 21.24 percentage points
- Improvement over Raw CNN: 12.45 percentage points
- SVM-447 validation-test gap: 0.09 percentage points

## Scope

The final project includes:

1. SVM using 33 engineered features
2. SVM using the combined 447-dimensional representation
3. CNN using raw tactile measurements

CNN + engineered features experiments were excluded from the final scope.