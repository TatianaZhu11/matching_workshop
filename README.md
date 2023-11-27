# matching_workshop

Цель работы: разработать алгоритм, который для множества товаров А подбирает несколько вариантов наиболее похожих товаров из множества В.

Описание данных
base.csv - анонимированный набор товаров. Каждый товар представлен как уникальный id и вектор признаков размерностью 72. train.csv - каждая строка - один товар, для которого известен уникальный id, вектор признаков и id товара из base, который максимально похож на него. validation.csv - товары, для которых требуется найти наиболее близкие товары из base.csv.

Наилучшие показатели качества поиска похожих товаров удалось достичь с помощью:
•	библиотки FAISS,
•	масштабирования признаков с помощью RobustScaler,
•	удаления признаков, распределение которых отклонялось от нормального,
•	выделения наиболее значимых признаков с помощью иерархической кластеризации.
•	
Accuracy@5 составила 67.466.

