# 2.3. Ветвления в Git, Кузьмин Илья (поток 2)

## Задание 1. Ветвление, merge и rebase.

1. Подготовка - создаем файлы merge.sh и rebase.sh

* **Начальное состояние репозитория**

![start_rep_state](resources/start_rep_state.jpg)

* **После подготовительного коммита**

![init_commit_1](resources/init_commit_1.jpg)

![init_commit_2](resources/init_commit_2.jpg)

2. Подготовка merge.sh

* **Создаем ветку Merge**

![merge_commit_1](resources/merge_commit_1.jpg)

* **Заливаем в нее изменения соотв. файла**

![merge_commit_2](resources/merge_commit_2.jpg)

* **Граф после добавление ветки Merge**

![merge_commit_3](resources/merge_commit_3.jpg)

3. Изменения в ветке master

* **Меняем файл Rebase.sh**

![master_commit_1](resources/master_commit_1.jpg)

* **Граф после коммита в master**

![master_commit_2](resources/master_commit_2.jpg)

4. Подготовка rebase.sh

* **Создаем из master ветку Rebase и меняем в ней файл Rebase.sh**

![rebase_commit_1](resources/rebase_commit_1.jpg)

![rebase_commit_2](resources/rebase_commit_2.jpg)

* **Граф после коммитов в Rebase**

![rebase_commit_3](resources/rebase_commit_3.jpg)

5. Merge

* **Мержим ветку Merge в Master**

![merge_master_1](resources/merge_master_1.jpg)

![merge_master_2](resources/merge_master_2.jpg)

* **Граф после мержа**

![merge_master_3](resources/merge_master_3.jpg)

P.S. В системном файле были изменения (забыл добавить в .gitignore ранее, поэтому мерж прошел с конфликтом в этом файле)

6. Rebase

* **Переключаемся на ветку Rebase**

![rebase_master_1](resources/rebase_master_1.jpg)

* **Вызываем git rebase**

![rebase_master_2](resources/rebase_master_2.jpg)

* **Решаем конфликт**

![rebase_master_3](resources/rebase_master_3.jpg)

* **Завершаем rebase**

![rebase_master_4](resources/rebase_master_4.jpg)

* **Пытаемся запушить без force**

![rebase_master_5](resources/rebase_master_5.jpg)

* **Пушим с атрибутом -f**

![rebase_master_6](resources/rebase_master_6.jpg)

* **Мержим rebase и master**

![rebase_master_7](resources/rebase_master_7.jpg)

* **Итоговый граф репозитория**

![rebase_master_8](resources/rebase_master_8.jpg)

* P.S.S. Во время rebase некорректно изменил файл rebase.sh при ребэйзе, поэтому не получил второго конфликта. Однако на итоговом результате это не сказалось.

![fuckup_1](resources/fuckup_1.jpg)