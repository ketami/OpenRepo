# Документация по работе с проектом

## Общее описание
Проект реализует инвертированный индекс с поддержкой сжатия гамма-кодированием Элиаса для поиска по текстовым данным.
Выводит размер индекса со сжатием и без сжатия, время поиска со сжатием и без сжатия.


## Установка и требования
Для работы парсера требуются зависимости, указанные в файле requirements.txt.
Также необходим файл .npy, содержащий numpy-массив из словарей. 
В каждом элементе массива должен быть ключ text, по элементам которого производится поиск.

## Использование
Для создания индекса: 
python create_index.py --data /path/to/.npy --output /path/to/.pkl

Для поиска по индексу (в качестве примера запроса "ректор"):
python search_index.py "ректор" --index /path/to/.pkl