# Вводная документация по C#
В данной документации будут рассмотрены базовые принципы работы с языком программирования, синтаксис таких конструкций как метод, класс, точка входа. Будет рассмотрена нотация или правила написания методов классов, переменных.
## Нотация
Перед тем как приступить к самому языку и его синтаксису, разберём его правила написания, которые используют сами разработчики языка.

### PascalCase

Все слова пишутся слитно и с большой буквы.
```
//ВотПримерНаРусскомЯзыке
```
Данная нотация используется при написании:
классов,методом,публичных переменных.

### camelCase

Принцип тот же, но первое слово пишется с маленькой буквы.
```
//такЖеПример
```
Данная нотация используется при создании приватных переменных.

### SNAKE-CASE

В данной нотации все слова пишутся с большой буквы и разделены чертой, используется при создании константных переменных.
``` C#
public const int MONTH-COUNT = 12
```
### Правильная нотация
Правильная нотация приучает писать код более понятным, с правильной нотацией не нужно вспоминать что мы написали, мы сразу понимаем, метод или класс перед нами или же переменная.

## Типы в C#

под типом мы подразумеваем определенный объект, который несёт в себе определенные данные: число, строка, символ и т.д, так как C# является статическим или типизированные языком программирования, то мы не можем в один тип положить другой.

### INT целое число
Данный тип представляет собой структуру, или же переменная = значение. В нем мы можем хранить числа без дробной части.

```C#
int year = 2024;
```
Мы не можем положить в нее строку или дробное число, будет ошибка типизации, но с дробным числом есть особенность, если мы захотим положить число с дробной частью, то нам нужно явно преобразовать в другой тип.

```C#
public double Mass = 123,45d;
int massInt = (int)Mass; //123
```
В данном примере мы присвоили к целочисленной переменной число с дробной частью, но при явном преобразовании мы потеряли дробную часть.

### double и float числа с дробной частью

Два данных типа данных являются числом с дробной частью или число с плавающей точкой. Их отличие заключается в количестве знаков после запятой, у double число больше.

### bool состояние

Данный тип имеет два состояния лож false и истина true.

### char и string
char является типом данных который хранит в себе символ. Переменная с типом char заключается в одинарные кавычки.
Тип string является строчным типом данных и хранит в себе массив символов.
```C#
string name = "MyName";
char i = 'i';
```
