# Проект по SQL

## Описание проекта


Коронавирус застал мир врасплох, изменив привычный порядок вещей. В свободное время жители городов больше не выходят на улицу, не посещают кафе и торговые центры. Зато стало больше времени для книг. Это заметили стартаперы — и бросились создавать приложения для тех, кто любит читать.

Ваша компания решила быть на волне и купила крупный сервис для чтения книг по подписке. Ваша первая задача как аналитика — проанализировать базу данных. В ней — информация о книгах, издательствах, авторах, а также пользовательские обзоры книг. Эти данные помогут сформулировать ценностное предложение для нового продукта.


## Описание данных

**Таблица `books`**

Содержит данные о книгах:
* `book_id` — идентификатор книги;
* `author_id` — идентификатор автора;
* `title` — название книги;
* `num_pages` — количество страниц;
* `publication_date` — дата публикации книги;
* `publisher_id` — идентификатор издателя.


**Таблица `authors`**

Содержит данные об авторах:
* `author_id` — идентификатор автора;
* `author` — имя автора.

**Таблица `publishers`**

Содержит данные об издательствах:
* `publisher_id` — идентификатор издательства;
* `publisher` — название издательства;

**Таблица `ratings`**

Содержит данные о пользовательских оценках книг:
* `rating_id` — идентификатор оценки;
* `book_id` — идентификатор книги;
* `username` — имя пользователя, оставившего оценку;
* `rating` — оценка книги.

**Таблица ``reviews``**

Содержит данные о пользовательских обзорах:
* `review_id` — идентификатор обзора;
* `book_id` — идентификатор книги;
* `username` — имя автора обзора;
* `text` — текст обзора.


## Схема данных

![схема данных](https://pictures.s3.yandex.net/resources/scheme_1589269096.png "Yandex")


## Задачи

- Посчитайте, сколько книг вышло после 1 января 2000 года;
- Для каждой книги посчитайте количество обзоров и среднюю оценку;
- Определите издательство, которое выпустило наибольшее число книг толще 50 страниц — так вы исключите из анализа брошюры;
- Определите автора с самой высокой средней оценкой книг — учитывайте только книги с 50 и более оценками;
- Посчитайте среднее количество обзоров от пользователей, которые поставили больше 50 оценок.
