# Kaggle

## Topic: JPX Tokyo Stock Exchange Prediction


## folder hierarchy
```
# source data & env
    ㄴinput
        ㄴdata
        
# conda environment setting files
    ㄴconda_env

# eda_notebook
    ㄴdata_search

# source code (ML Pipleline)
    ㄴsrc
        ㄴdo.py
        ㄴconfiguration: 모형 학습 이전의 모든 전처리, 하이퍼 파라미터
        ㄴdata_ingestion: ETL, 데이터 수집, 변환, Merge (prep로 이동 가능) _ 1회성
        ㄴpreparation: Feature 엔지니어링
        ㄴmodel_training: 학습
        ㄴmodel_deployment: 배포, Best parameter

# prediction results
    ㄴoutput

# reference documentations
    ㄴdocs

# template files
    ㄴ.github
```


# Environment
conda create -n jpx-env



# Competition information

## Link
https://www.kaggle.com/competitions/jpx-tokyo-stock-exchange-prediction

## Target: Top 100!

## [Description](https://www.kaggle.com/competitions/jpx-tokyo-stock-exchange-prediction/overview/description)
- Undervalued stock buy, overvalued sell, Quantitative trading
- Japan Exchange Group, Inc. (JPX)
    - Stock exchange = Tokyo Stock Exchange (TSE)
    - Derivatives exchanges = Osaka Exchange (OSE) and Tokyo Commodity Exchange (TOCOM)
    - AlpacaJapan Co.,Ltd.
- 2000 stocks future returns ranks, eval in difference in returns



## [Evaluation](https://www.kaggle.com/competitions/jpx-tokyo-stock-exchange-prediction/overview/evaluation)
- [Sharpe Ratio](https://en.wikipedia.org/wiki/Sharpe_ratio)
- file name = submission.csv
- No over or under rank, No duplicated rank, No row change
- [JPX Competition Metric Definition](https://www.kaggle.com/code/smeitoma/jpx-competition-metric-definition)

```
import jpx_tokyo_market_prediction
env = jpx_tokyo_market_prediction.make_env()   # initialize the environment
iter_test = env.iter_test()    # an iterator which loops over the test files
for (prices, options, financials, trades, secondary_prices, sample_prediction) in iter_test:
    sample_prediction_df['Rank'] = np.arange(len(sample_prediction))  # make your predictions here
    env.predict(sample_prediction_df)   # register your predictions
```



## [Timeline](https://www.kaggle.com/competitions/jpx-tokyo-stock-exchange-prediction/overview/timeline)
- June 28, 2022 - Team merger deadline
- July 5, 2022 - Final



## [Code Requirements](https://www.kaggle.com/competitions/jpx-tokyo-stock-exchange-prediction/overview/code-requirements)
- CPU, GPU Notebook <= 9 hours run-time
- **Freely & Publicly available external data, pre-trained models**
