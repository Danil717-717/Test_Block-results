Задача: Написать программу, которая из имеющегося массива строк формирует массив из строк, длина которых меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

Примеры:

["hello", "2", "world", ":-)"] -> ["2", ":-)"]

["1234", "1567", "-2", "computer science"] -> ["-2"]

["Russia", "Denmark", "Kazan"] -> []

Решение задачи
Блок ввода массива из строк:
Согласно заданию, первоначальный массив вводися либо с клавиатуры, либо он задан на старте. Данный ввод реализован методом ввода с клавиатуры Yes или No.

При вводе Yes предлагается сначала ввести количество планируемых элементов массива строк (ввод реализован в виде функции InputNumbers), затем заполнить этот массив.
При вводе No первоначальный массив имеет значение: ["hello", "2", "world", ":-)"]
Переменная lengthLimit - согласно заданию равна 3

CheckArray - Метод подсчёта количества элементов, размер которых меньше lengthLimit
Подсчёт осуществляется перебором элементов массива arrayOfStrings и сравнением количества их элементов с переменной lengthLimit.
Результат выводится в переменную numberResult.
Инициализируется новый массив строк newArrayStrings, размером, равным переменной numbersResult.

FillNewArray - Метод формирования нового массива строк
Формирование осуществляется перебором элементов массива arrayStrings, сравнением количества их элементов с переменной lengthLimit и добавлением в массив newArrayStrings элемента, удовлетворяющего условию.
На выходе метода получается заполненный массив строк newArrayStrings, удовлетворяющий условию, что и является решением задачи.