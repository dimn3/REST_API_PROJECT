### Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:
git clone https://github.com/dimn3/REST_API_PROJECT.git
cd infra_sp2
Cоздать и активировать виртуальное окружение:
python3 -m venv env
* Если у вас Linux/macOS
    source env/bin/activate
* Если у вас windows
    source env/scripts/activate
python3 -m pip install --upgrade pip
Установить зависимости из файла requirements.txt:
pip install -r requirements.txt
Выполнить миграции:
python3 manage.py migrate
Запустить проект:
python3 manage.py runserver

___________________________________________________________________________________________________________________________________________________

Проект представляет собой REST API для проекта , в котором собираются отзывы поьзователей на различные произведения.
В данном проекте REST API для проекта реализован следующий функционал:
* Получение списка категорий или добавление категории администратором, поиск категории по названию, удаление категорий администратором.
* Получение списка  жанров или добавление жанра администратором, удаление жанра администратором.
* Получение списка произведений или отдельного произведения по id или добавление произведения администратором, удаление произведения администратором,частичное обновление информации по произведению администратором.
* Получение списка отзывов или отдельного отзыва по id, добавление нового отзыва, но только одного на одно произведение Аутентифицированным пользователем, частичное изменение или удаление отзыва автором отзыва, администратором или модератором.
* Получение всех комментариев к отзыву по id.
* Просмотр, создание, удаление и изменение комментариев.
* Создание аккаунта пользователя самим пользователем или суперюзером.
* Авторизация по JWT (JSON Web Token) токену.
* Регистрация пользователей и управление правами доступа.
## Используемые технологии
* Python 3.7
* Django 2.2
* Django Rest Framework 3.12
* Postman
* Simple-JWT 4.7.2
## Установка проекта
Клонируйте данный репозиторий на свой компьютер и перейдите в папку проекта.
<pre><code>git clone https://github.com/dimn3/REST_API_PROJECT.git</code>
<code>cd api_final_yatube</code></pre>
Создайте и активируйте виртуальное окружение:
<pre><code>python -m venv venv</code>
<code>source venv/Scripts/activate  #для Windows</code>
<code>source env/bin/activate       #для Linux и macOS</code></pre>
Установите требуемые зависимости:
<pre><code>pip install -r requirements.txt</code></pre>
Примените миграции:
<pre><code>python manage.py migrate</code></pre>
Запустите django-сервер:
<pre><code>python manage.py runserver</code></pre>
## Документирование API
Структура запросов и ответов API документирована в ReDoc.
После запуска проекта документация доступна по адресу http://localhost:8000/redoc/


Лицензия MIT

Авторское право (c) 2023 Парфенов Дмитрий

Настоящим бесплатно предоставляется разрешение любому лицу, получающему копию
этого программного обеспечения и связанных с ним файлов документации ("Программное обеспечение"), на работу
с Программным обеспечением без ограничений, включая без ограничений права
на использование, копирование, модификацию, объединение, публикацию, распространение, сублицензирование и/или продавать
копии Программного обеспечения и разрешать лицам, которым предоставляется программное
обеспечение, делать это при соблюдении следующих условий:

Вышеуказанное уведомление об авторских правах и это уведомление о разрешении должны быть включены во все
копии или существенные части программного обеспечения.

ПРОГРАММНОЕ ОБЕСПЕЧЕНИЕ ПРЕДОСТАВЛЯЕТСЯ "КАК ЕСТЬ", БЕЗ КАКИХ-ЛИБО ГАРАНТИЙ, ЯВНЫХ ИЛИ
ПОДРАЗУМЕВАЕМЫХ, ВКЛЮЧАЯ, НО НЕ ОГРАНИЧИВАЯСЬ ГАРАНТИЯМИ ТОВАРНОЙ ПРИГОДНОСТИ,
ПРИГОДНОСТИ ДЛЯ ОПРЕДЕЛЕННОЙ ЦЕЛИ И ОТСУТСТВИЯ НАРУШЕНИЙ. НИ В КОЕМ СЛУЧАЕ
АВТОРЫ ИЛИ ПРАВООБЛАДАТЕЛИ НЕ НЕСУТ ОТВЕТСТВЕННОСТИ ЗА КАКИЕ-ЛИБО ПРЕТЕНЗИИ, УЩЕРБ ИЛИ ДРУГИЕ
ОТВЕТСТВЕННОСТЬ, БУДЬ ТО В РЕЗУЛЬТАТЕ ДЕЙСТВИЯ ДОГОВОРА, ДЕЛИКТА ИЛИ ИНЫМ ОБРАЗОМ, ВОЗНИКАЮЩАЯ ИЗ,
ВНЕ ПРОГРАММНОГО ОБЕСПЕЧЕНИЯ ИЛИ В СВЯЗИ С НИМ, А ТАКЖЕ С ИСПОЛЬЗОВАНИЕМ ПРОГРАММНОГО ОБЕСПЕЧЕНИЯ ИЛИ ДРУГИМИ ОПЕРАЦИЯМИ С НИМ.

MIT License

Copyright (c) 2023 Parfenov Dmitrii

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
