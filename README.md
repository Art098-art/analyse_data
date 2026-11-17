# analyse_data
I just try to study for machine learning

# ML Start 2026. ДЗ #1

## Датасет
Online Shoppers Purchasing Intention (Kaggle, 12.3k строк).
Бинарная классификация: купит ли посетитель (Revenue).
Выбрал из-за сильного дисбаланса классов и смеси числовых и категориальных признаков.

Данные: https://www.kaggle.com/datasets/imakash3011/online-shoppers-purchasing-intention-dataset

## Гипотезы (сформулированы до начала работы)
1) Отбор 5 лучших признаков через SelectKBest не ухудшит ROC-AUC сильно
2) Подбор гиперпараметров даст прирост к дефолтной модели
3) Самыми важными по feature importance окажется PageValues
4) LogReg справится не хуже Random Forest по ROC-AUC

## Результаты
| № | Гипотеза | Вывод | Комментарий |
|---|----------|-------|-------------|
| 1 | F1 macro vs accuracy | Подтвердилась | accuracy 0.89, F1 macro 0.75, разрыв 14 п.п. |
| 2 | ... | Частично | ... |

## Как запустить
pip install -r requirements.txt
jupyter notebook research.ipynb
