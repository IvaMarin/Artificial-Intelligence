# Лабораторная работа №1

| Студент           | Мариничев И. А. |
| ----------------: | :-------------: |
| **Преподаватель** | **Ахмед С. Х.** |

## Сравниваемые линейные модели

1. `MyMulticlassLogisticRegression` vs `LogisticRegression`
2. `MySVM`  vs `SVC`
3. `MyKNN` vs `KNeighborsClassifier`
4. `MyNaiveBayes` vs `GaussianNB`

## Результаты

|                                | Accuracy | Recall | Precision |
| -----------------------------: | :------: | :----: | :-------: |
| MyMulticlassLogisticRegression | 0.52     | 0.52   | 0.70      | 
| LogisticRegression             | 0.58     | 0.58   | 0.70      | 
| MySVM                          | 0.51     | 0.51   | 0.65      | 
| SVC                            | 0.64     | 0.64   | 0.74      | 
| MyKNN                          | 0.60     | 0.60   | 0.71      | 
| KNeighborsClassifier           | 0.59     | 0.59   | 0.71      | 
| MyNaiveBayes                   | 0.40     | 0.40   | 0.65      | 
| GaussianNB                     | 0.46     | 0.46   | 0.65      | 

## Выводы

Лучшей моделью по всем параметрам (кроме времени обучения :cry:) оказалась `SVC`, а из моих моделей лучшей оказалась `KNN`. Хотя стоит отметить, что все модели имеют не очень высокие значения метрик, это связано по большей части с особеностями самого набора данных. 

Лучше всего модели угадывают:
- `Lodgepole Pine (2)`
- `Spruce/Fir (1)`

а хуже всего:
- `Cottonwood/Willow (4)` 
- `Aspen (5)`
