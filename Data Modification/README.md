# Data Modification

In the pursuit of understanding the impact of data granularity on our analyses, we employed two primary modifications to our dataset: frequency sampling and data period adjustments.

## Frequency Sampling

The primary data was sampled at distinct frequencies to identify potential variations in analysis results. The chosen frequencies were:

- 300Hz
- 100Hz
- 50Hz
- 25Hz

Each frequency level represents a reduced granularity, allowing us to assess the sensitivity of our findings to the frequency of data collection.

## Data Period Adjustments

Beyond frequency sampling, we recognized the importance of evaluating the impact of data duration on our results. As such, we shortened the data period in a systematic manner to observe any consequential variations. The periods chosen were:

- 50% of the original data duration
- 25% of the original data duration
- 10% of the original data duration

Each adjustment provides a window into the robustness of our findings, determining if shorter data spans significantly alter our conclusions.

## Data Resampling Results

### Subject-Independent Modelling – Global Features – Multiclass

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.49      | 0.5    | 0.47 | 0.5      |
| 300Hz            | 0.52      | 0.55   | 0.51 | 0.55     |
| 100Hz            | 0.49      | 0.53   | 0.49 | 0.53     |
| 50Hz             | 0.52      | 0.56   | 0.52 | 0.56     |
| 25Hz             | 0.53      | 0.56   | 0.53 | 0.56     |

### Subject-Independent Modelling – Global Features – Binary

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.92      | 0.91   | 0.91 | 0.91     |
| 300Hz            | 0.91      | 0.88   | 0.87 | 0.88     |
| 100Hz            | 0.87      | 0.82   | 0.81 | 0.82     |
| 50Hz             | 0.9       | 0.89   | 0.89 | 0.89     |
| 25Hz             | 0.93      | 0.92   | 0.92 | 0.92     |

### Subject-Independent Modelling – Local Features – Multiclass

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.49      | 0.5    | 0.47 | 0.5      |
| 300Hz            | 0.55      | 0.59   | 0.55 | 0.59     |
| 100Hz            | 0.51      | 0.52   | 0.49 | 0.52     |
| 50Hz             | 0.49      | 0.53   | 0.5  | 0.53     |
| 25Hz             | 0.55      | 0.59   | 0.54 | 0.59     |

### Subject-Independent Modelling – Local Features – Binary

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.92      | 0.91   | 0.91 | 0.91     |
| 300Hz            | 0.91      | 0.9    | 0.89 | 0.9      |
| 100Hz            | 0.9       | 0.88   | 0.87 | 0.88     |
| 50Hz             | 0.94      | 0.93   | 0.92 | 0.93     |
| 25Hz             | 0.97      | 0.97   | 0.97 | 0.97     |

### Subject-Dependent Modelling – Global Features – Multiclass

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.74      | 0.82   | 0.77 | 0.82     |
| 300Hz            | 0.52      | 0.65   | 0.56 | 0.65     |
| 100Hz            | 0.37      | 0.53   | 0.41 | 0.53     |
| 50Hz             | 0.22      | 0.38   | 0.26 | 0.38     |
| 25Hz             | 0.17      | 0.33   | 0.21 | 0.33     |

### Subject-Dependent Modelling – Global Features – Binary

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.74      | 0.83   | 0.77 | 0.83     |
| 300Hz            | 0.83      | 0.89   | 0.85 | 0.89     |
| 100Hz            | 0.5       | 0.7    | 0.58 | 0.7      |
| 50Hz             | 0.42      | 0.64   | 0.51 | 0.64     |
| 25Hz             | 0.44      | 0.67   | 0.53 | 0.67     |

### Subject-Dependent Modelling – Local Features – Multiclass

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.62      | 0.71   | 0.65 | 0.71     |
| 300Hz            | 0.75      | 0.82   | 0.77 | 0.82     |
| 100Hz            | 0.44      | 0.56   | 0.47 | 0.56     |
| 50Hz             | 0.32      | 0.43   | 0.35 | 0.43     |
| 25Hz             | 0.22      | 0.35   | 0.26 | 0.35     |

