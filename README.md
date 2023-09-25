# Перечень автоматизируемых сценариев
## Предусловия к сценариям тестирования:
1. Навигация с главной страницы на страницу формы заявки на курс "Тестировщик" через каталог курсов раздел "Программирование" с проверкой фильтрации по курсам
   ![Курсы программирования онлайн – обучение с нуля - Нетология 2023-09-25 13-48-56](https://github.com/Dimonstratos/HW4.2/assets/130654761/7fc22b26-6a70-482e-8d9a-a0fcd8f009b4)
   ![Курсы программирования онлайн – обучение с нуля - Нетология 2023-09-25 13-32-00](https://github.com/Dimonstratos/HW4.2/assets/130654761/c95c3365-6035-4d47-99cb-cc1914c3a9de)
1. Навигация с главной страницы на страницу формы заявки на курс "Тестировщик" через "Каталог курсов" с проверкой фильтрации по курсам
   ![Нетология — обучение современным профессиям онлайн 2023-09-25 13-39-13](https://github.com/Dimonstratos/HW4.2/assets/130654761/7d2d3a7e-c2e0-4909-8075-163a02852326)
   ![Курсы программирования онлайн – обучение с нуля - Нетология 2023-09-25 13-32-00](https://github.com/Dimonstratos/HW4.2/assets/130654761/cea3c710-864c-4ded-96ef-57b70855e064)
1. Навигация с главной страницы на страницу каталога курсов раздела "Программирование" через раздел "Направления обучения"
   ![Desktop 2023-09-25 20-27-17](https://github.com/Dimonstratos/HW4.2/assets/130654761/6105636c-47d4-49ba-8d65-2dff84071e7b)
1. Навигация с футера главной страницы на страницу "Программирование"
   ![Desktop 2023-09-25 20-38-01](https://github.com/Dimonstratos/HW4.2/assets/130654761/6d62f335-f4ab-4002-b8fd-ee6c570f5346)
1. Навигация с футера главной страницы на страницу "Популярные курсы"
   ![Desktop 2023-09-25 20-40-21](https://github.com/Dimonstratos/HW4.2/assets/130654761/b7edc86a-92db-4636-be0a-dc250a2bf194)
1. Навигация с футера главной страницы на страницу "Каталог курсов"
   ![Desktop 2023-09-25 20-42-40](https://github.com/Dimonstratos/HW4.2/assets/130654761/2f2c5869-8551-45c7-988a-10352b78c874)
1. Переход со страницы курса "Тестировщик ПО" к форме записи на курс
   ![Desktop 2023-09-25 20-51-46](https://github.com/Dimonstratos/HW4.2/assets/130654761/ae0a9132-f0cc-43cf-bc12-86546a33310d)

## Сценарии тестирования:
1. Успешная отправка валидно заполненной формы записи на курс "Тестировщик ПО", включая проверку ввода действующего промокода (с изменением стоимости курса) и перехода на страницы с условиями политики и 
   пользовательского соглашения
1. Появление сообщения "Должно состоять из букв" у поля "Имя" при заполнение его спецсимволами в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Должно состоять из букв" у поля "Имя" при заполнение его цифрами в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Должно быть не короче 2 символов" у поля "Имя" при заполнение его одной буквой в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Обязательное поле" у поля "Имя" при оставление поля пустым в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Номер в формате +9 (999) 999-99-99" у поля "Телефон" при заполнение поля 8 цифрами в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Номер в формате +9 (999) 999-99-99" у поля "Телефон" при заполнение поля 15 цифрами в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Обязательное поле" у поля "Телефон" при оставление поля пустым в форме записи на курс "Тестировщик ПО"
1. Появление сообщения "Устаревший промокод" у поля "Промокод" при вводе устаревшего валидного промокода в форме записи на курс "Тестировщик ПО" 10.Появление сообщения "Промокод не найден" у поля "Промокод" при 
   вводе не валидного промокода в форме записи на курс "Тестировщик ПО"

# Перечень используемых инструментов с обоснованием выбора
1. IDE: IntelliJ IDEA
1. Язык программирования: Java
1. Система сборки: Gradle (легче настраивать зависимости)
1. Фреймворк для UI тестирования: Selenide (популярный и простой инструмент)
1. Фреймворк для API тестирования: REST Assured вместе с JSON Schema Validator (для отправки необходимых запросов и валидации JSON схемы)
1. Фреймворки для управления данными: Java Faker (для генерации данных), необходимый драйвер (в зависимости от диалекта) для подключения к БД и DBUtils (для чтения записей с БД), Gson (для генерации body  
   апросов при API тестирования)
   
# Перечень необходимых разрешений, данных и доступов
1. Разрешение на проведение автотестирования
1. Доступ к тестовым данным
1. Доступ на чтения БД

# Перечень и описание возможных рисков при автоматизации
1. Дополнительная нагрузка на сервер
1. Появление "мусорных" записей в БД
1. Потеря актуальности тестов при изменение сайта

# Перечень необходимых специалистов для автоматизации
   Достаточно тестировщика уровня junior

# Интервальная оценка с учётом рисков в часах
   У спеиалиста написание тестов займет, примерно 20-24 часа.
