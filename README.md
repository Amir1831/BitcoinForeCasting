# BitcoinForecasting 💲💰


The series of expriments that you see in this notebook:


| Model Number | Model Type | Horizon size | Window size | Extra data | MAE | MSE |
| ----- | ----- | ----- | ----- | ----- |------ | -------|
| 0 | Naïve model (baseline) | NA | NA | NA | 567.9802 | 1147547.0 |
| 1 | Dense model | 1 | 7 | NA | 570.3884 | 1162499.5 |
| 2 | Same as 1 | 1 | 30 | NA | 606.88934 | 1256685.8 |
| 3 | Same as 1 | 7 | 30 | NA | 1240.4626 | 5447789.5 |
| 4 | LSTM | 1 | 7 | NA | 575.19183 | 1174953.1 |
| 5 | Same as 1 (but with `multivariate data`) | 1 | 7 | Block reward size | 569.68774 | 1165185.5 |
| 6 | Same as 5 (but with `multiinput model`) | 1 | 7 | Block reward size | 588.8948 | 1204816.4 |
| 7 | [N-BEATs Algorithm](https://arxiv.org/pdf/1905.10437.pdf) | 1 | 7 | NA | 582.5573 | 1165783.8 |
| 8 | Ensemble (multiple models optimized on different loss functions) | 1 | 7 | NA | 579.04333 | 1181153.6 |
| 9 | Future prediction model (model to predict future values) | 1 | 7 | NA| NA | NA |

* **horizon** = number of timesteps to predict into future
* **window** = number of timesteps from past used to predict **horizon**
