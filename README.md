# <img width="30" height="30" src="https://img.icons8.com/nolan/96/console.png" alt="console"/> Работа с Bash

В процессе обучения я работала с базовыми командами Bash, включая создание и удаление директорий и файлов, перемещение, копирование и редактирование файлов, а также взаимодействие с процессами и API-запросами..

## Базовые команды с файлами и директориями в Bash
```bash
$ cd                                             # Переход в домашнюю директорию
$ pwd                                            # Определение текущей директории
$ mkdir test1                                    # Создание каталога test1
$ cd test1                                       # Переход в каталог test1
$ touch 1.txt 2.txt 3.txt                        # Создание файлов 1.txt, 2.txt, 3.txt
$ ls                                             # Просмотр содержимого каталога test1
$ cd                                             # Возвращение в домашнюю директорию
$ mkdir test2                                    # Создание каталога test2
$ rmdir test2                                    # Удаление каталога test2
$ rm test1/2.txt                                 # Удаление файла 2.txt из каталога test1
$ mkdir test3                                    # Создание каталога test3
$ touch test3/1.txt test3/2.txt                  # Создание файлов 1.txt и 2.txt в каталоге test3
$ rm -r test3                                    # Удаление каталога test3
$ mkdir test4                                    # Создание каталога test4
$ mv test1/1.txt test1/3.txt test4               # Перемещение файлов 1.txt и 3.txt в каталог test4
$ echo line > test4/1.txt                        # Добавление в файл 1.txt  трех строк со словами line
$ echo line >> test4/1.txt
$ echo line >> test4/1.txt
$ cat test4/1.txt                                # Просмотр содержимого файла 1.txt
$ cat test4/1.txt >> test4/3.txt                 # Добавление содержимого файла 1.txt в 3.txt
$ cat test4/1.txt test4/3.txt                    # Просмотр содержимого файлов 1.txt и 3.txt
$ nano test4/1.txt                               # Редактирование файла с помощью редактора nano
    Search (to replace): line
    Replace with: Hello
    A (ALL)
$ cd                                             # Переход в домашнюю директорию.
$ mkdir test3                                    # Создание каталога test3
$ touch test3/4.txt test3/5.txt test3/6.txt      # Создание файлов 4.txt, 5.txt и 6.txt в каталоге test3 со следующим содержимым "row1, row2, row3, row4"
$ echo row1 > test3/4.txt
$ echo row2 >> test3/4.txt
$ echo row3 >> test3/4.txt
$ echo row4 >> test3/4.txt
$ cat test3/4.txt >> test3/5.txt
$ cat test3/4.txt >> test3/6.txt
$ grep "row2" test3/5.txt                        # Обнаружение строки row2 в файле 5.txt
$ grep -r "row" test3                            # Обнаружение строк, содержащих "row", в каталоге test3
$ grep -c "row" test3/6.txt                      # Подсчет количества строк с "row" в test3/6.txt
$ find -name "5.txt"                             # Обнаружение файла 5.txt в каталоге test3
$ find  -name "5.txt" -delete                    # Удаление файла 5.txt с помощью find
$ echo test > 4.txt                              # Добавление "test" в файл 4.txt
$ nano 4.txt                                     # Замена "test" на "fail" в файле 4.txt
    Search (to replace): test
    Replace with: fail
    A(ALL)
$ echo test >> 4.txt                             # Добавление "test" в файл 4.txt без потери содержимого

```


## Базовые команды с процессами и API-запросами в Bash

```bash

$ ps aux                                         # Просмотр всех процессов в системе
$ kill 666                                       # Завершение процесса с PID 666
$ ping rusau.net                                 # Проверка доступности ресурса rusau.net
$ ping -c 5 rusau.net                            # Отправка 5 пакетов на сайт rusau.net
$ curl -X GET                                    # Использование GET для получения данных с API Petstore
    https://petstore.swagger.io/v2/pet/findByStatus?status=pending                       
$ curl -X POST                                   # Использование POST для создания нового пользователя
    https://petstore.swagger.io/v2/user    
      -H "Content-Type: application/json" -d          
          '{"username": "fhgdsh",
            "email": "rfgt@mail.ru",
            "password": "fhgdffhfsghsg"}'
```
