# Lesson5
Functions: file handling, strings, arrays, datetime, images, etc

##Homework:

Написать скрипт, который:

1. Создает переменную - многомерный массив с элементами - сообщения. Пример:
```php
$messages = array(
  0 => array(
    'sender' => 'max'
    'email' => 'max@xx.xx'
    'message' => 'text text text text text'
  )
  1 => ...
);
```
2. Делает сериализацию данных функцией serialize и записывает их в файл "database/database.txt" с помощью функций работы с файлами (http://php.net/manual/ru/book.filesystem.php)

3. Делат извлеченние данных из файла и конвертирует их назад в массив через unserialize.

4. Выводит массив данных в формате HTML на страницу (в любом оформлении).

5. Представление данных и логика работы скрипта должны быть разделены на отдельные файлы.

Дополнение 1:
1. Текст сообщений должен очищаться перед записью в файл: 
1.1. Все HTML переносы строк <br/> должны быть заменены на переносы в вашей системе. Например, "\r\n" в windows или использовать системную константу PHP_EOL - http://php.net/manual/ru/reserved.constants.php#constant.php-eol 
1.2. Должны быть удалены все HTML теги и пробелы в начале и конце строки. Функции: trim(), striptags().
1.3. Текст должен начинаться с заглавной буквы.
2. В тексте, который считываеться с файла, произвести обратную замену разделителей системы, например, "\r\n", на теги <br/>
3. Логично разделить код на функции.

 

