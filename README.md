Разбор 3 методов для решения задачи классификации
=====================

Установка
---------

Для запуска кода нужно запустиь файл либо в Google colab, либо на локальной машине, установив при этом 
необходимые модули python

```shell script
pip install tensorflow
pip install keras
pip install sklearn
pip install matplotlib
pip install numpy
```

Теория
------
 В данной работе разберем 3 метода.
 
 1)Нейронная сеть многослойный персептронс дополнительным нормальным шумом
 
 2)Наивный классификатор Байеса
 
 3)Рандомное дерево решений
 
 Для начала работы необходимо считать данные из txt файлов. Затем представить их в виде многомерных массивов и отнормализовать. (нужно вычесть среднее значение по столбцу и поделить на дисперсию по столбцу).
 
Практика
--------
 В результате получены данные:
 
 1)Нейронная сеть обучается довольно долго (40 эпох минимум), однако ее точность (доля верных ответов) на тестовой выборке выше всех –0.98. Нормальный шум добавлен для того, чтобы модель не переобучилась на обучающей выборке.
 
 2)Наивный классификатора байеса с ядром гаусса и бернулли показали средний результат –0,93 и 0,6 соответственно, однако у них есть сильная сторона –высокая скорость обучения и простота реализации 
 
 3)Дерево рандомных решений показало на тестовой выборке 0,95. Что в целом вполне оптимально по соотношению к точности и скорости обучения.
 
 Выводы: рандомное дерево решений – оптимальный вариант для решения поставленной задачи
 --------------------------------------------------------------------------------------
