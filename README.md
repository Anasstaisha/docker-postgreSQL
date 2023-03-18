[![Build status](https://ci.appveyor.com/api/projects/status/qsdvaivkkw50dxfi?svg=true)](https://ci.appveyor.com/project/Anasstaisha/datapatterns))


# Задача: PostgreSQL

Вам необходимо подготовить приложение к тестированию на СУБД PostgreSQL. Используйте образ 12-alpine, если он недоступен, то берите последний опубликованный на Docker Hub. Возьмите собранный JAR-файл db-api.jar, аналогично примеру на лекции положите рядом файл application.properties, но в строке: jdbc:mysql://... поменяйте mysql на postgresql.

Вам нужно дописать остальные настройки: хост, порт, БД, имя пользователя и пароль.

Кроме того, вам нужно подготовить файл docker-compose.yml, в котором прописать настройки для запуска контейнера PostgreSQL. Всю информацию о его запуске вы найдёте на официальной странице образа на Docker Hub.

В результате выполнения этой задачи вы должны положить в репозиторий следующие файлы:

* db-api.jar,
* application.properties,
* docker-compose.yml.

**Важно:** для удаления всех данных и начала с чистого листа сделайте следующее:

* docker-compose down в каталоге с файлом docker-compose.yml,
* удалите каталог для хранения данных data,
* запустите заново docker-compose up, после того как всё исправите.

**Важно:** команда docker-compose rm в каталоге с файлом docker-compose.yml удаляет сам контейнер.