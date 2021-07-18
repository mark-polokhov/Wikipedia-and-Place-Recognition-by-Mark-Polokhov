# Wikipedia-and-Place-Recognition-by-Mark-Polokhov

Это приложение позволяет открыть любую вики страницу и отобразить на карте все места, упомянутые на ней.
Делается это при помощи web-scraping на языке Python через Beautiful Soup, который собирает все ссылки на странице и среди них отбирает только те, текст которых напоминает название.
После этого отправляет запросы к Mapbox API, которое возвращает список мест с похожим названием, и отбирает самые релевантные, а затем отбражает их на карте на веб-странице. 

## Установка

+ Скачать репозиторий в локальную папку
+ Открыть данную папку через терминал/консоль
+ Выполнить команду ```pip install -r requirements.txt```
+ Создать в папке файл ```mapbox_key.txt```, в который нужно записать Ваш API access token.
  
  Получить его можно на сайте [mapbox.com](https://www.mapbox.com/)
  
+ Открыть сайт (бла бла)
+ готово
