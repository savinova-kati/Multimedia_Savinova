Работу выполнилa 
Студентка группы: М8О-407Б-21 
Савинова Екатерина Ильинична

# Выбор датасета

Будем использовать набор данных о недвижимости California Housing, классический набор данных для прогнозирования цен на жилье.
Преобразует данные для двух задач:
- Классификация (по категориям цен - дорого, средне, дешево).
- Регрессия (предсказание цены).

Датасет широко используется для предсказания стоимости недвижимости на основе ряда факторов, таких как доход, плотность населения, уровень образования, средний возраст зданий и другие.

# Метрики

Для классификации я выбираю две метрики: accuracy и F1.

Для регрессии - MSE, для оценивания крупных ошибок.

Таблица с результатами работы программ во всех лабораторных работах.

| Алгоритм | Задача | Бейзлайн | Улучшенный бейзлайн | Самостоятельная имплементация |
| - | - | - | -- | -- |
| KNN | Классификация | Accuracy = 0.74, F1 = 0.74 | Accuracy = 0.77, F1 = 0.77 | Accuracy = 0.77 |
| | Регрессия | MSE = 0.43 | MSE = 0.37 | MSE = 0.37 |
| Линейные модели | Классификация | Accuracy = 0.7456, F1 = 0.7416 | Accuracy = 0.7469, F1 = 0.7428 | - |
| | Регрессия | MSE = 0.5559 | MSE = 0.5483 | - |
| Решающее дерево | Классификация | Accuracy = 0.75, F1 = 0.75 | Accuracy = 0.77, F1 = 0.77 | Accuracy = 0.49, F1 = 0.33 |
| | Регрессия | MSE = 0.49 | MSE = 0.41 | MSE = 0.75 |
| Случайный лес | Классификация | Accuracy = 0.8319, F1 = 0.8304 | Accuracy = 0.8333, F1 = 0.8320 | Accuracy = 0.65 |
| | Регрессия | MSE = 0.2553 | MSE = 0.2552 | MSE = 0.2536 |
| Градиентный бустинг | Классификация | Accuracy = 0.8270, F1 = 0.8263 | Accuracy = 0.8561, F1 = 0.8554 | Accuracy = 0.6262 |
| | Регрессия | MSE = 0.2940 | MSE = 0.2071 | MSE = 0.6424 |

# Вывод

Исходя из результатов, занесенных в таблицу, можно заметить, что методы, реализованные вручную, уступают встроенным. Это может быть связано с возможными погрешностями в самостоятельной реализации. Также наблюдается, что улучшенный бейзлайн превосходит обычный, что можно объяснить оптимизацией гиперпараметров для каждого алгоритма. Один из лучших результатов показал алгоритм градиентного бустинга с улучшенным бейзлайном.
