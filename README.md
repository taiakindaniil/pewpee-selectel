# pewpee-selectel

## Описание проекта

PewPee – облачный музыкальный стриминговый сервис, который доступен во всех странах мира. Можно пользоваться как iOS/iPadOS приложением, так и в веб-браузере (в будущем будет развиваться кроссплатформенность).

Приложение iOS входит в [топ чарты App Store](https://app.sensortower.com/category-rankings?os=ios&start_date=2023-09-01&end_date=2023-09-30&countries=US&category=6011&chart_type=free&device=iphone&hourly=false&selected_tab=country-summary&date=2023-09-30&app_id=1483338834&summary_chart_type=topfreeapplications) во многих странах мира, включая США, Мексику, Турцию, Эквадор, Ирак, Аргентину, Австрию и т.д. Количество скачиваний уже превысило 250 тыс. единиц.

PewPee имеет свою собственную базу данных музыкальных треков, которых уже более 1 млн (музыка лицензирована). И она дальше продолжает расти. Помимо базы данных музыки, PewPee предоставляет возможность импортировать свои песни через облачные сервисы (Google Drive, Dropbox, iCloud и прочие) или прямо с устройства.

Функциональные возможности не уступают другим популярным стриминговым сервисам: офлайн режим; просмотр текстов песен; создание и редактирование собственных плейлистов; добавление плейлистов / альбомов / треков / исполнителей в свою медиатеку; подписываться и следить за друзьями через ленту; следить за новыми релизами / топ-чартами / популярными плейлистами / исполнителями; находить музыку по жанрам; слушать в shuffle режиме; установливать таймер сна и многое другое (введение персонализированной подборки музыки при помощи нейронных сетей будет тоже добавлено в скором времени).

[Веб-приложение](https://pewpee.com) было первым что вышло в свет, и код писался тогда, когда я только начинал изучать программирование (PHP, SQL, JavaScript + jQuery). Однако приложение для iOS уже развивалось по-другому. Сперва, я написал серверную сторону с API и с собственным протоколом OAuth2 (на PHP). Сейчас я все разбиваю на микросервисы с использованием Docker-контейнеров и брокера для связи между ними. Для того, чтобы сделать какие-то сервисы в PewPee быстрее, использую Redis (к примеру, для пользоовательской ленты). Затем, создавал нативное приложение под iOS, используя язык программирования Swift и MVC модель.

Идеология: нет рекламы, данные не передаются 3-м сторонам. Ознакомится с политикой конфиденциальности можно [тут](https://pewpee.com/privacy).

PewPee находится в стадии активной разработки, и планируется расширение не только в масштабах нескольких операционных систем, но и в создании удобных сервисов для артистов для продвижения и монетизации их работ.

## Ссылки
1. https://pewpee.com
2. https://apps.apple.com/us/app/pewpee-music-player/id1483338834
