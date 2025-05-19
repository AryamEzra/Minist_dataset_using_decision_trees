# Decision Tree Classifier on the Digits Dataset

This project implements and tunes a Decision Tree classifier to recognize handwritten digits using the scikit-learn's Digits dataset. The notebook explores the impact of various hyperparameters on the model's performance and demonstrates how to improve accuracy by tuning these parameters.

## Dataset

The project uses the Digits dataset, a collection of 1797 8x8 grayscale images of handwritten digits (0-9). Each image is represented by a 64-feature vector, with values indicating pixel intensity.

## Notebook Analysis

The notebook covers the following steps:

1.  **Data Loading and Exploration:** The Digits dataset is loaded and a few sample images are displayed to visualize the data.
2.  **Data Splitting:** The dataset is split into training, validation, and testing sets to facilitate model evaluation and prevent overfitting.
3.  **Baseline Model:** A Decision Tree classifier is trained with default parameters and its performance is evaluated using accuracy and a confusion matrix. The analysis identifies overfitting in the baseline model.
4.  **Hyperparameter Tuning (max_depth):** The impact of the `max_depth` hyperparameter on model performance is explored by training and evaluating the model with different `max_depth` values. The results are visualized to identify an optimal range for this parameter.
5.  **Hyperparameter Tuning (Grid Search):** A grid search is performed to find the optimal combination of multiple hyperparameters, including `criterion`, `min_samples_split`, and `min_samples_leaf`, in addition to `max_depth`.
6.  **Evaluation of Tuned Model:** The Decision Tree model with the best hyperparameters found through grid search is evaluated on the test set, and its performance is compared to the baseline model and the model tuned only for `max_depth`.
7.  **Conclusion:** The notebook concludes that hyperparameter tuning significantly improves the Decision Tree model's performance on the Digits dataset.
8.  **Limitations and Future Work:** The limitations of the Decision Tree model are discussed, and suggestions for future work, such as exploring other classification algorithms, are provided.

## Dependencies

The code requires the following libraries:

*   numpy
*   pandas
*   matplotlib
*   scikit-learn

You can install these dependencies using pip:
`bash pip install numpy pandas matplotlib scikit-learn`

## How to Run

1.  Clone this repository.
2.  Open the notebook in Google Colab or a Jupyter Notebook environment.
3.  Run the cells sequentially to execute the code and see the results.

## Results

The analysis shows that tuning hyperparameters, especially using a grid search, leads to improved accuracy on the test set compared to the baseline model and tuning only `max_depth`. The notebook presents the performance metrics for each stage of the tuning process.
