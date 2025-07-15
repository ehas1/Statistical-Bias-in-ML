# Statistical Bias In ML

This repository contains code for analyzing the COMPAS recidivism dataset using various machine learning models. The analysis includes decision trees, XGBoost, and neural networks, along with model interpretability using LIME and SHAP.

## Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/compas-analysis.git
cd compas-analysis
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Initialize DVC:
```bash
dvc init
dvc add data/  # If you have data files to track
```

## Project Structure

- `OAIP_Skeleton.ipynb`: Main notebook containing model training and evaluation
- `LIME_and_SHAP.ipynb`: Model interpretability analysis using LIME and SHAP
- `models/`: Directory containing saved models (tracked by DVC)
- `requirements.txt`: Project dependencies
- `.dvc/`: DVC configuration and cache

## Usage

1. Run the main analysis notebook:
```bash
jupyter notebook OAIP_Skeleton.ipynb
```

2. Run the interpretability analysis:
```bash
jupyter notebook LIME_and_SHAP.ipynb
```

The models will be automatically saved to your local `models/` directory and tracked by DVC.

## Model Storage

Models are saved locally in the `models/` directory and tracked using DVC. Each model is saved with its metadata in JSON format. The following models are generated:

- Decision Tree: `models/decision_tree_model.joblib`
- XGBoost: `models/xgboost_model.json`
- Neural Network: `models/neural_network_model.keras`

## Model Interpretability

The `LIME_and_SHAP.ipynb` notebook provides detailed analysis of model predictions using:
- LIME (Local Interpretable Model-agnostic Explanations)
- SHAP (SHapley Additive exPlanations)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
