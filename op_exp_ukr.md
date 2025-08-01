# Оператори та вирази
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Operators and Expressions_

Більшість statements (логічних рядків), які ви пишете, міститимуть _вирази_. Простим прикладом виразу є `2 + 3`. Вираз можна розбити на оператори та операнди.

_Оператори_ — це певний функціонал, який виконує певні дії та який може бути представлений такими символами, як наприклад «+», або спеціальними ключовими словами. Операторам потрібні деякі дані для роботи, і такі дані називаються _операндами_. У цьому випадку "2" і "3" є операндами.

## Оператори
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Operators_

Ми коротко розглянемо оператори та їх використання.

Зверніть увагу, що ви можете обчислити вирази, наведені у прикладах, використовуючи інтерпретатор інтерактивно. Наприклад, щоб перевірити вираз `2 + 3`, скористайтесь інтерактивним командним рядком інтерпретатора Python:

::::{admonition} код Python (використовуючи idle)
```python
>>>2 + 3
5
>>>3 * 5
15
>>>
```
::::

Ось короткий огляд доступних операторів:

- `+`  (Плюс, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _plus_) 
    - Підсумовує два об'єкта
    - `3 + 5` дорівнює `8`. `'a' + 'b'` дорівнює `'ab'`.

- `-` (Мінус, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _minus_)
    - Дає віднімання одного числа від іншого; якщо перший операнд відсутній, він вважається нульовим.
    - `-5.2` дасть негативне число, а `50 - 24` дасть `26`.

- `*` (Mноження, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _multiply_)
    - Видає множення двох чисел або повертає рядок, що повторюється задане число разів.
    - `2 * 3` дорівнює `6`. `'la' * 3` дорівнює `'lalala'`.

- `**` (Піднесення до степеня, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _power_)
    - Повертає число х, зведене в ступінь y
    - `3 ** 4` дорівнює `81` (тобто `3 * 3 * 3 * 3`)

- `/` (Ділення, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _divide_)
    - Ділить x на y
    - `13 / 3` дорівнює `4.333333333333333`

- `//` (Цілочисельний поділ, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _divide and floor_)
    - Розділіть x на y та округліть відповідь _вниз_ до найближчого цілого значення. Зауважте, що якщо одне зі значень є числом з плаваючою комою, ви отримаєте значення з плаваючою комою.
    - `13 // 3`  дорівнює `4`
    - `-13 // 3` дорівнює `-5`
    - `9//1.81`  дорівнює `4.0`

- `%` (Поділ по модулю, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _modulo_) 
    - Повертає залишок від ділення
    - `13 % 3` дорівнює `1`. `-25.5 % 2.25` дорівнює `1.5`.

- `<<` (Оператори зсуву вліво на задану кількість біт, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _left shift_)
    - Зсуває біти числа вліво на задане число позицій. (Кожне число представлено в пам’яті бітами або двійковими цифрами, тобто 0 і 1)
    - `2 << 2` дорівнює `8`. У двійковій системи числення `2` представляє собою`10`.
    - Зрушення вліво на 2 біта дає «1000», що у десятковій системи числення означає 8.

- `>>` (Оператори зсуву вправо на задану кількість біт, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _right shift_)
    - Зсуває біти числа вправо на задане число позицій.
    - `11 >> 1` дорівнює `5`.
    - У двійковій системи числення `11` представлено в бітах як `1011` яке при зсуві вправо на 1 біт дорівнює `101` і яке є десятковим `5`.

- `&` (Побітове І, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bit-wise AND_)
    - Побітова операція І над числами: якщо обидва біти дорівнюють `1`, то результат дорівнює `1`. В іншому випадку це `0`.
    - `5 & 3` дорівнює `1` (`0101 & 0011` дорівнює `0001`)
    
- `|` (Побітове АБО, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bit-wise OR_)
    - Побітова операція АБО над числами: якщо обидва біти дорівнюють `0`, результат `0`.  В іншому випадку це `1`. 
    - `5 | 3` дорівнює `7` (`0101 | 0011` дорівнює `0111`)
    
