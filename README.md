#  AI Business Idea Feasibility Validator (ML + XAI Project)

This project implements a web-based application to assess the feasibility and market potential of new startup concepts using a combination of Machine Learning (ML) and Explainable AI (XAI) features.

## 🌟 Key Features

* **ML Prediction:** Uses a **TF-IDF Vectorizer** coupled with a **Logistic Regression Classifier** to predict an idea's potential into three classes: **High, Medium, or Low**.
* **Explainable AI (XAI):** The model provides **Feature Breakdown Scores** (Keyword Richness, Novelty, Simplicity) based on NLP analysis to explain *why* the idea received its score.
* **Visual Analysis:** Includes a dedicated dashboard to visualize **Class Probabilities** (ML confidence) and Feature Scores.
* **Data Size:** The final model is trained on a **10,000-row dataset** of labeled startup ideas (using the data structure defined in `appropriate_startup_data.csv`).
* **Risk & Strategy:** Provides rule-based suggestions for business models, key risks, and goal-based next steps.

## 🛠️ Technology Stack

| Component | Library / Framework | Purpose |
| :--- | :--- | :--- |
| **Frontend/Hosting** | Streamlit | Rapid creation and hosting of the interactive web UI. |
| **Machine Learning** | Scikit-learn | Core library for model training (Logistic Regression). |
| **NLP Features** | Scikit-learn / Python `re` | Used for TF-IDF vectorization and custom rule-based feature engineering. |
| **Data Processing** | Pandas / NumPy | Handling and preparing the 10,000-row training dataset. |

## 🚀 How to Run the Application

This application is deployed and run directly using Streamlit Cloud.

1.  **Prerequisites:** Ensure all required files (`streamlit_app.py`, `requirements.txt`, `appropriate_startup_data.csv`) are in the root of this public GitHub repository.
2.  **Deployment:** Navigate to [https://share.streamlit.io](https://share.streamlit.io).
3.  Select this repository and the `main` branch.
4.  Set the main file path to **`streamlit_app.py`**.
5.  Click **Deploy**.

The app will install dependencies (from `requirements.txt`) and train the model immediately, resulting in a live, public web application.