### Subject-Dependent Modelling – Local Features – Binary

| Frequency        | Precision | Recall | F1   | Accuracy |
| ---------------- | --------- | ------ | ---- | -------- |
| 500Hz (Baseline) | 0.82      | 0.89   | 0.85 | 0.89     |
| 300Hz            | 0.8       | 0.88   | 0.83 | 0.88     |
| 100Hz            | 0.54      | 0.71   | 0.6  | 0.71     |
| 50Hz             | 0.44      | 0.65   | 0.52 | 0.65     |
| 25Hz             | 0.54      | 0.72   | 0.61 | 0.72     |

## Data Period Results

Absolutely! I'll create the table contents for each of the data period datasets you've provided:

### Subject-Independent Modelling – Global Features – Multiclass

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.49      | 0.5    | 0.47 | 0.5      |
| 50%             | 0.57      | 0.56   | 0.54 | 0.56     |
| 25%             | 0.59      | 0.58   | 0.57 | 0.58     |
| 10%             | 0.59      | 0.58   | 0.56 | 0.58     |

### Subject-Independent Modelling – Global Features – Binary

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.92      | 0.91   | 0.91 | 0.91     |
| 50%             | 0.9       | 0.88   | 0.87 | 0.88     |
| 25%             | 0.92      | 0.91   | 0.91 | 0.91     |
| 10%             | 0.87      | 0.85   | 0.84 | 0.85     |

### Subject-Independent Modelling – Local Features – Multiclass

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.49      | 0.5    | 0.47 | 0.5      |
| 50%             | 0.55      | 0.56   | 0.54 | 0.56     |
| 25%             | 0.58      | 0.58   | 0.56 | 0.58     |
| 10%             | 0.57      | 0.54   | 0.52 | 0.54     |

### Subject-Independent Modelling – Local Features – Binary

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.92      | 0.91   | 0.91 | 0.91     |
| 50%             | 0.9       | 0.88   | 0.87 | 0.88     |
| 25%             | 0.91      | 0.89   | 0.89 | 0.89     |
| 10%             | 0.9       | 0.88   | 0.87 | 0.88     |

### Subject-Dependent Modelling – Global Features – Multiclass

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.74      | 0.82   | 0.77 | 0.82     |
| 50%             | 0.49      | 0.62   | 0.53 | 0.62     |
| 25%             | 0.64      | 0.74   | 0.67 | 0.74     |
| 10%             | 0.37      | 0.53   | 0.42 | 0.53     |

### Subject-Dependent Modelling – Global Features – Binary

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.74      | 0.83   | 0.77 | 0.83     |
| 50%             | 0.81      | 0.88   | 0.84 | 0.88     |
| 25%             | 0.71      | 0.82   | 0.75 | 0.82     |
| 10%             | 0.61      | 0.76   | 0.67 | 0.76     |

### Subject-Dependent Modelling – Local Features – Multiclass

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.62      | 0.71   | 0.65 | 0.71     |
| 50%             | 0.59      | 0.7    | 0.62 | 0.7      |
| 25%             | 0.61      | 0.71   | 0.64 | 0.71     |
| 10%             | 0.59      | 0.7    | 0.62 | 0.7      |

### Subject-Dependent Modelling – Local Features – Binary

| Period          | Precision | Recall | F1   | Accuracy |
| --------------- | --------- | ------ | ---- | -------- |
| 100% (Baseline) | 0.82      | 0.89   | 0.85 | 0.89     |
| 50%             | 0.79      | 0.86   | 0.82 | 0.86     |
| 25%             | 0.74      | 0.83   | 0.77 | 0.83     |
| 10%             | 0.82      | 0.88   | 0.84 | 0.88     |
