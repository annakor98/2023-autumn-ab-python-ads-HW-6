# 2023-autumn-ab-python-ads-HW-6
## Общее описание
Дополнить HW5 работой с базой данных, тестированием методов API и настроить автоматический запуск линтеров и тестов при push в репозиторий.

## API endpoints
| endpoint | Обновить существующий endpoint | Создать новый endpoint | Тип запроса | Действие | Подсказка |
| --- | :---: | :---: | --- | --- | --- |
| /predict/{baseline} | :heavy_check_mark: | | POST | Возвращает предсказание класса (fraud/clean) для заданного входного текста **и записывает входной текст, предсказание, используемый бейзлайн и время выполнения в базу ``messages.db``** | |
| /get_latest_entry/{baseline} | | :heavy_check_mark: | GET | Возвращает крайнюю запись в БД ``messages.db`` для бейзлайна ``baseline``| |
| /get_number_of_entries | | ✔️ | GET | Возвращает количество записей в БД ``messages.db`` для каждого бейзлайна, например: ``{"constant-fraud": 1, "constant-clean": 2, "first-hypothesis": 3}`` | |
