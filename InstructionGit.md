# Настройка Git-а и основные команды.

* git version - узнаем установлен ли Git и какая версия его.

* git config --global.name "  " - задать/ изменить имя пользователя.

* git config -- user/email "  " - задать/изменить email пользователя.
 
* git init - создание репозитория текущей папке.
![git init comand](GitInit.jpg)

* git add . - добавление всех файлов в папке.

* git add ./NameOfFile - добавление файла  с именем NemeOfFile (достаточно написать 4 первые буквы имени файла и нажать клавишу "Tab").
![git add comand](GitAdd.jpg)

* git commit -m 'Заметка' - сохранение измененний.
![git commit comand](GitCommit.jpg)

* git status - Показывает текущее состояние Git -а, есть ли изменения, которые нужно закоммитить (сохранить).

* git log - просмотр истории Commit -ов (сохранений).
![git log comand](GitLog.jpg)
> Нажатие клавиши ‘q’ на английской рвскладке клавиатуры - возвращает в исходное окно терминала.

* git checkout - переключение между commit -ами (сохранениями).
> для этого нужно запомнить номер (первые 4 символа) интересующего нас commit -а и записать команду так:
![git checkout commit comand](GitCheckoutCommit.jpg)

* git diff - список изменений, внесенных в респозиторий.
![git diff comand](GitDiff.jpg)

## Создание веток (Branch) и переключение между ними.  

* git branch - при выполнении этой строки мы получим список существующих веток, где символом * будет отмечена ветка, где вы сейчас находитесь.
![git branch comand](GitBranch.jpg)

* git branch NameOfNewBranch - добавление новой ветки NameOfNewBranch.
![git branch comand](GitBranchNB.jpg)

* git checkout NameOfBranch - преход на другую ветку NameOfBranch.
![git checkout comand](GitCheckout.jpg)

        > git checkout branch NameOfBranch - одновременное создание и преход на ветку NameOfBranch.

* git merge NameOfBranch - при выполнениее этой команды проиходит слияние или перенос изменений с одной ветки на другую.
![git merge comand](GitMerge.jpg)

* git branch -d NameOfBranch - удаление ветки NameOfBranch.Для корректного удаления нужно помнить несколько правил, чтобы не получить ошибки:
    1. Нельзя удалить ветку, в которой вы находитесь. Git выкинет ошибку и не произведет удаление. Следовательно, нужно перейти на другую ветку.
    2. Git не позволит удалить ветку, у которой есть несохраненные изменения. Так мы избегаем ситуации, когда часть написанного кода будет безвозвратно утеряна.
![git branch -d](Git-d.jpg)

* git branch -D NameOfBranch - удаление ветки, несмотря на на условие 2. предидущего пункта.

* в новой ветке, для создания сохранения, необходимо последовательно выполнить следующие команды (git add и git commit).

*git log --graph - позволяет отобразить коммиты в виде дерева.
![git log --graph comand](GitLogGraph.jpg)

Чтобы очистить терминал - нужно ввести **clear** в строке терминала.
![clear comand](Clear.jpg)
 
 ### Тренажер по веткам Git: 
 [Learn Git Branching](https://learngitbranching.js.org/?locale=ru_RU)

# Основная литература по Git:
 [Git для профессионального програмиста (С.Чакон и Б. Штрауб)](https://gbcdn.mrgcdn.ru/uploads/asset/4245110/attachment/d4eb8c232f8f2bdf4e42ba7cb49e0c50.pdf) 

