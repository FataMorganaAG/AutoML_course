# AutoML_course
Репозитория для домашнего задания по курсу AutoML

* Соревнование на Kaggle [Feedback Prize - Predicting Effective Arguments](https://www.kaggle.com/competitions/feedback-prize-effectiveness/data)


Структура проекта
------------
    ├── AutoML.ipynb              <- Ноутбук применением AutoML подходов (Линейная модель и LightGBM, Линейная модель и CatBoost, BERT)                  
    │   
    ├── AutoML_data.ipynb         <- Ноутбук с работой с данными
    │
    ├── No_AutoML_1.ipynb         <- Ноутбук с решением без AutoML (LogReg Model + Optuna)
    │
    ├── No_AutoML_2.ipynb         <- Ноутбук с решением без AutoML (Transformers + Optuna)
    │
    └── README.md                 <- README файл

    
--------

## Результаты
С LAMA: Линейная модель и LightGBM (pooled_bert), Линейная модель и CatBoost (Random LSTM), BERT.
Собственные реализации: LogReg и ансамбль Transformers (distilbert и roberta) для оптимизации в обоих случаях использовалась Optuna.


|                 Model                 |    Log Loss  |
|:-------------------------------------:|:------------:|
|  AML Линейная модель + LightGBM       |    0.8488    |
|  AML Линейная модель + CatBoost       |    0.8479    |
|  **AML BERT**                         |  **0.9347**  |
|  No_AML LogReg + Optuna               |    0.7833    |
|  **No_AML Transformers + Optuna**     |  **0.9746**  |
