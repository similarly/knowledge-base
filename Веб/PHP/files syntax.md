**Что такое стрим:**
	https://stackify.com/a-guide-to-streams-in-php-in-depth-tutorial-with-examples/

Возвращает массив с файлами и директориями в заданной директории (`__DIR__` - текущая)
	`scandir (__DIR__);`

Проверка
	`is_dir()`
	`file_exists()`
	`file`
	`filesize()` кэшируется, cleatstatcache()

Редактирование файлов
	`file_put_contents(file, contents, FILE_APPEND)`
	`unlink(file)` удаление
	`copy(file, file)`
	`rename(file, file)`
	`pathinfo() `возвращает массив с информацией 

Редактирование директорий 
	`mkdir()` recursive: true для foo/bar вложенности
	`rmdir()`

Чтение файла
	`fopen(file, mode)` mode r/w/rw, возвращает resource 
	`fgets(file)` можно прочитать по строкам через while false 
	`fclose(file)`
	`fgetscsv(file)` парсит строку и возвращает массив с полями
	`file_gets_contents(file, offset = a, length = b)` (лучше юзать curl)