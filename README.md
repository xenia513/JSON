# JSON

## Homework to the first GIT lesson JSON part - Vadim Ksendzov's course

### 1. Создать внешний репозиторий c названием JSON

    Repositories >> New >> JSON >> Create repository 

### 2. Клонировать репозиторий JSON на локальный компьютер

    JSON >> Code >> Copy HTTPS

    $ git clone https://github.com/xenia513/JSON.git

### 3. Внутри локального JSON создать файл “new.json”

    $ touch new.json

### 4. Добавить файл под гит

    $ git add new.json

### 5. Закоммитить файл

    $ git commit -m "created new.json"

### 6. Отправить файл на внешний GitHub репозиторий

    $ git push

### 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON

    $ vim new.json

Эта команда открывает встроенный редактор текста, для начала редактирования необходимо нажать `i` и ввести текст:
    
    {
    	"name": "Kseniia_Kiseleva",
    	"age": 30,
    	"petsCount": 1,
    	"salary": 80000
    }

После завершения редактирования нажимаем `Esc` и `:wq` для сохранения внесенных изменений и выхода из режима редактора.

### 8. Отправить изменения на внешний репозиторий

    $ git commit -a -m "added text"

### 9. Создать файл preferences.json

    $ cat > preferences.json
    
После ввода этой команды открывается поле ввода текста для записи в файл, поэтому мы сразу же приступаем к выполнению следующего задания.

### 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, стрaна, которую хотели бы посетить) в формате JSON

    {
    	"favouriteMovie": "Inception",
    	"favouriteSeries": "YouAreTheWorst",
    	"favouriteFood": "Curry",
    	"favouriteSeason": "Summer",
    	"tripDestination": "SriLanka"
    }

Для завершения редактирования нажимаем `Enter` и `Ctrl+C`

### 11. Создать файл skills.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON

    $ cat > skills.json

    {"skills": ["bash","postman","GIT","clientServerArchitecture","devTools","charlesProxy","fiddler","andriodStudio"]}

### 12. Сделать коммит в одну строку

    $ git add . && git commit -m "added preferences.json and skills.json"

### 13. Отправить сразу 2 файла на внешний репозиторий

    $ git push

### 14. На веб-интерфейсе создать файл bugReport.json

    JSON >> Add file >> Create new file >> bugReport.json

### 15. Сделать Commit changes (сохранить) изменения на веб-интерфейсе

    Commit new file 

### 16. На веб-интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON

    JSON >> bugReport.json >> Edit this file

Кнопка редактирования файла выглядит так:

![Edit this file button](https://docs.github.com/assets/cb-47677/mw-1440/images/help/repository/edit-file-edit-button.webp)

Вводим текст: 

    {
     "ID": "0001",
     "Severity":"Trivial",
     "Enviroment":"Win 7 Chrome 109 IPhone 11 IOS 16.4.1",
     "Title": "The link [Share price] redirects to the english page from Trading Course 1, section 2 when AR, NL, VI, TH or ZN is chosen",
     "Precondition": "",
     "Steps": {
       "1": "Navigate to capital.com",
       "2": "Hover over the [Education] menu section",
       "3": "Click the [Trading сourses] menu item",
       "4": "Click the [Who are the main market players?] row in the Introduction to Financial Markets box",
       "5": "Select AR, NL, VI, TH or ZN language",
       "6": "Scroll to the second to the last paragraph",
       "7": "Click the link [Share price]"
     },
     "Postcondition": "",
     "ExpectedResult":"The link [Share price] redirects to the page translated into chosen language",
     "ActualResult":"The link [Share price] redirects to the english page",
     "Attachment": "link"
     "Author": "@xenia513"
    }

### 17. Сделать Commit changes (сохранить) изменения на веб-интерфейсе

    Commit changes

### 18. Синхронизировать внешний и локальный репозиторий JSON

    $ git pull
