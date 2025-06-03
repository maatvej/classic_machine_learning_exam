## Описание проекта

В рамках этого проекта была проведена обработка и анализ данных с целью прогнозирования биоактивности лекарственных препаратов. Целью исследования было создание моделей машинного обучения, способных предсказывать три основных параметра: SI (индекс селективности), CC50 (полумаксимальная цитотоксическая концентрация) и IC50 (полумаксимальная ингибирующая концентрация). Эти параметры также использовались для изучения задач классификации.

Исследовательский анализ данных (EDA), предобработка данных, создание и оценка моделей регрессии и классификации — все это было использовано для решения поставленных задач.

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
