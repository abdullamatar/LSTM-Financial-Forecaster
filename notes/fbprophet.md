# Introductory notes: Facebook Prophet Library

- Facebook [prophet](https://facebook.github.io/prophet/) website
- Face book's _Prophet_ which is an open source library aiding time series pattern recognition for non-stationary data ➡️ i.e. moving averages and variances. The source for this information is linked [_here._](https://towardsdatascience.com/predicting-apple-inc-stock-prices-using-facebooks-prophet-54ed6e91dbda)

- _Prophets_ equation is as follows:

  `y(t) = g(t) + s(t) + h(t) + e(t)`

  - g(t) represents the trend using a piecewise linear model
  - s(t) represents periodic changes
  - h(t) represents the effect of the 'off season' on the business
  - e(t) covers the changes or errors not considered by the model
