Программа получает данные о компаниях и вакансиях с сайта hh.ru, создает базу данных и таблицы в PostgreSQL и загружает полученные данные в созданные таблицы.

Компании, вакансии которых программа будет загружать:

*Тинькофф
*Газпром нефть
*Яндекс
*СБЕР
*Российские железные дороги
*Аэрофлот
*Альфа-Банк
*VK
*Норникель
*Ланит

Структура репозитория:

main.py - файл для запуска программы
classes - директория классов: hh.py - класс для работы с сайтом hh.ru db_manager.py - класс для работы с базой данных
utils - директория функций: utils.py - функции для работы программы config.py - функция для получения словаря с данными для подключения к базе данных
tests - директория тестов
data - директория файлов для работы с программой
requirements.txt - список необходимых пакетов для работы с программой
Перед началом работы программы необходимо:

установить виртуальное окружение
установить пакеты из файла requirements.txt
создать конфигурационный файл database.ini для подключения к базе данных Шаблон для создания конфигурации: [postgresql] host=localhost user=postgres password=12345(логин и пароль вводим свои-от базы постгрес) port=5432
Описание работы программы:

Программа собирает данные по 10 вакансиям
Создает базу данных и таблицы
Записывает полученные данные в созданные таблицы
Выводит меню для пользователя
