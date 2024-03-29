# Подсказки по командной строке 

Команда смены директории:
```sh
cd c:\folder_name
```
Вызов функции "Git help"
```sh
git
```
Инициализация пустого репозитория
```sh
git init
```

Листинг текущей директории. Отображение того, что файл лежит в текущей директории

для Windows:
```sh
dir
```
для MacOS, Linux: 
```sh
ls
```
Добавление имя и почты того кто работает в репозитории, где --global добавляет во все репозитории, а --local в локальный. 
```sh
git config --global user.name
git config --global user.email
```
Проверка имени и почты. 
```sh
git config user.name
git config user.email
```

Удаление файла с репозитория

для Windows:
```sh 
del имя_файла
```
для MacOS, Linux: 
```sh
rm имя_файла
```

Отображает статус текущего репозитория. Показывает какие файлы отслеживаються, а какие не отслеживаються.
```sh
git status
```
Клонирование репозитория к себе.
```sh
git clone ссылка_на_репозиторий
```

Отправляет в интернет в репозиторий на GitHub все изменния.
```sh
git push
```

Стянуть из основного репозитория все изменния в свой локальный репозиторий.
```sh
git pull
```

Добавляет файл(ы) к отслеживанию.
```sh
git add имя_файла
```

Делает коммит.
```sh
git commit -m "Пишем сообщение"
```

Удаление файла с репозитория.
```sh
del имя_файла
```

Логи действий. Для выхода с логов нужно нажать "Q".
```sh
git log
git log --oneline  - логи действий в одну строчку
git log --graph - визуализация комитов, веток
```

Переход в определенный комит.
```sh
git checkout идентификатор_комита
```

Переход в самое последнее состояние. В главную ветку master.
```sh
git checkout master
```

Переход в другую ветку.
```sh
git checkout имя_ветки
```

Создает новую ветку.
```sh
git branch название_новой_ветки
```

Выводит список веток которые есть.
```sh
git branch
```

Удаляет ветку.
```sh
git branch -d название_ветки
```

Сбрасывает изменения. Делается до команды commit.
```sh
git restore имя_файла
```

Показывает отличие чего либо.
```sh
git diff
```

Вытирает с поля ввода в терминале ранее написанные команды. Очищает терминал. Изменения не тиряються.
```sh
clear
```

Слияние веток. Пишем ветку которую нужно добавить в основную ветку master. 
```sh
git merge название_ветки
```
Как скопировать репозиторий и отправлять в него изменения. Репозиторий находится в интернете.
1. Создаем аккаунт github.com 
2. Создаем локальный репозиторий
3. "Подружить" локальный и удаленный репозиторий. github при создании нового репозитория подскажет как это сделать.
4. Сделать "git add ..." и "git commit ..." Потом отправляем "git push" ваш локальный репозиторий в удаленный репозиторий на github. При этом, возможно, нужно будет авторизироваться на удаленом репозитории.
5. Произвести изменения можно и с другого компьютера и закачать их в удаленный репозиторий на github.
6. Чтобы получить актуальную версию с удаленного репозитория пишем у себя в терминале комнду git pull.

Как сделать fork репозитория.

1. Делаем clone СВОЕЙ версии репозитория
2. Создаем новую ветку и в НЕЕ вносим свои изменения
3. Фиксируем изменения (делаем коммиты)
4. Отправляем свою версию в свой GitHub
5. На сайте GitHub нажимаем кнопку pull request 
