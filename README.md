# 🩺 End-to-End Chest Cancer Classification using MLflow & DVC
This project demonstrates a full pipeline for chest cancer classification using machine learning, version control, and experiment tracking. It integrates MLflow for experiment management and DVC (Data Version Control) for reproducible pipelines.

## 🔁 Workflow Overview
To run or modify the pipeline, follow these steps in order:

```
1️⃣  Configure `config.yaml`

2️⃣  (Optional) Configure secrets in `secrets.yaml`

3️⃣  Set hyperparameters in `params.yaml`

4️⃣  Update the entity definitions

5️⃣  Adjust configuration logic in `src/config/`

6️⃣  Modify component-level logic

7️⃣  Update the pipeline structure

8️⃣  Edit the main entry script (`main.py`)

9️⃣  Finalize the pipeline in `dvc.yaml`
```

## 📈 Experiment Tracking with MLflow
📄 [Documentation](https://mlflow.org/docs/latest/index.html)

🎥 [MLflow tutorial](https://youtube.com/playlist?list=PLkz_y24mlSJZrqiZ4_cLUiP0CBN5wFmTb&si=zEp_C8zLHt1DzWKK)

---

## 🚀 Launch MLflow UI Locally
```bash
mlflow ui
```

---
## ☁️ MLflow on DAGsHub
You can track your MLflow experiments directly on [dagshub](https://dagshub.com/):
```bash
MLFLOW_TRACKING_URI=https://dagshub.com/<MLFLOW_USER_NAME>/chest-Disease-Classification-MLflow-DVC.mlflow \
MLFLOW_TRACKING_USERNAME=<USER_NAME> \
MLFLOW_TRACKING_PASSWORD=<YOUR_TRACKING_PASSWORD> \
python script.py
```

To export these variables as environment variables:
```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/<MLFLOW_USER_NAME>/chest-Disease-Classification-MLflow-DVC.mlflow
export MLFLOW_TRACKING_USERNAME=<USER_NAME> 
export MLFLOW_TRACKING_PASSWORD=<YOUR_TRACKING_PASSWORD>
```

🔒 Security Note: Avoid hardcoding sensitive credentials like passwords or API tokens. Instead, use .env files or secret managers where applicable.

---
## 🧪 Reproducibility Tools
- **DVC:** Ensures data and model versioning

- **MLflow:** Tracks parameters, metrics, models, and artifacts

- **ConfigBox (via box):** Structured config management

- **YAML/JSON:** Configuration-driven development
