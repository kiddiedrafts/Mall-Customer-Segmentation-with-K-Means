# Customer Segmentation with K-Means

This project implements a customer segmentation analysis using K-Means clustering. The dataset contains information about mall customers, such as their gender, age, annual income, and spending scores. The project preprocesses the data and evaluates the model using the Silhouette Score.

## Dataset

The dataset used in this project is sourced from Kaggle and can be found at the following link: [Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python).

### Dataset Columns

- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer.
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: Customer's spending score, with higher scores indicating more willingness to spend.

  
### Dataset Location

- **Data/**: This folder will contain the dataset files downloaded from Kaggle.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**


## Project Structure

```plaintext
Mall-Customer-Segmentation/
├── Data/
│   └── [dataset files downloaded from Kaggle]
├── Notebooks/
│   └── [Jupyter notebooks for analysis and modeling]
└── README.md
```


## Project Workflow

### Data Preprocessing

1. **Handling Missing Values**: Missing numerical values are replaced with the mean.
2. **Encoding Categorical Features**: Gender is encoded into numerical form using `LabelEncoder`.
3. **Scaling Numerical Features**: Features are standardized using `StandardScaler`.
4. **Dropping Unnecessary Columns**: The `CustomerID` column is dropped as it does not contribute to clustering.

### Model Training

A **K-Means** clustering model is trained on the preprocessed data with the following configuration:
- Number of Clusters: 5

### Model Evaluation

The model's performance is evaluated using the **Silhouette Score**, which quantifies how well the clusters are defined.
- **Silhouette Score**: 0.6589

## Requirements

To run this project, install the following libraries:
- numpy
- pandas
- scikit-learn
- kaggle
