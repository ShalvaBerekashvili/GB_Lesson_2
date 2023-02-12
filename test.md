# _Инструкция_ __по__ ___настройке GIT___

[Markdown syntax](https://www.markdownguide.org/basic-syntax/) 

## git init 

>Команда *git init* создает git репазиторий в текущей папку

## git config --global user.name - "имя пользователя"

>Команда *git config --global user.name - <font color="yellow">"имя пользователя" </font>* позволяеет аутентифицировать пользователя.

## git config --global user.mail - "email"

>Команда git config --global user.mail - <font color="green"> "имя пользователя" </font>  позволяеет добавть email пользователя.

## git add -"fale_name"

>Команда git add -"fale_name" позволяеет добавить файл в список отслеживаемых (индексирируемых) файлов.


## git checkout "первые четыре символа хеша"

>Команда git checkout "первые четыре символа хеша" позволяеет перемещаться между комитами.

## <font color="green"> git log --pretty=oneline </font>

>Команда "git log --pretty=oneline" позволяеет вывести в одну строку хеш_файла + меседж к нему

![](/git_log.png)

## git show "хеш_файла"

>Команда *git show "хеш_файла"* позволяет посмотреть содежимое измененного файла

![](/git_show.png)


Berekashvili Shalva

sbit_menedger@mail.ru

## ветки GIT

Для создания веток в GIT необходимо из рабочей директории исполизовать следующую кострукцию:

git branch **name_barnch**

Для созздани ветки и перход в нее:

git checkout -b **name_barnch**


## создание ветки

Для того, чтобы созlать ветку  необходимо использовать команду:

*git branch имя_ветки*

Для того, чтобы созлать ветку и преключиться необходимо использовать команду:

> *git checkout -b имя_ветки*

## слияние веток 

Для слияния веток в GIT необходимо из нужной ветки 
слить ту которую необходимо обьяденить, необходимо использовать следеющую команду:

git marge **name_commit**



## Удаление веток

Для удаления ветки в GIT необходимо быть в главной ветки, и использовать следующию команду:

git branch -d **name_commit**


## Визуализация репазитория