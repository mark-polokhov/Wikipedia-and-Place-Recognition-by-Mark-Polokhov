# Wikipedia and Place Recognition by Mark Polokhov

Это приложение позволяет открыть любую вики страницу и отобразить на карте все места, упомянутые на ней.
Делается это при помощи web-scraping на языке Python через Beautiful Soup, который собирает все ссылки на странице и среди них отбирает только те, текст которых напоминает название.
После этого отправляет запросы к Mapbox API, которое возвращает список мест с похожим названием, и отбирает самые релевантные, а затем отображает их на карте на веб-странице. 

С помощью данной программы можно иследовать явление глобализации, влияние одних стран на другие, пытаться анализировать, какое из разных мест на карте с одинаковым названием искал пользователь, и многое другое.


## Установка и запуск

+ Скачать репозиторий в локальную папку
+ Открыть данную папку через терминал/консоль
+ Выполнить команду ```pip install -r requirements.txt```
+ Создать в папке файл ```mapbox_key.txt```, в который нужно записать Ваш API access token.
  
  Получить его можно на сайте [mapbox.com](https://www.mapbox.com/)
  
+ Запустить сервер, выполнив команду ```python main.py``` на Windows или ```python3 main.py``` для Linux и MacOS.
+ Открыть http://localhost:5000/form

После этого вы попадёте на страницу, которая и представляет интерфейс приложения.


## Использованные технологии

+ Языки программирования Python, HTML, Javascript
+ Mapbox API
+ Flask
+ Beautiful Soup

## Рекомендации

Лучше всего использовать англоязычную Википедию. Связанно это с тем, что Mapbox API официально не поддерживает русский язык и поэтому плохо отвечает на запросы на русском.
