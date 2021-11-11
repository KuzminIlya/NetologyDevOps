# 2.4. Инструменты Git, Кузьмин Илья (поток 2)

**Склонированный репозиторий**

![ins](resources/ins.jpg)

1. Полученный полный хэш - aefead2207ef7e2aa5dc81a34aedf0cad4c32545. Получено с пом. команды
git show. Поиск можно проводить даже по четырем первым символам - тогда в подсказке будут выданы
разные совпадающие варианты.

![ins_1](resources/ins_1.jpg)

2. На коммите стоит тег - v0.12.23. Об этом можно узнать с пом. того же git show 85024d3 с подробной инфой о коммите
или вывести краткую инфу по команде git log 85024d3 --oneline -1

![ins_2](resources/ins_2.jpg)

3. У заданного коммита два родителя: 56cd7859e05c36c06b56d013b55a252d0bb7e158 и 9ea88f22fc6269854151c571162c5bcf958bee2b
Сперва была выполнена команда git log b8d720 --oneline --graph, чтобы увидеть дерево коммитов

![ins_3](resources/ins_3.jpg)

Затем с пом. команд git show b8d720^ и git show b8d720^2 мы посмотрели описание коммитов-родителей

![ins_4](resources/ins_4.jpg)

![ins_5](resources/ins_5.jpg)

Еще, т.к. наш у нас мерж коммит, это можно увидеть, если выполнить просто команду git show b8d720

![ins_6](resources/ins_6.jpg)

4. Список хэшэй и сообщений, полученных с пом. команды git log --oneline v0.12.23^..v0.12.24

![ins_7](resources/ins_7.jpg)

5. Хэш коммита с добавлением функции - 8c928e835.
Узнаем в каком коммите добавлена функция git log -S "func providerSource(" --oneline

![ins_8](resources/ins_8.jpg)

Убеждаемся в том, что функция была добавлена git show 8c928e835

![ins_9](resources/ins_9.jpg)

6. Находим файл, где определяется функция с пом. команды git grep "globalPluginDirs"

![ins_10](resources/ins_10.jpg)

Теперь получаем коммиты, где эта функция изменялась в данном файле с пом. команды 
git log -s --oneline -L :globalPluginDirs:plugins.go

![ins_11](resources/ins_11.jpg)

7. Находим коммиты с изменениями этой функции git log --oneline -S "synchronizedWriters"

![ins_12](resources/ins_12.jpg)

Смотрим инфу по коммиту, где была добавлена функция git show 5ac311e2a

![ins_13](resources/ins_13.jpg)





