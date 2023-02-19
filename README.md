# ControlWork

## Задача: 
Написать программу, которая из имеющегося массива строк формирует массив из строк, *длина которых меньше либо равна 3 символам*. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

* Нарисована **Блок-схема** (графическое представление метода) в приложении _diagrams.net_, далее была загружена мной в данный репозиторий в формате *.png*.  

* Программа по прешению данной задачи написанна на языке ***C#***
```C#
string[] array1 = new string[5] {"Hi", "569", "Angel", "the", "array"};
string[] array2 = new string[array1.Length];
void SecondArrayWithIF(string[] array1, string[] array2)
{
    int count = 0;
    for (int i = 0; i < array1.Length; i++)
    {
    if(array1[i].Length <= 3)
        {
        array2[count] = array1[i];
        count++;
        }
    }
}
void PrintArray(string[] array)
{
    for (int i = 0; i < array.Length; i++)
    {
        Console.Write($"{array[i]} ");
    }
    Console.WriteLine();
}
SecondArrayWithIF(array1, array2);
PrintArray(array2);
```
