# ShapTST-Finance: A Unified Transformer for Real-Time Prediction and Explanation

1. Introduction
This project addresses a critical challenge in quantitative finance: the trade-off between the predictive power of complex AI models and the need for real-time transparency. While state-of-the-art models like Transformers excel at forecasting, their "black box" nature makes them difficult to trust, manage, and audit, especially in high-speed trading environments.   

The current industry standard for model explanation relies on post-hoc techniques like SHAP (SHapley Additive exPlanations). However, these methods are computationally intensive and introduce significant latency, as the explanation is calculated in a separate process after a prediction is made. This makes them unsuitable for real-time applications.

2. The Solution: A Unified Framework
This project implements ShapTST-Finance, a novel framework that unifies prediction and explanation into a single, efficient forward pass. By adapting the cutting-edge ShapTST (Shapley Time-Series Transformer) architecture, this model generates both a financial forecast and its corresponding feature-level explanation simultaneously.

The core innovation is a specialized two-stage training protocol that embeds the explanation mechanism directly into the model's architecture, eliminating the need for slow, post-hoc computations.
