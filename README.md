Тема 2. Домашня робота

Сьогодні ми перейдемо до практичної роботи з розгортанням застосунків.

Вам необхiдно клонувати FastAPI-застосунок, налаштувати його та запустити в Docker-контейнері. Після цього перевірите правильність роботи застосунку і переконатись в успішному підключенні до бази даних.

Технічний опис завдання

1. Використовуючи команду git clone, клонуйте репозиторій за адресою https://github.com/GoIT-Python-Web/FullStack-Web-Development-hw2. Перейдіть у клонований каталог.

2. Створіть Dockerfile із вказівками для створення образу Docker застосунку.

3. Напишіть docker-compose.yaml з конфігурацією для застосунку та PostgreSQL.

4. Використайте Docker Compose для побудови середовища, команду docker-compose up для запуску середовища.

💡 Підказка:

Внесіть зміни в рядку підключення до бази даних SQLALCHEMY_DATABASE_URL: вона знаходиться у файлі \\conf\\db.py. Замість localhost вставте ім'я сервісу PostgreSQL з вашого файлу docker-compose.yaml .

SQLALCHEMY_DATABASE_URL = f"postgresql+psycopg2://postgres:567234@localhost:5432/hw02"

Коли ви використовуєте Docker Compose, кожен сервіс (контейнер) має власну мережу, і вони зазвичай не можуть звертатися один до одного за допомогою localhost. Замість цього, ви маєте використовувати назву сервісу в якості імені хоста.

5. Перевірте функціональність застосунку та доступність бази даних.

💡 Підказка:

Після запуску контейнера із застосунком вигляд у браузері повинен бути наступним:

Якщо все правильно налаштовано у файлі docker-compose.yaml, натиснувши кнопку Перевірити БД, ви повинні побачити наступне:

Якщо замість"Welcome to FastAPI!” ви бачите червоне віконце з повідомленням про помилку, значить ви неправильно налаштували docker-compose.yaml

Критерії прийняття

Клоновано репозиторій, створено Dockerfile для створення образу Docker застосунку.
Написано docker-compose.yaml з конфігурацією для застосунку та PostgreSQL.
Використано Docker Compose, команду docker-compose up для побудови та запуску середовища.
Застосунок є функціональним, а база даних — доступною, що підтверджується натисканням кнопки Перевірити БД.

Підготовка та завантаження домашнього завдання

Створіть публічний репозиторій goit-pythonweb-hw-02.
Виконайте завдання та відправте його у свій репозиторій.
Завантажте робочі файли на свій комп’ютер та прикріпіть їх у LMS у форматі zip. Назва архіву повинна бути у форматі ДЗ2_ПІБ.
Прикріпіть посилання на репозиторій goit-pythonweb-hw-02 та відправте на перевірку.

Формат оцінювання

Залік / Незалік

Формат здачі

Прикріплені файли репозиторію у форматі zip з назвою ДЗ2_ПІБ.
Посилання на репозиторій.
🚨 ВАЖЛИВО
Перегляньте Інструкцію щодо завантаження робочого файлу з репозиторію на Github