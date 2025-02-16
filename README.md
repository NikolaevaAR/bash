# <img width="30" height="30" src="https://img.icons8.com/nolan/96/console.png" alt="console"/> Работа с Bash

В процессе обучения я работала с базовыми командами bash: создание и удаление директорий и файлов, перемещение, копирование и редактирование файлов, работа с процессами и API-запросами.

Ниже Вы можете ознакомиться с командами, которые я выполняла в процессе обучения.

## Базовые команды с файлами и директориями в Bash
```bash
$ cd                                             # Открыть домашнюю директорию через терминал
$ pwd                                            # Определить имя папки, в которой вы находитесь
$ mkdir test1                                    # Создать внутри этой папки каталог с именем test1
$ cd test1                                       # Перейти в папку test1
$ touch 1.txt 2.txt 3.txt                        # Создать файл 1,2 и 3 внутри каталога test1
$ ls                                             # Проверить содержимое каталога test1
$ cd                                             # Перейти в домашнюю директорию
$ mkdir test2                                    # Создать папку test2 внутри домашней директории
$ rmdir test2                                    # Удалить папку test2
$ rm test1/2.txt                                 # Удалить файл 2 из папки test1
$ mkdir test3                                    # Создание папки в домашней директории test3
$ touch test3/1.txt test3/2.txt                  # Создание файлов в папке test3
$ rm -r test3                                    # Удалить папку test3
$ mkdir test4                                    # Создать папку test4 в домашней директории
$ mv test1/1.txt test1/3.txt test4               # Перемещение файлов 1 и 3 из папки test1 в папку test4
$ echo line > test4/1.txt                        # Добавить в файл 1 три строки со словами line
$ echo line >> test4/1.txt
$ echo line >> test4/1.txt
$ cat test4/1.txt                                # Посмотреть содержимое файла 1
$ cat test4/1.txt >> test4/3.txt                 # Добавьте в файл 3 три строки со словами line
$ cat test4/1.txt test4/3.txt                    # Просмотрите содержимое двух файлов (1 и 3) сразу
$ nano test4/1.txt                               # Используя один из редакторов замените все строки в файле 1
    Search (to replace): line
    Replace with: Hello
    A (ALL)
$ cd                                             # Перейти в домашнюю директорию.
$ mkdir test3                                    # Создать папку test 3
$ touch test3/4.txt test3/5.txt test3/6.txt      # Добавить в папку test 3 три файла 4, 5 и 6, в каждом из которых должно быть по 4 строки row1, row2, row3, row4
$ echo row1 > test3/4.txt
$ echo row2 >> test3/4.txt
$ echo row3 >> test3/4.txt
$ echo row4 >> test3/4.txt
$ cat test3/4.txt >> test3/5.txt
$ cat test3/4.txt >> test3/6.txt
$ grep "row2" test3/5.txt                        # Найдите строку row2 в файле 5
$ grep -r "row" test3                            # Найдите строку row в папке test3
$ grep -c "row" test3/6.txt                      # Посчитайте сколько строк с содержимым row в файле 6
$ find -name "5.txt"                             # Найдите файл 5 внутри папки test3
$ find  -name "5.txt" -delete                    # Используя команду find, удалите файл 5
$ echo test > 4.txt                              # Используя команду echo, добавьте слово test в файл 4
$ nano 4.txt                                     # Замените слово test в файле 4 на fail
    Search (to replace): test
    Replace with: fail
    A(ALL)
$ echo test >> 4.txt                             # Добавьте в файл 4 слово test так, чтобы сохранилось содержимое

```


## Базовые команды с процессами и API-запросами в Bash

```bash

$ ps aux                                         # Просмотрите все процессы для юзеров не только в консоли, которые происходят в системе
$ kill 666                                       # Убейте процесс 666 в консоли (можно не убивать, а просто написать команду)
$ ping rusau.net                                 # Узнайте доступность ресурса rusau.net, используя ping
$ ping -c 5 rusau.net                            # Отправьте 5 пакетов на сайт rusau.net
$ curl -X GET                                    # Используя GET и команду curl, получите информацию о зарегистрированных питомцах с любым статусом на https://petstore.swagger.io/
    https://petstore.swagger.io/v2/pet/findByStatus?status=pending                       
$ curl -X POST                                   # Используя POST и команду curl, создайте нового пользователя на https://petstore.swagger.io/
    https://petstore.swagger.io/v2/user    
      -H "Content-Type: application/json" -d          
          '{"username": "fhgdsh",
            "email": "rfgt@mail.ru",
            "password": "fhgdffhfsghsg"}'
```
