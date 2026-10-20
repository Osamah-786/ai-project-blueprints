# Project Guide: Machine Learning

## Decide before coding
- Define the target, intended use, baseline, evaluation metrics, and acceptance threshold.
- Identify data sources, permissions, data quality, missing values, leakage risks, and class imbalance.
- Choose a reproducible split strategy and record random seeds where relevant.
- Establish a simple baseline before trying complex models.
- Decide how experiments, features, models, and datasets will be versioned.
- Define inference latency, resource needs, monitoring, and retraining triggers.

## Workflow
1. Inspect and validate the data.
2. Establish a baseline.
3. Build repeatable preprocessing and training.
4. Compare models using suitable metrics.
5. Evaluate on data not used to fit or tune the model.
6. Package inference and document limitations.

## Reliability
- Prevent train/test leakage.
- Keep preprocessing consistent between training and inference.
- Track data sources and relevant licenses.
- Record assumptions and limitations.
- Test input validation, model loading, and representative predictions.
- Report metrics with their evaluation setup.
