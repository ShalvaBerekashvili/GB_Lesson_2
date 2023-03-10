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

git merge **name_commit**



## Удаление веток

## Визуализация репазитория

Для вывода визуализации в GIT необходимо использовать следующую команду:

>git log -graph

но лично мне нравиться на данный момент:

>git log --pretty=oneline

Но сегодня на семинаре нам расказали про такой вариант вывода:

>git log --all --graph --oneline --decorate

И еще один любопытный метод

>git log --pretty=format:"%h - %an, %ar : %s"


>## Списки

Чтобы добавит ненумерованые списки, необходимо пукты выделить звездочкой (*) или знаком +.
Напрмер, вот так:

* Элимент 1
* Элимент 2
* Элимент 3
+ Элимент 4

Чтобы довать нумерованые списки, необходимо пронумеровать пункты.
Напрмер, вот так:

1. Первый пункт
2. Второй пунктпше

## Команда **clone**

Очень полезная команда, она необходима для полного копированиея удаленной директоии в локальную!

выглять очень так:

git clone __"тут_праямая_ссылка_на_удаленную_директорию"__

*Прмер: git clone https://github.com/ShalvaBerekashvili/GB_Lesson_2.git*

для успешного проведения данной манипуляции, необходимо провести подготтовительные действия:

- Создать новую папку, в котрой будем работать с новыми фалами.
- убедится что находитшся в рабочей паке, перед чем вносить какие либо изменния, НУЖНО БЫТЬ очкнь аккуратным в работе с GIT.


## Работа с удаленным репазиторием

+ Необходимо быть авторизованным на GitHab (как пример)
+ Необходимо создать удаленный репазиторий
+ При создании следовать подсказкам, согласно той задачи которая стоит.

Для того чтобы GIT понял с каким удаленным репазиторием он работает необходим применить слкдующую команду:

> git remote add origin https://github.com/ShalvaBerekashvili/GB_Lesson_2.git

Далее определяем главную ветку, командой:

> git brach -M main

Для отправки уже изменненой версии, на удаленный репазиторий главную ветку:

> git push -u origin main

Тут важно указать слдедующий момент, необходимо быть авторизованным, без этого не выйдет.

Также есть команда *pull* - какбы стягивает, при помощт нее можно подтянуть новое состояние файла с удаленного репазитория, но есть нюанс, при поддягивании она делает merge всех веток из удаленного репазитория, с локальным репазиторием! Выглядит она следующим образом:

> git pull 

Это нам позволит выкачать актуальную версию с удаленного репазитория.

