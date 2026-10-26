# Отток клиентов телеком-оператора: разведочный анализ

Разведочный анализ (EDA) датасета [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) — 7 032 клиента телеком-компании с данными о подключённых услугах, договоре и платежах. Цель — понять, какие факторы связаны с уходом клиента, и подготовить данные для модели прогнозирования оттока.

![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![seaborn](https://img.shields.io/badge/seaborn-4C72B0)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/статус-в_работе-yellow)

## Что сделано

- Проверка структуры данных, типов и пропусков.
- Баланс классов: распределение целевой переменной `Churn`.
- Сравнение общей суммы платежей (`TotalCharges`) у ушедших и оставшихся клиентов.
- One-hot кодирование категориальных признаков.
- Корреляция каждого признака с оттоком — показывает, какие услуги, тип договора и способ оплаты сильнее всего связаны с уходом клиента.

## Дальнейшие шаги

- Обучение моделей классификации (логистическая регрессия, градиентный бустинг) и сравнение по ROC-AUC и recall для класса «ушёл».
- Учёт дисбаланса классов.
- Интерпретация важности признаков для бизнеса.

## Структура

```
.
├── ml_customer_project.ipynb   # ноутбук с анализом
├── Telco-Customer-Churn.csv    # исходные данные
└── requirements.txt
```

## Запуск

```bash
pip install -r requirements.txt
jupyter notebook ml_customer_project.ipynb
```

## Автор

Куценко Игорь — [@igr43](https://github.com/igr43)
