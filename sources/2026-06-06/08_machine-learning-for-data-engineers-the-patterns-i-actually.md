---
type: story
story_id: devto_3829790
episode_date: 2026-06-06
rank: 8
source: devto
url: "https://dev.to/de_clerke/machine-learning-for-data-engineers-the-patterns-i-actually-used-across-7-projects-eoi"
title: Machine Learning for Data Engineers The Patterns I Actually Used Across 7 Projects
quality_score: 0.89
content_hash: "sha256:7483a2c745bb2796dd1f6b51181762d518cb2dd980bb4b7a1b8c477d47105af3"
concepts: [xgboost, facebook-prophet, shap, finbert, huggingface-transformers, sentence-transformers, pgvector, mlflow, lightgbm, scikit-learn, optuna, apache-airflow, random-forest, joblib]
companies: [meta-facebook, huggingface, world-bank]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-06-06 10:19:43.883000"
tags: [story, source/devto]
---

## Summary
A data engineer describes the ML stack and patterns used across seven production projects, including used car price prediction, health outcome modelling, time-series forecasting, financial sentiment analysis, semantic job search, inflation forecasting, and crop yield projection. The core tools were XGBoost for tabular regression, Facebook Prophet for time-series forecasting, SHAP for explainability, and HuggingFace Transformers (FinBERT and sentence-transformers) for NLP tasks. Supporting tools included scikit-learn, MLflow, Optuna, joblib, and pgvector for queryable embeddings. The author emphasizes that these were data engineering projects where a model replaced a dashboard as the final step, and the entire stack runs locally or on free tiers without paid cloud ML platforms. Practical gotchas and benchmark comparisons between XGBoost, LightGBM, and Random Forest are shared from real datasets.

## Key claims
- XGBoost outperformed LightGBM and Random Forest on a 291-row used car dataset with MAE of 3,706 and R² of 0.722.
- Facebook Prophet was used to run 109 separate time-series forecasts for 15 African development indicators.
- FinBERT was used for financial news sentiment analysis without requiring OpenAI API keys.
- pgvector was used to make sentence-transformer embeddings queryable for semantic job search.
- MLflow was used for experiment tracking across all projects, integrated into an Airflow DAG for weekly retraining.
- The entire ML stack is reproducible locally or on free tiers with no paid cloud ML platforms.
- SHAP was used to provide model explainability across projects.

## Source
- **Origin:** devto
- **URL:** <https://dev.to/de_clerke/machine-learning-for-data-engineers-the-patterns-i-actually-used-across-7-projects-eoi>

## Related
[[concepts/xgboost|xgboost]] · [[concepts/facebook-prophet|facebook-prophet]] · [[concepts/shap|shap]] · [[concepts/finbert|finbert]] · [[concepts/huggingface-transformers|huggingface-transformers]] · [[concepts/sentence-transformers|sentence-transformers]] · [[concepts/pgvector|pgvector]] · [[concepts/mlflow|mlflow]] · [[concepts/lightgbm|lightgbm]] · [[concepts/scikit-learn|scikit-learn]] · [[concepts/optuna|optuna]] · [[concepts/apache-airflow|apache-airflow]] · [[concepts/random-forest|random-forest]] · [[concepts/vector-embeddings|vector-embeddings]] · [[concepts/data-engineering|data-engineering]] · [[concepts/machine-learning|machine-learning]] · [[concepts/semantic-search|semantic-search]] · [[concepts/data-science|data-science]] · [[concepts/embeddings|embeddings]] · [[concepts/pipeline|pipeline]] · [[concepts/airflow|airflow]] · [[concepts/python|python]] · [[concepts/cloud|cloud]] · [[concepts/api|api]] · [[concepts/dag|dag]] · [[companies/meta-facebook|Meta (Facebook)]] · [[companies/huggingface|HuggingFace]] · [[companies/world-bank|World Bank]] · [[episodes/2026-06-06|2026-06-06]]
