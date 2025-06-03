## Описание проекта

В рамках данного проекта была проведена комплексная обработка и анализ данных для предсказания биоактивности лекарственных препаратов. Целью исследования являлось разработка моделей машинного обучения, способных предсказывать три ключевых параметра: **IC₅₀** (полумаксимальная ингибирующая концентрация), **CC₅₀** (полумаксимальная цитотоксическая концентрация) и **SI** (индекс селективности). Также рассматривались задачи классификации на основе этих параметров.

Для решения поставленных задач были использованы методы исследовательского анализа данных (EDA), предобработки данных, построения и оценки моделей регрессии и классификации.

### 1. Структура репозитория
```
├── data
│   ├── cleaned_data.xlsx          # Очищенные данные
│   └── farmacydata.xlsx           # Исходные данные
├── reports
│   ├── classification_cc50_median_metrics.xlsx            # Метрики качества для классификации CC50 > медиана
│   ├── classification_cc50_median_feature_importance.xlsx # Важность признаков для классификации CC50 > медиана
│   ├── classification_ic50_median_metrics.xlsx            # Метрики качества для классификации IC50 > медиана
│   ├── classification_ic50_median_feature_importance.xlsx # Важность признаков для классификации IC50 > медиана
│   ├── classification_si_8_metrics.xlsx                   # Метрики качества для классификации SI > 8
│   ├── classification_si_8_feature_importance.xlsx        # Важность признаков для классификации SI > 8
│   ├── classification_si_median_feature_importance.xlsx   # Важность признаков для классификации SI > медиана
│   ├── classification_si_median_metrics.xlsx              # Метрики качества для классификации SI > медиана
│   ├── regression_cc50_metrics.xlsx                       # Метрики качества для регрессии CC50
│   ├── regression_cc50_feature_importance.xlsx            # Важность признаков для регрессии CC50
│   ├── regression_ic50_metrics.xlsx                       # Метрики качества для регрессии IC50
│   ├── regression_ic50_feature_importance.xlsx            # Важность признаков для регрессии IC50
│   ├── regression_si_metrics.xlsx                         # Метрики качества для регрессии SI
│   └── regression_si_feature_importance.xlsx              # Важность признаков для регрессии SI
├── notebooks
│   ├── classification_cc50_median.ipynb                   # Ноутбук для классификации CC50 > медиана
│   ├── classification_ic50_median.ipynb                   # Ноутбук для классификации IC50 > медиана
│   ├── classification_si_8.ipynb                          # Ноутбук для классификации SI > 8
│   ├── classification_si_median.ipynb                     # Ноутбук для классификации SI > медиана
│   ├── EDA.ipynb                                          # Ноутбук для исследовательского анализа данных
│   ├── regression_cc50.ipynb                              # Ноутбук для регрессии CC50
│   ├── regression_ic50.ipynb                              # Ноутбук для регрессии IC50
│   └── regression_si.ipynb                                # Ноутбук для регрессии SI
├── README.md                                              # Документация проекта
├── requirements.txt                                       # Необходимые библиотеки
└── report.pdf                                             # Аналитический отчёт
```

### 2. Установка и запуск
Для установки и запуска проекта выполните следующие шаги:

1. Установите необходимые библиотеки:
```bash
pip install -r requirements.txt
```

2. Запустите Jupyter Notebook:
```bash
jupyter notebook
```

3. Откройте соответствующие ноутбуки в папке `notebooks` и выполните их.
