# 1. Представление чисел
Вычислить произведение длин своих имени, фамилии и отчества. Вывести на экран двоичное представление следующих величин в указанных форматах данных:

А) отрицательного 32-битного целого, модуль которого равен найденному произведению;

Б) положительного числа с плавающей запятой единичной точности по стандарту IEEE 754, модуль которого равен найденному произведению;

В) отрицательного числа с плавающей запятой двойной точности по стандарту IEEE 754, модуль которого равен найденному произведению.


# 2. Пифагоровы тройки
Пифагоровой тройкой называют тройку натуральных чисел (x,y,z), удовлетворяющих условию $x^2 + y^2 = z^2$. Пифагорова тройка называется примитивной, если числа, её составляющие, взаимно просты. Для введённых пользователем трёх чисел определить, являются ли они пифагоровой тройкой, и если да, являются ли они также простой пифагоровой тройкой. Порядок, в котором числа вводятся, произвольный.

# 3. Углы треугольника
Определить, можно ли, исходя из трёх введённых пользователем чисел, построить невырожденный треугольник с соответствующими сторонами. Если возможно, определить его углы в градусах, минутах и секундах с точностью до секунды. Предусмотреть ввод пользователем чисел с дробной частью.

# 4. Числа Мерсенна
Числами Мерсенна называются числа вида 2N -1, где N – натуральное число. Вывести на экран все простые числа Мерсенна на отрезке $[1; 2^31 - 1]$.

# 5. Цепные дроби
Цепная дробь – конечное или бесконечное выражение вида
$[a_0; a_1, a_2, a_3, ...] = a_0 + 1/(a_1 + 1/(a_2+ 1/(a_3+...)))$,
где $a_0$ – целое, остальные $a_i$ – натуральные числа. Любое вещественное число представимо в виде цепной дроби, при этом рациональные числа представляются конечной цепной дробью, иррациональные – бесконечной. Квадратный корень целого числа, не являющегося квадратом другого целого, является иррациональным числом. Цепная дробь квадратного корня обладает таким свойством, что начиная со следующего за некоторым $а_i a_j=a_{j-i}: a_{i+1}=a_1, a_{i+2}=a_2$ и т.д. i называют периодом данной цепной дроби. Для введённого пользователем числа, не являющегося квадратом целого, вывести период i и последовательность $[a_0; a_1…a_i]$.

# 6. Сортировка строк
Написать программу для сортировки строк в текстовом файле с использованием механизма файлов, отображаемых на память (memory mapped files). Строки в файле оканчиваются по правилам операционной системы (\n или \r\n). В качестве компаратора можно использовать любой адекватный поставленной задаче. Для примера достаточно больших текстовых файлов можно брать файлы с геномами из https://www.ncbi.nlm.nih.gov/genome.

# 7. Хэш-таблица
Создать структуру данных для хэш-таблицы и определить для неё следующие операции:
- Вставка нового ключа и значения. При этом при достижении некоторого условия (например, слишком длинный список для одной из корзин относительно общего числа элементов в хэш-таблице) должна происходить перебалансировка хэш-таблицы.
- Поиск значения по ключу. В случае, если ключ не найден, возвращается некоторое заранее определённое значение.
- Удаление ключа и значения. Если ключ не найден, ничего не происходит. Обратная перебалансировка не требуется.

# 8. Фильтры
Требуется написать программу, получающую из командной строки следующие данные:
- Имя входного файла.
- Тип фильтра.
- Имя выходного файла.
Входной файл представляет из себя 24-битный или 32-битный BMP-файл без сжатия, но, возможно, с палитрой. Требуется считать из него данные об изображении и применить к нему один из следующих фильтров согласно переданному параметру:
- Усредняющий фильтр 3x3.
- Усредняющий фильтр Гаусса 3x3 или 5x5. Допустимо использование других размеров фильтра, если будут правильно подобраны параметры гауссианы.
- Фильтр Собеля по X. Допустимо использовать вместо него фильтр Щарра.
- Фильтр Собеля по Y. Допустимо использовать вместо него фильтр Щарра.
- Перевод изображения из цветного в оттенки серого.
Полученное изображение необходимо сохранить по указанному пути выходного файла в формате BMP. Полученный файл должен открываться стандартными средствами просмотра изображений.
Возможный пример командной строки для использования программы: MyInstagram C:\Temp\1.bmp SobelX C:\Temp\2.bmp

# 9. Менеджер памяти
Реализовать набор из следующих функций и показать их работоспособность:
- void* myMalloc(size_t size) – аналог функции malloc;
- void myFree(void* ptr) – аналог функции free;
- void* myRealloc(void* ptr, size_t size) – аналог функции realloc;
- void init() – вспомогательная функция, инициализирующая необходимые структуры данных;
В функции init() происходит выделение большой области динамической памяти штатными средствами. Выделение памяти в реализуемых функциях должно происходить в этой области. За пределами функции init() нельзя использовать функции malloc, realloc и free.

# 10. Английские монеты
В Англии в обращении находятся монеты следующего достоинства: 1 пенс, 2 пенса, 5 пенсов, 10 пенсов, 20 пенсов, 50 пенсов, 1 фунт (100 пенсов) и 2 фунта (200 пенсов). Пользователь вводит натуральное число, обозначающее некоторую сумму денег в пенсах. Вывести на экран количество способов, которыми эту сумму можно набрать, пользуясь любым количеством любых английских монет.

# 11. Цифровой корень
Цифровым корнем называется число в десятичной системе счисления, полученное из цифр исходного числа путём их сложения и повторения этого процесса над полученной суммой до тех пор, пока не будет получено число, меньшее 10. Например, цифровой корень 467 равен 8.
Известно, что составное число можно разложить на множители различными способами, например
24 = 2x2x2x3 = 2x3x4 = 2x2x6 = 4x6 = 3x8 = 2x12 = 24.
В данном случае умножение на единицу не рассматривается.
Назовём суммой цифровых корней сумму цифровых корней отдельных множителей в разложении составного числа. Например, для 24:
Разложение - Сумма цифровых корней
2x2x2x3 - 9
2x3x4 - 9
2x2x6 - 10
4x6 - 10
3x8 - 11
2x12 - 5
24 - 6
В этом случае максимальная сумма цифровых корней равна 11.
Обозначим максимальную сумму цифровых корней среди всех разложений числа n на множители как MDRS(n).
Вычислить сумму всех MDRS(n) при n=[2; 999999]

# 12. Длинная арифметика
Вычислить с помощью алгоритмов длинной арифметики значение числа 3^5000 и представить его в шестнадцатеричной системе счисления.