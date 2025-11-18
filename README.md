# Breast Cancer Status Prediction: A Comparative Study of Machine Learning Models

## Project Overview

This project implements and compares two distinct machine learning classification models—a **Neural Network** and a **Logistic Regression** classifier—to predict the survival status (**Alive or Dead**) of breast cancer patients.

The core objective is to determine which modeling approach offers superior performance, efficiency, and insight when applied to this specific, structured medical dataset.

## 📁 Repository Contents

| File Name | Description |
| :--- | :--- |
| **`Lab6.ipynb`** | The main Jupyter notebook containing the complete machine learning workflow: data preparation, model definition, training, evaluation, and comparative analysis. |
| **`Breast_Cancer.csv`** | The dataset used for this analysis. It includes patient records with crucial clinical features like `Age`, various cancer staging indicators (`T Stage`, `N Stage`), `Tumor Size`, `Estrogen Status`, and `Survival Months`. |

## ⚙️ Methodology and Workflow

The analysis follows a standard data science pipeline as detailed in the `Lab6.ipynb` notebook:

1.  **Data Loading and Preprocessing:**
    * The `Breast_Cancer.csv` dataset is loaded.
    * Categorical features (like `Race`, `Marital Status`, `A Stage`) are encoded into numerical formats suitable for modeling.
    * Numerical features (e.g., `Age`, `Tumor Size`, `Regional Node Examined`) are scaled or standardized to prevent bias in the model training process.
2.  **Model Training:**
    * A **Neural Network** architecture is defined and trained to capture potentially non-linear relationships.
    * A **Logistic Regression** model is trained, serving as an interpretable linear baseline.
3.  **Evaluation:**
    * Both models are rigorously evaluated on a held-out test set to ensure generalizability.
    * Performance is assessed using critical classification metrics, including **Accuracy, Recall, Precision, and F1-Score**.
4.  **Comparative Analysis:**
    * The performance metrics of the two models are compared directly.

## ✨ Key Findings

The project's analysis yielded a significant result: the **Logistic Regression model demonstrated superior overall performance** compared to the more complex Neural Network.

This finding leads to two main conclusions:

1.  **Data Structure:** The relationship between the patient's clinical features and their survival status is likely **linear and well-structured**.
2.  **Model Choice:** For small, clean, and structured datasets in the medical domain, a simpler, highly interpretable model like **Logistic Regression** is often more effective and a better choice for practical application than a complex deep learning architecture.

## 🚀 How to Run the Project

1.  **Clone the repository:**
    ```bash
    git clone [your-repo-url]
    ```
2.  **Set up the environment:**
    ```bash
    # Create and activate a virtual environment
    python -m venv venv
    source venv/bin/activate  # on macOS/Linux
    .\venv\Scripts\activate   # on Windows

    # Install dependencies (assuming you created requirements.txt)
    pip install -r requirements.txt
    ```
3.  **Execute the notebook:**
    Open `Lab6.ipynb` in a Jupyter environment (Jupyter Notebook, JupyterLab, or VS Code) and run the cells sequentially to reproduce the analysis.
