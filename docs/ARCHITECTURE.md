# Botanical Plant Species Classification & Thriving Predictor - Architecture & Pipeline Design

```mermaid
graph TD
    DataInput[Raw CSV Dataset: plants_dataset_euhm_itai_07.csv] --> Preproc[Data Cleaning & Column Transformer]
    Preproc -->|Numeric| Scaler[StandardScaler Normalization]
    Preproc -->|Categorical| Encoder[One-Hot Categorical Encoding]
    Scaler --> Split[Train/Test Stratified Split 80/20]
    Encoder --> Split
    Split --> Train[Model Training: XGBoost Classifier]
    Train --> Eval[Evaluation & Benchmarks]
    Eval --> Inference[Production Inference & CLI]
```

## Comparative Models Evaluated
- **XGBoost Classifier**
- **Random Forest**
- **K-Nearest Neighbors**
- **Multi-Layer Perceptron**
