# Disease Prediction Using Machine Learning and NLP

## Objective

Build a system that predicts the likelihood of a disease (or multiple diseases) based on patient input data — symptoms, medical history, or diagnostic measurements — using machine learning models.

## Scope

This project can be implemented at one of three levels:

- **Single disease** — predicts one specific condition (e.g. Diabetes, Heart Disease, or Breast Cancer) from relevant diagnostic inputs. Simplest to build and a good starting point.
- **Multi-disease** — the user selects a disease, enters the relevant parameters for it, and the app runs the appropriate trained model for that disease.
- **Symptom-based (NLP)** — the user types symptoms in free text; the system extracts and normalizes symptoms using NLP, then predicts the probable disease(s).

*(State here which of the three this repository implements.)*

## Features

- Predicts disease likelihood from structured input (diagnostic measurements) and/or free-text symptoms
- NLP-based symptom extraction and normalization (for the symptom-based mode)
- Trained ML classifier(s) with probability/confidence output
- Simple interface for entering input and viewing predictions

## Tech Stack

- **Language:** Python 3.x
- **ML:** scikit-learn
- **NLP:** NLTK / spaCy *(symptom-based mode only)*
- **Data handling:** Pandas, NumPy
- **Interface:** Flask / Streamlit
- **Model storage:** Pickle / Joblib

## Dataset

Trained on a public dataset relevant to the chosen disease(s), e.g. the Pima Indians Diabetes Dataset, UCI Heart Disease Dataset, or a symptom-disease dataset for the NLP mode. Place dataset files in `data/` before training.

*(Add the exact dataset name and source link used.)*

## Installation

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

## Usage

**Train the model:**
```bash
python src/train_model.py
```

**Run a prediction:**
```bash
python src/predict.py --input "<symptoms or parameter values>"
```

**Run the web app:**
```bash
streamlit run app.py
```

## Project Structure

```
├── data/            # Datasets
├── models/          # Saved trained models
├── src/
│   ├── preprocessing.py
│   ├── train_model.py
│   └── predict.py
├── app.py
├── requirements.txt
└── README.md
```

## Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---|---|---|---|
|  |  |  |  |  |

## Disclaimer

This project is for educational and research purposes only and is not a substitute for professional medical diagnosis or advice.

## License

MIT License.
