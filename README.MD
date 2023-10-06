# Human Activity Classification Using Wearable Sensor Data

## Experimental Design

Our experimental methodology was meticulously crafted to investigate the classification of human activities based on wearable sensor data. We placed our focus on exploring various configurations to determine the optimal approach for classifying activities such as sitting, walking, and running. Our investigations revolved around the following key aspects:

1. **Subject-Dependent vs. Subject-Independent Modelling:** We delved into two distinct modeling approaches. In subject-dependent modeling, we trained and tested on data from individual subjects, whereas in subject-independent modeling, we trained on data from multiple subjects and tested on others.

2. **Global vs. Local Features:** Our feature extraction process encompassed both global and local features derived from raw ECG (Electrocardiogram) and PPG (Photoplethysmogram) signals. Global features provided a comprehensive summary of the entire signal, while local features honed in on characteristics within localized windows.

3. **Binary vs. Multi-label Classification:** In binary classification, we categorized activities into 'movement' or 'rest,' while in multi-label classification, we sought to identify specific activities such as sitting, walking, and running.

## Data Collection

We collected our dataset using wearable sensors capable of capturing ECG and PPG signals, with a consistent sampling frequency set at 500 Hz. The dataset was meticulously organized into individual files, each corresponding to a specific subject's performance of a distinct activity.

## Data Modification

To gain deeper insights into the impact of data granularity on our analyses, we undertook two primary modifications to our dataset: frequency sampling and data period adjustments.

### Frequency Sampling

We systematically sampled the primary data at various frequencies, including 300 Hz, 100 Hz, 50 Hz, and 25 Hz. Each frequency level represented a different level of granularity, allowing us to assess the sensitivity of our findings to the frequency of data collection.

### Data Period Adjustments

In addition to frequency sampling, we recognized the significance of evaluating the influence of data duration on our results. Consequently, we systematically adjusted the data period to 50%, 25%, and 10% of the original data duration, observing any consequential variations. Each adjustment offered valuable insights into the robustness of our findings, revealing whether shorter data spans significantly affected our conclusions.

## Feature Extraction

For both ECG and PPG signals, we meticulously extracted a range of statistical and spectral features, encompassing measures such as mean, median, variance, standard deviation, skewness, kurtosis, number of peaks, number of valleys, spectral entropy, dominant frequency, and heart rate variability indices (e.g., mean NNI, SDNN). These features were extracted both globally, summarizing the entire signal, and locally, within overlapping windows.

## Modelling

Our modeling approach hinged on the utilization of a Random Forest Classifier comprising 1000 trees. We employed Stratified K-Fold cross-validation for subject-independent modeling and a train-test split for subject-dependent modeling.

### Subject-Dependent Modelling

For subject-dependent modeling, we partitioned each subject's data into a training set and a test set, preserving the original proportions of each activity type. Subsequently, we trained a Random Forest model for each subject and assessed its performance using metrics such as accuracy, precision, recall, and F1-score.

### Subject-Independent Modelling

Subject-independent modeling involved the use of Stratified K-Fold cross-validation to maintain the original proportions of each activity type across folds. The Random Forest model was trained on 4 folds and tested on the remaining one, repeating this process for each fold while averaging performance metrics.

## Evaluation Metrics

We assessed our models using a range of evaluation metrics, including accuracy, precision, recall, and F1-score, to provide a detailed performance analysis accounting for both false positives and false negatives.

## Feature Importance

To gain insights into the significance of each feature on the classification process, we leveraged SHAP (SHapley Additive exPlanations) to calculate Shapley values for each feature.

## Aggregated Metrics

In subject-dependent modeling, we calculated the weighted average of precision, recall, and F1-score across all subjects to obtain an overall performance metric.

## Results

The outcomes of each experiment were meticulously analyzed to comprehend the influence of different configurations on the performance of our activity classification model. Additionally, we evaluated aggregated metrics to gain a holistic perspective of the model's performance across diverse conditions.

## Conclusion

This comprehensive methodology serves as a robust framework for evaluating human activity classification using wearable sensor data. It systematically explores multiple configurations, employs various evaluation metrics, and aims to identify the most effective approach for real-world applications. Our project contributes valuable insights to the field of human activity classification and sensor-based applications.
