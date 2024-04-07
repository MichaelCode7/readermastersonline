# Masters of Reading Online
## Описание
**Masters of Reading Online**(или MARO) - сервис для загрузки, скачивания и чтения электонных книг.
Загружайте свои книги на сайт и удобно читайте их где угодно! Помимо этого вы можете создавать собственные сбоники.
MARO поддерживает популярные форматы электронных книг: *txt*, *ePub*, *PDF* и *fb2*.
Чтобы полноценно пользоватся сервисом неоходима регистрация.

## ТЗ
Сервис будет написан на Python 3.10, Flask, ORM SQLAlchemy, Flask-WTF.

### Страницы

#### Начальная
 - Базовая страница для новых юзеров. На ней подробно расписываются функции и возможности сервиса, а также предлагают регистрацию или вход.

#### Регистрация
 - Страница для регистрации новых пользователей, реализована будет на flask-wtf:
   - Поля: ввод ника, ввод emailа, ввод пароля, повторный ввод пароля, ввод описания, выбор даты рождения, выбор пола, дата регистрации(скрытно).
   - Переадресовывает на *Главную страницу аккаунта*.    

#### Вход
 - Страница для входа, будет реализована на flask-wtf:
   - I Поля: ввод emailа, ввод пароля.
   - II Поля: подтверждение emailа.
   - Переадресовывает на *Главную страницу аккаунта*.

#### Главная страница аккаунта
 - Будет кратко отображатся информация о юзере, книгах и сборниках.
 - *Подробную информацию о пользователе можно развернуть кликнув на ник.
 - Список книг/сборников открывается щелчками по блокам.

#### Список книг
 - На список можно применить фильтры.
 - Книги можно скачивать, загружать или читать.
 - Подбор алгоритма отображения происходит автоматически, учитывая тип электронной книги.
 - Скачиваются книги в том формате, в котором их загрузили(в будущем планирую это исправить).
