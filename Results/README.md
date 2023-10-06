## Model Performance Metrics

Below is a summary of the performance metrics for different model configurations in our experiment. We evaluated these models in both subject-independent and subject-dependent modeling scenarios, utilizing global and local features for binary and multilabel classification tasks.

### Subject-Independent Modelling

| Feature | Label      | Precision | Recall | F1   | Accuracy |
| ------- | ---------- | --------- | ------ | ---- | -------- |
| Global  | Binary     | 0.92      | 0.91   | 0.91 | 0.91     |
| Global  | Multilabel | 0.49      | 0.50   | 0.47 | 0.50     |
| Local   | Binary     | 0.92      | 0.91   | 0.91 | 0.91     |
| Local   | Multilabel | 0.49      | 0.50   | 0.47 | 0.50     |

### Subject-Dependent Modelling

| Feature | Label      | Precision | Recall | F1   | Accuracy |
| ------- | ---------- | --------- | ------ | ---- | -------- |
| Global  | Binary     | 0.74      | 0.83   | 0.77 | 0.83     |
| Global  | Multilabel | 0.74      | 0.82   | 0.77 | 0.81     |
| Local   | Binary     | 0.82      | 0.89   | 0.85 | 0.89     |
| Local   | Multilabel | 0.62      | 0.71   | 0.65 | 0.71     |

These performance metrics provide valuable insights into the effectiveness of different model configurations and feature sets for classifying human activities using wearable sensor data.
