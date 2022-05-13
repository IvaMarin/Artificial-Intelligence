# Лабораторная работа №0

| Студент            | Мариничев И. А. |
| -----------------: | :-------------: |
| **Преподаватель**  | **Ахмед С. Х.** |

## Описание набора данных

Будем работать с данными `covtype.data` о типе лесного покрытия из репозитория UCI. 

Доступно 7 различных классов:

| [Spruce/Fir](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type1.jpg) | [Lodgepole Pine](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type2.jpg)|[Ponderosa Pine](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type3.jpg) | [Cottonwood/Willow](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type4.jpg)| [Aspen](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type5.jpg)| [Douglas-fir](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type6.jpg)| [Krummholz](https://github.com/IvaMarin/Artificial-Intelligence/blob/main/Machine-Learning/ml_lab0/img/cover_type7.jpg)|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| *1* | *2* |*3* | *4* | *5* |*6* | *7* |

Каждый объект описывается 54 признаками. Более подробно они описаны в файле `covtype.info`. 

Скачать данные: http://archive.ics.uci.edu/ml/datasets/Covertype

## Постановка решаемой задачи

Поставим задачу классификации - определить тип лесного покрова. 

## Порядок действий

1. Cкачать данные и привести их к типу .csv (comma-separated values)
2. Добавить названия столбцов в соответствии с `covtype.info`
3. Разделить набор данных на тестовый, тренировочный и валидационный
4. Провести анализ на чистоту данных и отсутствие бесполезных значений
5. Разделить признаки на числовые и категориальные, чтобы работать с ними отдельно
6. Произвести анализ зависимостей для числовых признаков:
    - графики распределений,
    - двойные графики
    - матрица корреляций
7. Произвести графический анализ зависимостей для категориальных признаков
8. Добавить при необходимости или удалить признаки, исходя из проведенного анализа
9. Провести тестовое обучение модели и посмотреть на точность

## Выводы

Набор данных о типе лесных покровов предоставляет довольно интересные возможности для анализа. К сожалению, почти все признаки в отдельности имеют довольно низкую корреляцию с типом лесного покрова, что не позволяет достичь максимальной точности. Кроме того, некоторые признаки оказались коллинеарными и их пришлось исключить. После пробного обучения модели *RandomForestClassifier* была достигнута точность 0.75 на тестовых данных.
