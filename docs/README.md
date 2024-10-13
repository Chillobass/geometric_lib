
# How to use calculator:
1. Run `python calculate.py`
2. Enter the figure name. Available are Circle, Square.
3. Enter the function: Area or Perimeter.
4. Enter figure sizes. Radius for circle, one side for square.
5. Get the answer!

# Math formulas
## Area
- Circle: `S = πR²`
- Rectangle: `S = ab`
- Square: `S = a²`
- Triangle: `S = sqrt(p * (p-a) * (p-b) * (p-c))` where p is semiperimeter

## Perimeter
- Circle: `P = 2πR`
- Rectangle: `P = 2a + 2b`
- Square: `P = 4a`
- Triangle: `P = a + b + c`

# Описание решения:
## calculate.py
- В файле Пользователь задаёт 3 параметра:
- 1) фигуру
- 2) функцию
- 3) параметр фигуры(длина стороны/радиуса).
- Программа по заданным аргументам считает функцию(периметр или площадь) от фигуры(квадрат или круг) с заданным значением длины стороны или радиуса соответственно.

описание каждой функции с примерами вызова:
### def calc(fig, func, size)
Вычисляет значение указанной функции (периметр или площадь) для заданной фигуры (круг или квадрат) и выводит результат.

Пример вызова:
calc('circle', 'area', [5])
вывод -> 25п
calc('square', 'perimeter', [4])
вывод -> 16


## circle.py
- вспомогательный файл calculate.py , содержащий функции для него.
### def area(r)
Вычисляет площадь круга по радиусу r.

Вывод:
area(5)
получим -> 25п

### def perimeter(r)
Вычисляет периметр (длину окружности) круга по радиусу r.

Вывод:
perimeter(4)
получим -> 8


## square.py
- вспомогательный файл calculate.py , содержащий функции для него.

### def area(a)
Функция для вычисления площади квадрата.

Вывод:
area(5)
25

### def perimeter(a)
Функция для вычисления периметра квадрата.

Пример использования:
perimeter(5)
20


## triangle.py
- Файл с функциями, которые нигде не используются. Создан для грядущих обновлений (я полагаю).

### def area(a, b, c)
Функция для вычисления площади треугольника    
Вывод:
area(3, 4, 5)
6.0
### def perimeter(a, b, c)
Функция для вычисления периметра треугольника

Вывод:
perimeter(3, 4, 5)
12

# история изменения проекта
commit 365bcac0aa1affc24f91d7f1a3b401c543a5531f (HEAD -> comments)
Author: Mikael Burunsuzian <mitchelbur@gmail.com>
Date:   Sat Oct 12 12:18:41 2024 +0300

    added comments for each function in each file

commit b5b0fae727ca72c317c383b39c0af73d6adcd81c (origin/develop, develop)
Author: Daniil.K <dlkay@yandex.ru>
Date:   Tue Mar 30 18:02:23 2021 +0300

    L-04: Update docs for calculate.py

commit d76db2ac7f69cc920ae2e6f669fb0671a7fa7d71
Author: Daniil.K <dlkay@yandex.ru>
Date:   Tue Mar 30 17:57:42 2021 +0300

    L-04: Add calculate.py

commit 51c40ebfd0e0b65f52fe5e54740cbb038e492db3
Author: smartiqa <info@smartiqa.ru>
Date:   Fri Mar 26 14:52:26 2021 +0300

    L-04: Doc updated for triangle

commit d080c7888b81955bad2ed78d58ad910526b5132a
Author: smartiqa <info@smartiqa.ru>
Date:   Fri Mar 26 14:48:39 2021 +0300

    L-04: Triangle added

commit d078c8d9ee6155f3cb0e577d28d337b791de28e2 (origin/main, origin/HEAD, main)
Author: smartiqa <info@smartiqa.ru>
Date:   Thu Mar 4 14:55:29 2021 +0300

    L-03: Docs added

commit 8ba9aeb3cea847b63a91ac378a2a6db758682460
Author: smartiqa <info@smartiqa.ru>
Date:   Thu Mar 4 14:54:08 2021 +0300

    L-03: Circle and square added




