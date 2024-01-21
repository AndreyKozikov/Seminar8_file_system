## Файловая система
*Функции:*
1. Добавление данных
2. Удаление данных
3. Изменение данных
4. Вывод данных
5. Копирование данных

**ui.py** - отвечает за взаимодействие программы с пользователем

**main.py** - главный файл, который вызывает всю цепочку

**db** - папка, в которой хранится 2 файла.

При выполнении домашнего задания в новой функции копирования данных максимально использован код, представленный в исходном проекте, для чего
исходный код некоторых функций проекта модифицирован: однотипные повторяющиеся операции в разных функциях 
вынесены в файл `support_func.py`

Меню вынесено в файл `menu.txt` (для чего модифицирован код файла `ui.py`), в который теперь можно вносить 
новые пункты меню в следующем формате
```
<порядковый номер пункта меню>;<описание действия>;<имя функции в коде без скобок>
```
Дополнительной модификации кода файла `ui.py`, отвечающего за меню, не требуется. Достаточно описать новую функцию в коде и
импортировать ее в `ui.py`. Вызов нужных функций происходит через словарь `globals()`