- `^` (Побітове виключне АБО, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bit-wise XOR_)
    - Побітова операція виключне АБО над числами: якщо обидва біти (`1 або 0`) однакові, результат дорівнює `0`.  В іншому випадку це `1`. 
    - `5 ^ 3` дорівнює `6` (`O101 ^ 0011` дорівнює `0110`)

- `~`(Побітове НЕ, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bit-wise invert_) 
    - Побітова операція НЕ для числа x відповідає -(x+1)
    - `~5` дорівнює `-6`. Детальніше на  http://stackoverflow.com/a/11810203

- `<` (Менше ніж, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _less than_) 
    - Визначає чи вірно те, що x менше за y. Усі оператори порівняння повертають`True` або `False`. Зверніть увагу на написання цих імен з великої літери.
    - `5 < 3` дорівнює `False`, а `3 < 5` дорівнює `True`.
    - Можна складати довільні ланцюжки: `3 < 5 < 7` дає `True`.

- `>` (Більше ніж, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _greater than_)
    - Визначає чи вірно те, що x більше за y
    - `5 > 3` повертає `True`. Якщо обидва операнди є числами, вони спочатку перетворюються на однаковий тип. В іншому випадку завжди повертається `False`.

- `<=` (менше або дорівнює, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _less than or equal to_) 
    - Визначає чи вірно те, що x менше або дорівнює y
    - `x = 3; y = 6; x <= y` повертає `True`

