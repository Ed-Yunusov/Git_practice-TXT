#### Git_practice-TXT
1. Создать внешний репозиторий c названием Git_practice-TXT
    + открыть `https://github.com`. Залогиниться. Нажать кнопку `New`. 
    + в поле Repository name ввести Git_practice-TXT, выбрать Public и Add a README file. 
    + Нажать `Create repository`.

2. Клонировать репозиторий Git_practice-TXT на локальный компьютер
    + Нажать `Code`, выбрать HTTPS, скопировать ссылку на репозиторий 
    + `git clone https://github.com/Ed-Yunusov/Git_practice-TXT.git`
    + в терминале перейти в папку Git_practice-TXT(`cd Git_practice-TXT`), в конце адреса расположения отображается main

3. Внутри локального Git_practice-TXT создать файл “new.txt”
    + `touch new.txt`
    + `git status` - new.txt отображается красным (изменения в файле не отслеживаются)

4. Добавить файл под гит
    + `git add new.txt`
    + `git status` - new.txt отображается зеленым (изменения в файле отслеживаются)

5. Закоммитить файл
    + `git commit -m "new file"` - создает снимок текущего состояния файла с комментарием "new file"

6. Отправить файл на внешний GitHub репозиторий
    + `git push`

7. Отредактировать содержимое файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT
    + `vim new.txt` 
    + `insert`
        + Full name: Yunusov Eduard Alexeevich
        + Age: 33
        + Number of pets: 1
        + Future desired salary: 2000$

    + `Esc`
    + `:wq`

8. Отправить изменения на внешний репозиторий
    + `git commit -am "added info" && git push` - "&&" -вторая команда автоматически запускается после завершения первой команды

9. Создать файл preferences.txt
    + `touch preferences.txt`

10. В файл preferences.txt добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить). Всё написать в формате TXT
    + `vim new.txt` 
    + `insert`
        + Favorite movie: Lord of the Rings
        + Favorite serial: Friends
        + Favorite food: Pizza
        + Favorite time of the year: Spring and summer
        + Country I would like to visit: The Kingdom of Thailand

    + `Esc`
    + `:wq`

11. Создать файл skills.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT
    + `vim new.txt` 
    + `insert`
    + skills:
        + Software testing theory
        + Client-server architecture
        + HTTP Server Request Methods
        + HTTP server Response codes
        + Structures of HTTP requests and responses
        + What is JSON, XML. Their structure
        + API testing via Postman JS, API autotests
        + Removing and reading logs from an external server
        + Sniffing http web traffic through Charles and Fiddler
        + Dev Tools of web browsers Google Chrome, FireFox
        + VPN. How it works, why you need it, how to use it, tool options
        + Mobile testing
        + Feature of iOS, Android, guidelines
        + Build iOS applications on Xcode
        + Build Android applications on Android Studio
        + ADB management of android devices
        + Setting up proxy and vpn on iOS and Android
        + Interception (sniffing) of mobile traffic through Charles and Fiddler on iOS and Android
        + Command line (terminal) Linux copy, create, view, move files on servers without a graphical interface
        + Basics of bash scripting, automation of routine tasks on the server
        + Access to remote servers
        + Basics of SQL Create, Delete, Drop, Insert Into, Select, From, Where, Join
        + Postgres database installation, configuration and use
        + Non-relational database Redis installation, configuration and use
        + Load testing in Jmeter
        + Scrum development methodology

    + `Esc`
    + `:wq`

12. Отправить сразу 2 файла на внешний репозиторий
    + `git add . ; git commit -m "adding two files to the rep" ; git push`

13. На веб интерфейсе создать файл bug_report.txt
    + Войти в репозиторий Git_practice-TXT. Нажать кнопку `Add file`.
    + Выбрать `Create new file`. В поле Name your file ввести bug_report.txt.

14. Сделать Commit changes (сохранить) изменения на веб интерфейсе
    + Нажать кнопку `Commit new file`.

15. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT
    + Открыть файл bug_report.txt, нажать на кнопку `Edit this file`.
    	+ ID: 1
    	+ Title: В разделе 'Помощь' не работает ссылка
    	+ Project: Сайт интернет-магазина HitechPlace
    	+ STR:
    	+ 1.Открыть главную страницу (ссылка_на_сайт)
    	+ 2.Нажать на кнопку 'Помощь' в верхнем меню
    	+ 3.Нажать на кнопку 'Где можно получить больше информации?'
    	+ 4.Нажать на кнопку 'тут'
    	+ Actual result: Возникает ошибка 'OOPS! THAT PAGE CAN'T BE FOUND'
    	+ Expected result: Появляется страница с необходимой информацией
    	+ Severity: Major
    	+ Priority: High
    	+ Status: Open
    	+ Attachments: ссылка_на_картинку_с_багом
    	+ Author: Эдуард Юнусов

16. Сделать Commit changes (сохранить) изменения на веб интерфейсе
    + Нажать кнопку `Commit changes`.

17. Синхронизировать внешний и локальный репозиторий Git_practice-TXT
    + `git pull`
