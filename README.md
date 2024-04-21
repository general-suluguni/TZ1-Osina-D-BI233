# ТЕХНИЧЕСКОЕ ЗАДАНИЕ №1: СКРИПТ ДЛЯ КОПИРОВАНИЯ ФАЙЛОВ
# Принцип работы
На вход программе подается два параметра: входная директория, из которой предстоит скопировать файлы, и выходная директория, в которую следует перенести копии файлов. Пример запуска скрипта:
```
sh tz1.sh С:/inp_dir C:/outp_dir
```
где С:/inp_dir - расположение входной директории, C:/outp_dir - расположение выходной директории.

Программа проходит по всем файлам во входной директории и всех ее поддиректорий и копирует их в выходную директорию. При переносе файлов их иерархия не сохраняется. В случае, если на момент копирования очередного файла в выходной директории уже существует файл с таким же названием, к названию текущего файла перед расширением добавляется _1, при повторном возникновении подобной ситуации - _2 и так далее. 
Если програма успешнно отработает, она выведет сообщение:
```
Все файлы из *входной_директории* скопированы в *выходную_директорию*
```
Имейте в виду, что адреса директорий необходимо вводить корректно. Если программе не удастся найти хотя бы одну из указанных директорий, она завершится с ошибкой и выведет сообщение:
```
Некорректные входные данные! Не существует директории: *некорректное_название*
```
Если Вы не передадите скрипту два аргумента, он завершится с ошибкой и выведет сообщение:
```
Некорректные входные данные! Пожалуйста, введите два аргумента.
```

# Пример входных данных
Хуй знает где пока в этом репозитории находятся тестовые данные: входная директория inp_dir и выходная директория outp_dir. Вы можете протестировать работу скрипта, загрузив данные папки с файлами и запустив программу на них.
Изначально, структура inp_dir является следующей:
КАРТИНКА
В outp_dir хранится только один файл:
КАРТИНКА
После запуска скрипта с входными данными: 
```
sh tz1.sh С:/inp_dir C:/outp_dir
```
