# Контрольная работа
1. Создать репозиторий на GitHub
2. Нарисовать блок-схему алгоритма 
3. Снабдить репозиторий оформленным текстовым описанием решения 
4. Написать программу, решаюшую поставленную задачу
5. Использовать конроль версий в работенад этим небольшим проектом.


# Решение задач:
1. Создать репозиторий на GitHub

*Ссылка на репозиторий: https://github.com/SemenBaranov/control.git*

2. Нарисовать блок-схему алгоритма

*Блок схема алгоритма:* ![diagrama](https://github.com/SemenBaranov/control/blob/main/diagrama.png)

3. Снабдить репозиторий оформленным текстовым описанием решения

*Ссылка на файл Readme.md 
<https://github.com/SemenBaranov/control/blob/main/Readme.md>*

4. Написать программу, решаюшую поставленную задачу

"Напишите программу, которая принимает на вход трёхзначное число и на выходе показывает вторую цифру этого числа." 

int number = ReadInt("Введите трехзначное число: ");
int amount = number.ToString().Length;

if (amount < 3 || amount > 3)
{
    Console.WriteLine("Вы ввели не трехзначное число");
}
else
{
    Console.WriteLine(InCenter(number));
}
int ReadInt(string message)
{
    Console.Write(message);
    return Convert.ToInt32(Console.ReadLine());
}


int InCenter(int a)
{
    
    int result = ((a / 10) % 10);
    return result;
}