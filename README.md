
## Описание

Это приложение предназначено для мониторинга изменений в файловой системе и генерации отчетов. Основные функции:

- **Мониторинг папок**: Автоматическое отслеживание файлов `.rvt`, `.ifc`, и `.dwg` в заданной директории по параметру: совпадение по имени и дата изм. день в день.
  
- **Хранение данных**: Использование SQLite базы данных для сохранения информации о файлах, включая имя, путь, дату последнего изменения и автора.

- **Сравнение с предыдущими состояниями**: Возможность сравнивать текущее состояние файловой системы с данными из старой базы данных для обнаружения новых, измененных или удаленных файлов.

- **Генерация отчетов**: Создание визуальных отчетов в формате PDF и Excel, включающих информацию о выделенных файлах.

- **Пользовательский интерфейс**: Простой и интуитивно понятный интерфейс на базе Tkinter.

## Основные функции

1. **Подключение к базе данных**: Приложение может работать как с новой, так и с существующей базой данных для хранения информации о файлах.

2. **Сравнение файлов**: Алгоритм вычисления схожести имен файлов для группировки и выделения пар файлов со схожими названиями и датами изменений.

3. **Выделение файлов**: Автоматическая подсветка файлов в зависимости от их расширения и состояния (новые, измененные, отсутствующие).

4. **Поддержка отчетов**: Экспорт выделенных файлов в документы PDF и Excel с указаним иерархии папок и ссылками на файлы.

5. **Копирование пути**: Быстрое копирование пути к выбранному файлу в буфер обмена.

## Начало работы

1. **Скачайте** исполняемый файл [Search.IFCs.exe](https://github.com/AniCatPro/Search-IFCs/releases/download/main-dev/Search.IFCs.v1.5.exe). 
2. **Запустите программу** и выберите папку для мониторинга.
3. Укажите путь для сохранения новой базы данных.
4. Нажмите кнопку "Начать мониторинг".

При мониторинге:
- **Зеленым цветом** выделяются строки, соответствующие заданным параметрам (схожесть имени файла и совпадение даты изменения до дня).
- **Синим цветом** подсвечиваются строки для файлов `.rvt`.
- **Желтым цветом** подсвечиваются строки для файлов `.ifc`.

## Примечания

1. Чтобы скопировать путь до файла, выберите строку и нажмите кнопку "Скопировать путь".
2. Обратите внимание: функция сравнения пока не работает.