- `>=` (більше або дорівнює, англ." ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _greater than or equal to_)
    - Визначає чи вірно те, що x більше або дорівнює y
    - `x = 4; y = 3; x >= 3` повертає `True`

- `==` (дорівнює, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _equal to_) 
    - Порівнює, чи однакові об'єкти
    - `x = 2; y = 2; x == y` повертає`True`
    - `x = 'str'; y = 'stR'; x == y` повертає `False`
    - `x = 'str'; y = 'str'; x == y` повертає `True`

- `!=` (не дорівнює, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _not equal to_) 
    - Порівнює, якщо об'єкти не рівні
    - `x = 2; y = 3; x != y` повертає `True`

- `not` (логічне НЕ, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _boolean NOT_)
    - Якщо x дорівнює `True`, оператор поверне `False`. Якщо ж x дорівнює `False`, отримаємо `True`.
    - `x = True; not x` повертає `False`.

- `and` (логічне І, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _boolean AND_) 
    - `x and y` повертає `False`,якщо x дорівнює `False`,в протилежному випадку(х=True) повертає значення y
    - `x = False; y = True; x and y` повертає `False` оскільки x є False. У цьому випадку Python не обчислюватиме y, оскільки він знає, що ліва частина виразу «and» має значення «False», що означає, що весь вираз буде «False» незалежно від інших значень. Це називається скороченою оцінкою булевих (логічних) виразів (англ. "short-circuit evaluation").

- `or` (логічне АБО, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _boolean OR_)
    - Якщо x дорівнює  `True`, він повертає True, в протилежному випадку отримаємо значення y
    - `x = True; y = False; x or y` повертає `True`.Тут також застосовується скорочена оцінка виразів.

## Короткий запис математичних операцій та привласнення

Зазвичай виконується математична операція над змінною, а потім привласнюється результат цієї операції тій самій змінній, отже, для таких виразів існує скорочення:

```python
a = 2
a = a * 3
```
можна записати як:

```python
a = 2
a *= 3
```

Зверніть увагу, що вирази виду  `var = var operation expression`("змінна = змінна операція
вираз") стає `var operation= expression`("змінна операція = вираз").

## Порядок обчислення
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _evaluation Order_

Якщо у вас є такий вираз, як «2 + 3 * 4», спочатку виконується додавання чи множення? Шкільний курс математики говорить нам, що спочатку потрібно виконати множення. Це означає, що оператор множення має вищий пріоритет, ніж оператор додавання.

У наcтупній таблиці нижче  наведено пріоритет операторів Python, починаючи з самого найнижчого пріоритету (найслабше зв'язування, англ."least binding") до найвищого пріоритету (найсильніше зв'язування, англ."most binding"). Це означає, що у будь-якому вираженні Python спочатку оцінить оператори та вирази, розташовані нижче в таблиці, а потім ті, що перераховані вище в таблиці.

Для повноти опису наведено наступну таблицю, взяту з [Посібника  мови Python (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Python reference manual_)](http://docs.python.org/3/reference/expressions.html#operator-precedence). Набагато краще використовувати  дужки для відповідного групування операторів і операндів, щоб явно вказати порядок обчислення виразів. Це робить програму більш читабельною. Див. [Зміна порядку оцінювання (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Changing the Order of Evaluation_)](#changing-order-of-evaluation) нижче для отримання додаткової інформації.

- `lambda` : Лямбда-вираз (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Lambda Expression_)
- `if - else`: Умовний вираз (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Conditional expression_)
- `or` : Логічне АБО (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Boolean OR_)
- `and` : Логічне І (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Boolean AND_)
- `not x` : Логічне НЕ (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Boolean NOT_)
- `in, not in, is, is not, <, <=, >, >=, !=, ==` : Порівняння, включаючи тести на приналежність і тести на тотожність
- `|` : Побітове АБО (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Bitwise OR_)
- `^` : Побітове ВИКЛЮЧНО АБО (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Bitwise XOR_)
- `&` : Побітове I (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Bitwise AND_)
- `<<, >>` : Зміщеня (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Shifts_)
- `+, -` : Додавання і віднімання(![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Addition and subtraction_)
- `*, /, //, %` : Множення, ділення, цілочисельне ділення та залишок від ділення (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Multiplication, Division, Floor Division and Remainder_)
- `+x, -x, ~x` : Позитивне, негативне, побітове НЕ (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Positive, Negative, bitwise NOT_)
- `**` : Піднесення до степеня (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Exponentiation_)
- `x[index], x[index:index], x(arguments...), x.attribute` : Звернення за індексом,зріз,виклик функції, посилання на атрибут (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Subscription, slicing, call, attribute reference_) 
- `(expressions,..), [expressions,..], {key: value,..}, {expressions...}` : Зв’язка або кортеж, список, словник, множина (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Binding or tuple display, list display, dictionary display, set display_)

Оператори, які ми ще не зустрічали, будуть пояснені в наступних розділах.

Оператори з _однаковим пріоритетом_ містяться в одному рядку у наведеній вище таблиці. Наприклад, «+» і «-» мають однаковий пріоритет.

## Зміна порядку обчислення 
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Changing the Order Of Evaluation_

Щоб зробити вирази більш зрозумілими, ми можемо використовувати круглі дужки.Наприклад, `2 + (3 * 4)` легше зрозуміти, ніж `2 + 3 * 4`, яке вимагає знання пріоритетів операторів. Як і в усьому іншому, дужки слід використовувати розумно (не перестарайтеся) і вони не повинні бути зайвими, як у `(2 + (3 * 4))`.

Є додаткова перевага використання круглих дужок - це допомагає нам змінити порядок обчислення.  Наприклад, якщо ви хочете, щоб додавання обчислювалося перед множенням у виразі, ви можете написати щось на зразок `(2 + 3) * 4`.

## Асоціативність

Оператори зазвичай обробляються зліва направо. Це означає, що оператори з однаковим пріоритетом обчислюються зліва направо. Наприклад, "2 + 3 + 4" обчислюється як "(2 + 3) + 4".

## Вирази
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _Expressions_

::::{admonition} код Python [expression_ukr.py](programs/expression_ukr.py)
:::{literalinclude} programs/expression_ukr.py
:::
**Висновок**:
:::{literalinclude} programs/expression_ukr.txt
:::
::::

**Як це працює**

Довжина і ширина прямокутника зберігаються в однойменних змінних (довжина та ширина) відповідно. Ми використовуємо їх для обчислення площі та периметра прямокутника за допомогою виразів. Ми зберігаємо результат виразу `довжина * ширина` у змінній `площа`, а потім друкуємо його за допомогою функції `print`. У другому випадку ми безпосередньо використовуємо значення виразу `2 * (довжина + ширина)` у функції друку.

Також зверніть увагу на те, як Python _"гарно друкує"_  результат. Навіть незважаючи на те, що  не вказано пробіл у кінці речення у лапках `'Площа дорівнює'`, Python розміщує його для нас, щоб ми отримали чистий гарний результат, і програма стала набагато читабельнішою таким чином (оскільки  не потрібно турбуватися про пробіли в рядках, які ми використовуємо для виведення(друку)). Це приклад того, як Python полегшує життя програміста.

##  Резюме

Ми побачили, як використовувати оператори, операнди та вирази - це основні будівельні блоки будь-якої програми. Далі ми побачимо, як використовувати їх у наших програмах за допомогою statements (операторів).




-- Від перекладачa --

## Розуміння двійкових цифр

[Двійкове число (![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _binary number_)](https://en.wikipedia.org/wiki/Binary_number) - це число, виражене у двійковій системі числення, використовуючи лише два різні символи, як 0 і 1.

Щоб краще зрозуміти двійкову систему числення, давайте спочатку розглянемо більш популярну [десяткову систему числення, ![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _decimal numeral system_](https://en.wikipedia.org/wiki/Decimal):

Вона містить 10 різних символів (0,1,2,3,4,5,6,7,8 і 9).

Щоб записати число більше 9, потрібно використати 2 або більше таких символів.

Наприклад, щоб записати число тридцять шість у десятковій системі, потрібно написати:

<pre>36</pre>

Тридцять шість — це двозначне число, тобто для його опису потрібні два символи. 

Якщо читати обидва символи зліва направо, вони утворюють інструкцію обчислення:

<pre>
36 (двозначне число)
розрахувати:
3 x 10 + 6 x 1 =
30 + 6 = 
36 
</pre>

Цікава частина цього полягає в тому, що лівий символ (3) має бути обчислений на 10, а правий символ (6) має бути обчислений на одиницю, а сума обох операцій представляє число.

Щоб записати число, більше 99, потрібні три цифри. Наприклад, щоб записати число дев'ятсот сорок два, потрібно написати:


<pre>942 (тризначне число)
читати зліва направо:
9 x 100 + 4 x 10 + 2 x 1 = 
900 + 40 + 2 = 
942</pre>

Оскільки число складається з трьох цифр, перший символ потрібно помножити на 100, другий на 10 і третій на 1. 

Цю десяткову систему числення також називають системою з основою 10.

Коефіцієнти для множення символів на (1,10,100,...) можна записати у вигляді степенів основи 10:

<pre>
10<sup>0</sup> =    1
10<sup>1</sup> =   10 
10<sup>2</sup> =  100
10<sup>3</sup> = 1000
і так далі...
</pre>

Інструкцію з розрахунку числа 942 також можна записати так:

<pre>
942:
9 x 10<sup>2</sup> + 4 x 10<sup>1</sup> + 2 x 10<sup>0</sup> =
9 x 100 + 4 x 10 + 2 x 1 =
900 + 40 + 2 = 
942
</pre>

### Двійкова система числення
Двійкова система має основу не 10, а 2:

<pre>
2<sup>0</sup> =   1
2<sup>1</sup> =   2
2<sup>2</sup> =   4
2<sup>3</sup> =   8
2<sup>4</sup> =  16
2<sup>5</sup> =  32
2<sup>6</sup> =  64
2<sup>7</sup> = 128
і так далі...
</pre>

Однозначні числа в двійковій системі можуть відображати тільки числа 0 і 1:

щоб виразити число нуль, ви пишете:

<pre>
0:
0 x 2<sup>0</sup> =
0 x 1 =
0
</pre>

щоб виразити число один, ви пишете:

<pre>
1:
1 x 2<sup>0</sup> =
1 x 1 =
1
</pre>

і для будь-якого числа, більшого за 1, необхідно більше цифр.

Для числа два ви пишете 10:

<pre>
10 (binary):
1 x 2<sup>1</sup> + 0 x 2<sup>0</sup>=
1 x 2 + 0 x 1=
2 (decimal)
</pre>

Для числа три ви пишете 11:

<pre>
11 (binary):
1 x 2<sup>1</sup> + 1 x 2<sup>0</sup>=
1 x 2 + 1 x 1=
2 + 1 =
3 (decimal)
</pre>

А для числа чотири потрібні вже три цифри:

<pre>
100 (у двійковій системі, чотири у десятковій системі)
1 x 2<sup>2</sup> + 0 x 2<sup>1</sup> + 0 x 2<sup>0</sup>=
1 x 4 + 0 x 2 + 0 x 1 =
4 + 0 + 0 =
4
</pre>

### Двійкові числа проти десяткових чисел

У цій таблиці порівнюються десяткова та двойкова системи числення

| 10-ва система | розрахунок| написання | 2-ва система | розрахунок|
| --: | --: | :--: | --: | --: |
|       0 | 0x10<sup>0</sup> |  нуль |  0  | 0x2<sup>0</sup>  |
|       1 | 1x10<sup>0</sup> |  один    |  1  | 1x2<sup>0</sup>  |
|       2 | 2x10<sup>0</sup> |  два    | 10   | 1x2<sup>1</sup>+0x2<sup>0</sup>  |
|       3 | 3x10<sup>0</sup> |  три  | 11 | 1x2<sup>1</sup>+1x2<sup>0</sup> |
|       4 | 4x10<sup>0</sup> |  чотири  | 100 | 1x2<sup>2</sup>+0x2<sup>1</sup>+0x2<sup>0</sup> |
|       5 | 5x10<sup>0</sup> |  п'ять   | 101 | 1x2<sup>2</sup>+0x2<sup>1</sup>+1x2<sup>0</sup> |
|       6 | 6x10<sup>0</sup> |  шість   | 110 | 1x2<sup>2</sup>+1x2<sup>1</sup>+0x2<sup>0</sup> |
|       7 | 7x10<sup>0</sup> |  сім | 111 | 1x2<sup>2</sup>+1x2<sup>1</sup>+1x2<sup>0</sup> |
|       8 | 8x10<sup>0</sup> |  вісім  | 1000 | 1x2<sup>3</sup>+0x2<sup>2</sup>+0x2<sup>1</sup>+0x2<sup>0</sup> |
|       9 | 9x10<sup>0</sup> |  дев'ять  | 1001 | 1x2<sup>3</sup>+0x2<sup>2</sup>+0x2<sup>1</sup>+1x2<sup>0</sup> |
|      10 | 1x10<sup>1</sup>+0x10<sup>0</sup> |  десять    | 1010 |  1x2<sup>3</sup>+0x2<sup>2</sup>+1x2<sup>1</sup>+0x2<sup>0</sup> |
|      11 | 1x10<sup>1</sup>+1x10<sup>0</sup> |  одинадцять | 1011 |  1x2<sup>3</sup>+0x2<sup>2</sup>+1x2<sup>1</sup>+1x2<sup>0</sup> |
|      12 | 1x10<sup>1</sup>+2x10<sup>0</sup> |  дванадцять | 1100 |  1x2<sup>3</sup>+1x2<sup>2</sup>+0x2<sup>1</sup>+0x2<sup>0</sup> |
|      13 | 1x10<sup>1</sup>+3x10<sup>0</sup> |  тринадцять| 1101 |  1x2<sup>3</sup>+1x2<sup>2</sup>+0x2<sup>1</sup>+1x2<sup>0</sup> |
|      14 | 1x10<sup>1</sup>+4x10<sup>0</sup> |  чотирнадцять | 1110 |  1x2<sup>3</sup>+1x2<sup>2</sup>+1x2<sup>1</sup>+0x2<sup>0</sup> |
|      15 | 1x10<sup>1</sup>+5x10<sup>0</sup> |  п'ятнадцять | 1111 |  1x2<sup>3</sup>+1x2<sup>2</sup>+1x2<sup>1</sup>+1x2<sup>0</sup> |
|      16 | 1x10<sup>1</sup>+6x10<sup>0</sup> |  шістнадцять | 10000 | 1x2<sup>4</sup>+0x2<sup>3</sup>+0x2<sup>2</sup>+0x2<sup>1</sup>+0x2<sup>0</sup> |

### Як перетворити двійкову систему у десяткову

Необхідно записати основу (2) у степені (цифр):

як перетворити число з основою 2 ```1001``` на число з основою 10 (```9``):

| число у двійковій системі: | 1 | 0 | 0 | 1 |
| ---               | - | - | - | - |
| степінь:        | 3 | 2 | 1 | 0 |
| =           | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup> | 2<sup>0</sup> |
| = | 8 | 4 | 2 | 1 |
|  розрахунок:  | 8 + | 0 + | 0 + | 1= |
| результат: 9 |||||

У Pyhton ви можете просто написати префікс ```0b``` перед числом, щоб вказати, що ви використовуєте двійкову систему. Python миттєво перетворює число на десяткову систему:
```python
>>>0b1001
9
```

###  Як перетворити десяткову систему у двійкову

Вам потрібно записати основу (2) у степені (цифри). Потім ви починаєте справа наліво встановлювати піднесення до степеня з основою 2 у порядку зростання, до того моменту поки сума всіх встановлених бітів є меншою або дорівнює числу з основою 10.

Приклад:

як перетворити число з основою 10 (```37```) у число з основою 2 (```100101```):
| степінь: | 5 | 4 | 3 | 2 | 1 | 0 |
| -- | -- | -- | -- | -- | -- | -- |
|       | 2<sup>5</sup> | 2<sup>4</sup> |  2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup> | 2<sup>0</sup> |
|   | 32 | 16 | 8 | 4 | 2 | 1  |
| встановлений біт: | 1 | 0 | 0 | 1 | 0 | 1 |
| 37 =       | 32+|0+|0+|4+|0+|1|
| двойкова система: **100101** |||||||


У Python ви просто використовуєте вбудовану функцію ```bin()```, щоб перетворити число з основою 10 у число з основою 2 (з префіксом ```0b```):

```python
>>>bin(37)
'0b100101'
```


## Оператори зсуву вліво на задану кількість біт
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _left shift operation_

_Дивіться також статтю у Вікіпедії про [Logical Shift](https://en.wikipedia.org/wiki/Logical_shift)_

Операцію зсуву вліво можна виконати лише для двійкового числа (з основою 2). Простіше кажучи, усі числа переміщуються ліворуч, а крайні праві позиції заповнюються нулями. Знаком оператора є ```<<```, і ви можете вказати, на скільки позицій ліворуч мають бути переміщені числа.

Приклад: виконайте операцію "зрушення вліво на 1" над двійковим числом ```1001``` (дев'ять за основою 10). Результат: ```10010``` (вісімнадцять за основою 10).


::::{admonition} код Python [`left_shift_ukr.py`](programs/left_shift_ukr.py)
```{literalinclude} programs/left_shift_ukr.py
```
**Висновок**:
:::{literalinclude} programs/left_shift_ukr.txt
::::

Зображення нижче зі статті у Вікіпедії:

MSB = старший біт, LSB = молодший значущий біт 

Зауважте, що біт, якби старший біт (MSB, число 7) був би 1, результуюче число було б більшим, як у прикладі вище.


::::{admonition} [left shift](img/Rotate_left_logically.svg.png) 
:class: seealso

:::{figure} img/Rotate_left_logically.svg.png
:figwidth: "image"

Опис зображення: 0001 0111 (десяткове число 23) логічно зсувається на один біт вліво, результат 0010 1110 (десяткове число 46).

Image rights: By <a href="https://en.wikipedia.org/wiki/User:Cburnett" class="extiw" title="en:User:Cburnett">en:User:Cburnett</a> - This W3C-unspecified <a href="https://en.wikipedia.org/wiki/Vector_images" class="extiw" title="w:Vector images">vector image</a> was created with <a href="https://en.wikipedia.org/wiki/Inkscape" class="extiw" title="w:Inkscape">Inkscape</a> ., <a href="http://creativecommons.org/licenses/by-sa/3.0/" title="Creative Commons Attribution-Share Alike 3.0">CC BY-SA 3.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=1505663">Link</a>
::::


## Оператори зсуву вправо на задану кількість біт
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _right shift operation_

_Дивіться також статтю у Вікіпедії про [Logical Shift](https://en.wikipedia.org/wiki/Logical_shift)_


Операція зсуву вправо працює трохи подібно до операції зсуву вліво: усі числа переміщуються праворуч, крайні ліві позиції заповнюються нулями, а числа, які були в крайній правій позиції, просто видаляються. 

Знаком оператора є ```>>```, і ви можете вказати, на скільки позицій праворуч слід перемістити кожне число.

Приклад: виконайте операцію «зсув праворуч на 1» над двійковим числом ```1001``` (дев’ять за основою 10). Результатом є ```0100``` і зазвичай записується без нуля на початку як ``` 100``` (чотири за основою 10).


::::{admonition} код Python [`right_shift_ukr.py`](programs/right_shift_ukr.py)
```{literalinclude} programs/right_shift_ukr.py
```

**Висновок**:
```{literalinclude} programs/right_shift_ukr.txt
```
::::

Зображення нижче зі статті у Вікіпедії:

MSB = старший біт, LSB = молодший значущий біт 

Зауважте, що на зображенні нижче молодший значущий біт (LSB) знищується
::::{admonition} [right shift](img/Rotate_right_logically.svg.png) 
:class: seealso

:::{figure} img/Rotate_right_logically.svg.png
:figwidth: "image"

Опис зображення: 0001 0111 (десяткове число 23) логічно зсувається на один біт вправо,результат буде: 0000 1011 (десяткове число 11)

Image rights: By <a href="https://en.wikipedia.org/wiki/User:Cburnett" class="extiw" title="en:User:Cburnett">en:User:Cburnett</a> - This W3C-unspecified <a href="https://en.wikipedia.org/wiki/Vector_images" class="extiw" title="w:Vector images">vector image</a> was created with <a href="https://en.wikipedia.org/wiki/Inkscape" class="extiw" title="w:Inkscape">Inkscape</a> ., <a href="http://creativecommons.org/licenses/by-sa/3.0/" title="Creative Commons Attribution-Share Alike 3.0">CC BY-SA 3.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=1505665">Link</a>
:::
::::






# Логічні оператори python
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _boolean operators_

| значення A | значення B | результат для AND | результат для OR |
| :--: | :--: | :--: | :--: |
| ```True``` |  ```True``` | ```True``` | ```True``` |
| ```True``` |  ```False``` | ```False``` | ```True``` |
| ```False``` | ```True``` | ```False``` | ```True``` |
| ```False``` | ```False``` | ```False``` | ```False``` | 

##  Логічне НЕ
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _NOT_

Оператор NOT дає значення інвертування: True стає False, а False стає True.

| операція | результат |
| -- | -- |
| ```not True``` | ```False``` |
| ```not False``` | ```True``` |

## Логічне І
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _AND_

Оператор AND повинен бути розміщений між двома логічними значеннями. Результатом буде True, якщо обидва логічні значення True, інакше результат буде False

| значення A | AND | значення B | результат | 
| :--: | :--: | :--: | :--: |
| ```True``` | AND |  ```True``` | = ```True``` | 
| ```True``` | AND |  ```False``` | =```False``` | 
| ```False``` | AND | ```True``` | =```False``` | 
| ```False``` | AND | ```False``` | =```False``` |

## Логічне АБО
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _OR_

Оператор АБО  має бути розміщено між двома логічними значеннями. Результат є True, якщо одне або обидва значення є True. Результатом буде False, якщо обидва значення є False.

| значення A | OR | значення B | результат  | 
| :--: | :--: | :--: | :--: |
| ```True``` | OR |  ```True``` | = ```True``` | 
| ```True``` | OR |  ```False``` | =```True``` | 
| ```False``` | OR | ```True``` | =```True``` | 
| ```False``` | OR | ```False``` | =```False``` |


## Логічні операції з двійковими цифрами
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _boolean operations with binary digits_

Логічні операції (and, or, xor, not) можуть бути застосовані не лише до логічних значень (True і False), а й безпосередньо до бітів (де 1 означає True, а 0 означає False). 

У Python є логічні команди ```not or and``` для логічних значень, але є також спеціальний набір команд для двійкових цифр:

```
~  Побітове НЕ (for bitwise inversion)
|  Побітове АБО (for bitwise OR)
&  Побітове І (for bitwise AND)
^  Побітове виключне АБО (for bitwise XOR)
```

###  Побітове НЕ
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bitwise inversion_

 `~` (bit-wise invert)
    - Побітова операція НЕ для числа  x відповідає -(x+1).
    Значення: до числа додається 0b01 і змінюється знак.

::::{admonition} код Python [`bitwise_inversion_ukr.py`](programs/bitwise_inversion_ukr.py)
:::{literalinclude} programs/bitwise_inversion_ukr.py
:::
**Висновок**:
:::{literalinclude} programs/bitwise_inversion_ukr.txt
:::
::::

###  Побітове І
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bitwise and_

- `&`(побітове І, англ."bit-wise AND")
    - Побітова операція І над числами: якщо обидва біти дорівнюють `1`, то результат дорівнює `1`. В іншому випадку це `0`.
    
| Приклад A | Приклад B | Приклад C | 
| :--: | :--: | :--: |
| 0b1100 | 0b1111 | 0b1011 |
| & | & | & |
| 0b0101 | 0b0000 | 0b0001 |
| = | = | = |
| 0b0100 | 0b0000 | 0b0001 |


## Побітне АБО
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bitwise or, inclusive OR_

- `|` (bit-wise OR)
    - Побітова операція АБО над числами: якщо обидва біти дорівнюють `0`, результат `0`.  В іншому випадку це `1`. 

    
| Приклад A | Приклад B | Приклад C | 
| :--: | :--: | :--: |
| 0b1100 | 0b1111 | 0b1011 |
| \| | \| | \| |
| 0b0101 | 0b0000 | 0b0001 |
| = | = | = |
| 0b1101 | 0b1111 | 0b1011 |

## Побітне ВИКЛЮЧНО АБО
![uk-flag](img/brit_flag.png){w=40px}{bdg-secondary-line}`англійська:` _bitwise xor, exclusive OR_

- `^` (bit-wise XOR) 
    - Побітова операція виключне АБО над числами: якщо обидва біти (`1 або 0`) однакові, результат дорівнює `0`.  В іншому випадку це `1`. 
    

| Приклад A | Приклад B | Приклад C | 
| :--: | :--: | :--: |
| 0b1100 | 0b1111 | 0b1011 |
| ^ | ^ | ^ |
| 0b0101 | 0b0000 | 0b0001 |
| = | = | = |
| 0b1001 | 0b1111 | 0b1010 |








