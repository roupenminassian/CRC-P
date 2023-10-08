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

Based on the provided data, here are some key conclusions:

### Subject-Independent Modelling:

1. **Global Features vs. Local Features:** In subject-independent modeling, both global and local features perform equally well in terms of precision, recall, F1-score, and accuracy for both binary and multilabel classification tasks. This suggests that the choice between global and local features may not significantly impact model performance in this scenario.

2. **Binary vs. Multilabel Classification:** Binary classification consistently achieves higher precision, recall, F1-score, and accuracy compared to multilabel classification in subject-independent modeling. This indicates that distinguishing between "movement" and "rest" is more accurate and reliable than classifying specific activities in this context.

### Subject-Dependent Modelling:

1. **Global Features vs. Local Features:** In subject-dependent modeling, local features outperform global features for binary classification in terms of precision, recall, F1-score, and accuracy. This suggests that capturing local variations in the signals is crucial when the model's performance depends on individual subjects.

2. **Binary vs. Multilabel Classification:** Binary classification generally performs better than multilabel classification in subject-dependent modeling, achieving higher precision, recall, F1-score, and accuracy. However, the difference in performance between binary and multilabel tasks is less pronounced compared to subject-independent modeling.

3. **Local Features in Binary Classification:** Among all configurations, subject-dependent modeling with local features for binary classification demonstrates the highest precision, recall, F1-score, and accuracy. This combination appears to be particularly effective in distinguishing "movement" from "rest" within individual subjects.

In summary, the choice of modeling approach (subject-independent or subject-dependent) and the type of features (global or local) should be tailored to the specific classification task and context. Binary classification consistently performs better than multilabel classification, but the effectiveness of global and local features varies depending on the modeling scenario.
