

# Disease_PREDICTOR

A GUI-based application for predicting diseases using symptoms, powered by machine learning algorithms (Decision Tree, Random Forest, Naive Bayes) in Python. Users enter symptoms via a graphical interface, and the app predicts the most likely disease.

***

## Features

- Select up to **five symptoms** from a large predefined list using dropdown menus.
- Predict disease using three machine learning models:
  - **Decision Tree**
  - **Random Forest**
  - **Naive Bayes**
- See predictions and model accuracy directly in the interface.
- Reset selections and clear results easily.
- Designed for educational and demonstration purposes.

***

## Directory Structure

```
deep_proj/
│
└── deep/
    ├── app.py
    ├── requirements.txt
    ├── data/
    │   ├── Training.csv
    │   └── Testing.csv
```

***

## Setup Instructions

### 1. Install Python

- Make sure you have **Python 3.x** installed.

### 2. Install Dependencies

- Open your terminal and change to the project directory:
  ```bash
  cd C:\Users\deepv\Downloads\deep_proj\deep
  ```

- **Edit requirements.txt**: Remove the lines for `tk` and `tkinter` (Tkinter is built-in with most Python installations).
  Your requirements.txt should look like:
  ```
  pandas
  numpy
  scikit-learn
  matplotlib
  ```

- Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```

### 3. Prepare Data Files

- Ensure `Training.csv` and `Testing.csv` are present in the `data` folder.
- These files must use the same symptom columns as defined in the code and end with a `prognosis` column.

***

## Running the Application

- In the terminal (from the `deep` directory), launch the app:
  ```bash
  python app.py
  ```
- A GUI window will open. Enter patient name, select up to five symptoms, and click the model buttons to predict disease.

***

## Usage Notes

- **Tkinter** is required but should come bundled with Python. If you see "No module named tkinter" errors, install Python from the official source.
- Model results and accuracy are printed in the terminal for each prediction.
- Only the listed symptoms can be used for prediction.

***

## Example

1. Open the app using the steps above.
2. Enter a name and select symptoms from the dropdowns.
3. Press "DecisionTree," "Randomforest," or "NaiveBayes" to see disease predictions and accuracy.
4. Use "Reset" to clear all selections.

***

## File Descriptions

| File            | Purpose                                            |
|-----------------|---------------------------------------------------|
| `app.py`        | Main application containing GUI and ML algorithms  |
| `requirements.txt` | List of installable Python packages (no tkinter) |
| `data/Training.csv` | Training data (symptoms and disease labels)     |
| `data/Testing.csv`  | Testing data used to evaluate model accuracy    |

