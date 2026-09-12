# Credit Card Fraud Detection

This project contains a notebook-based fraud detection workflow for credit card transaction data. It includes data exploration, preprocessing, feature engineering, and a deep learning LSTM model for fraud classification.

## Quick project setup

### 1) Create a virtual environment

```bash
cd "path/to/cc-fraud-detection"
python3 -m venv .venv
source .venv/bin/activate
```

### 2) Install dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

If you want to run notebooks in Jupyter locally, install Jupyter as well:

```bash
pip install notebook jupyterlab
```

### 3) Start the notebook environment

```bash
jupyter notebook
```

Then open either:
- `detector.ipynb`
- `fraud-detector.ipynb`

### 4) Check the dataset

The project expects credit card data in the `data/` folder, for example:

```bash
data/creditcard.csv
```

If the dataset is missing, download it or place the CSV file in the `data/` directory before running the notebook cells.

### 5) Run the notebook

Execute the cells from top to bottom in order. The notebook performs:
- dataset loading
- validation checks
- exploratory data analysis
- feature engineering
- train/validation/test splitting
- scaling and sequence creation
- LSTM model training and evaluation

## Project files

- `detector.ipynb` — main fraud detection workflow
- `fraud-detector.ipynb` — alternate notebook version
- `requirements.txt` — Python dependencies
- `data/` — transaction datasets

## Notes

- Recommended Python version: 3.10+
- For VS Code users, select the virtual environment interpreter (`.venv`) before running notebook cells.
