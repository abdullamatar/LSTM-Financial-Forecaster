# General LSTM and RNN notes

> _*"based on Brownian Motion, the future variations of stock price are independent of the past"*_ [src](https://towardsdatascience.com/lstm-for-google-stock-price-prediction-e35f5cc84165)

- meaning predicting exact price is somewhat impossible, but capturing the trend can be done.

- Long short term memory networks are a type of RNN capable of learning order dependence in sequence predictions.
  - [rc](https://machinelearningmastery.com/gentle-introduction-long-short-term-memory-networks-experts)

> "RNNs can only connect recent previous information and cannot connect information as the time gap grows. This is where LSTMs come into play; LSTMs are a type of RNN that remember information over long periods of time, making them better suited for predicting stock prices. For a technical explanation of LSTMs click [here"](https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21).

## `Final solution`

- Due to the lack of data for Borouge's stock price history I will train a LSTM model on ADNOC's price history and use a transfer learning approach. From what I've seen and tested this should work; however, time series data is very uncertain...
- The 'baseline' dataset (aka. _source domain_) would be ADNOCs price history. I would then be transferring the learned weights to serve as an initialization for the model to be trained on Borouge's data (the _target domain_).

#### `Some more on transfer learning`

1. [TransferLearning_src](https://analyticsindiamag.com/building-a-transfer-learning-model-for-time-series-forecasting/)
2. [TransferLearning_src2](https://towardsdatascience.com/transfer-learning-for-time-series-prediction-4697f061f000)

---
