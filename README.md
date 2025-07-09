# Time-Series-Forecasting

Kristan Böttjer (11422684)
Rafael Barros (11411431)

The repository is structured as follows:
For each model there is a notebook which consists of the model function and a basic evaluation with just a simple train test split.
In the end of each model notebook a cross validation is performed. Generally we tried to find one function which captures the design decisions one would make
manually. In the end we compare all models in the results notebook where you can see all models side by side.


General remarks:
For the Australian Electricity dataset. We used the data of the state of Victoria only. Also we aggregated it to daily data 
as hourly otherwise it was too much data. In Hindsight we could have also just reduced the number of data points to keep the diverstiy of frequencies. 
. The Car Parts dataset was also aggregated. Here we just used the sum of all shops so grouped by date.

Data Extraction:
. we basically defined 2 notebooks for that, for instance datagetter.ipynb & basic_functions.ipynb (also including tsf extraction function to a dataframe format for our analysis)



Moirai:
1. What is Moirai?
Moirai is an open-source, large-scale foundation model for time series forecasting developed by Salesforce AI.

     - It is designed to be domain-agnostic (works across industries and types of time series data).

     - Like language models for text (e.g., GPT), Moirai is a pre-trained model that can be fine-tuned or used directly for forecasting various time series tasks.

2. Why Moirai:
     - Traditional time series models (ARIMA, Prophet, etc.) or small deep learning models are often domain-specific and trained from scratch for each dataset.

     - Moirai aims to generalize forecasting by training on a massive collection of time series data, enabling zero-shot or few-shot forecasting (i.e., forecasting without or with very little additional training).

3. Key Features:
     - Scalable Transformer Architecture: Uses advanced transformer neural networks, which are state-of-the-art for sequence modeling.

     - Large-scale Pretraining: Trained on hundreds of millions of time series from various domains (retail, energy, finance, etc.).

     - Zero-shot & Few-shot Learning: Can make accurate predictions for new time series it has never seen before, or adapt quickly with small amounts of new data.

     - Domain Agnostic: Unlike models tailored for specific types of time series, Moirai works across many domains.

4. Technical Details:
     - Utilizes a causal transformer architecture (sequence-to-sequence model).

     - Handles seasonality, trend, and noise in time series through deep contextual understanding.

     - Supports multivariate time series (multiple variables/columns).

     - Pretrained on a vast, diverse dataset, enabling generalization and transfer learning.

5. Evaluation and Results:
     - Moirai was evaluated on dozens of public and proprietary datasets, outperforming classical models (ARIMA, Prophet, NBEATS, etc.) and other deep learning models.

     - Shows strong performance in both zero-shot (no retraining) and few-shot (minimal retraining) scenarios.

6. Pros and Cons:
Pros:

     - Generalization: Works well on many types of time series, not just one domain.

     - Zero-shot capability: Useful for forecasting when you have little or no data to retrain.

     - State-of-the-art performance: Competes with or beats specialized models in many benchmarks.

     - Open-source: Freely available for academic and industry use.

Cons:

     - Computationally Intensive: Large transformer models require more resources than simple statistical models.

     - Less Interpretable: Like most deep learning models, Moirai is less interpretable than classical models (harder to explain why it made a specific forecast).

     - May need fine-tuning for best performance on some niche datasets.