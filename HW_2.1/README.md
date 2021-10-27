#2.1. Системы контроля версий, Кузьмин Илья (поток 2)

##Задание 1

###**1. Настройка репозитория (первый коммит)**

**п. 1 - 5** 

![p1_5](resources/p1_5.png)

**п. 6 - 8**

![p6_8](resources/p6.jpg)

**п. 9**

![p9](resources/p9.jpg)

![p9](resources/p9.1.jpg)

**п. 10**

![p10](resources/p10.jpg)

**п. 12**

![p12](resources/p12.jpg)

###**2. gitignore (второй коммит)**

**п. 1**

![p2_1](resources/gitignore_1.jpg)

**п. 2**

![p2_2](resources/gitignore_2.jpg)

**п. 4**

Описание игнорируемых файлов в данном каталоге:
 * \*\*/.terraform/\* - игнорируются все файлы в директории .terraform не включая подкаталоги, 
Сама .terraform может находиться по любому пути, начиная с /terraform, т.к. gitignore находится в ней.
 * *.tfstate - все файлы с расширением .tfstate
 * \*.tfstate.\* - все файлы, содержащие подстроку .tfstate. в имени
 * crash.log - файл с указанным именем
 * *.tfvars - все файлы с расширением .tfvars
 * override.tf - файл с данным именем
 * override.tf.json - файл с данным именем
 * *_override.tf - все файлы, которые оканчиваются на _override.tf
 * *_override.tf.json - все файлы, которые оканчиваются на _override.tf.json
 * .terraformrc - файл с данным именем
 * terraform.rc - файл с данным именем

**п. 5**

![p2_3](resources/gitignore_3.jpg)

### **3. Удаление и перемещение файлов (третий и четвертый коммиты)**

**п. 1,2**

![p1_2](resources/movedelete_1.jpg)

**п. 3 - 5**

![p3_5](resources/movedelete_2.jpg)


### **4. Проверка изменений**

![pChch](resources/checkchanged.jpg)

##Задание 2

**Вывод git --help**

![githelp](resources/githelp.jpg)

  