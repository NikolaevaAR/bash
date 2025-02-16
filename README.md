# <img width="30" height="30" src="https://img.icons8.com/nolan/96/console.png" alt="console"/> Работа с bash


```bash
$ cd   Открыть домашнюю директорию через терминал
$ pwd  Определить имя папки, в которой вы находитесь
$ mkdir test1 Создать внутри этой папки каталог с именем test1
$ cd test1   Перейти в папку test1
$ pwd Проверка, что переход выполнен
$ touch 1.txt 2.txt 3.txt   Создать файл 1,2 и 3 внутри каталога test1
$ ls Проверить содержимое каталога test1
$ cd   Перейти в домашнюю директорию
$ mkdir test2   Создать папку test2 внутри домашней директории
$ rmdir test2   Удалить папку test2
$ rm test1/2.txt  Удалить файл 2 из папки test1
$ mkdir test3   Создание папки в домашней директории test3
$ touch test3/1.txt test3/2.txt     Создание файлов в папке test3
$ rm -r test3   Удалить папку test3
$ mkdir test4  Создать папку test4 в домашней директории
$ mv test1/1.txt test1/3.txt test4     Перемещение файлов 1 и 3 из папки test1 в папку test4
$ echo line > test4/1.txt     Добавить в файл 1 три строки со словами line
$ echo line >> test4/1.txt
$ echo line >> test4/1.txt
$ cat test4/1.txt  Посмотреть содержимое файла 1
$ cat test4/1.txt >> test4/3.txt   Добавьте в файл 3 три строки со словами line
$ cat test4/1.txt test4/3.txt    Просмотрите содержимое двух файлов (1 и 3) сразу
$ nano test4/1.txt   Используя один из редакторов замените все строки в файле 1
Search (to replace): line
Replace with: Hello
A

```

## Задание 25
Отправка базовых команд в bash
- [@Задача 1](https://github.com/NikolaevaAR/git_bash/blob/main/bash1.pdf)
- [@Задача 2](https://github.com/NikolaevaAR/git_bash/blob/main/bash2.pdf)
