### Лабораторная работа 3. OpenweatherAPI

Реализована функциия `get_weather_data(place, api_key=None)` в модуле
`getweatherdata`, в которой происходит получение информации 
о погоде с сайта [https://openweathermap.org/](https://openweathermap.org/).

Функция возвращает объект в **формате JSON**, включающий:

- информацию о названии города (в контексте openweathermap),
- код страны (2 символа),
- широту и долготу, на которой он находится,
- его временной зоне,
- а также о значении температуры (как она ощущается)


```python
get_weather_data('Kiev', api_key=key)
{"name": "Kyiv", "coord": {"lon": 30.52, "lat": 50.43}, "country": "UA", "feels_like": 21.96, "timezone": "UTC+3"}```

Результат:
{"coord": {"lon": 37.6156, "lat": 55.7522}, "feels_like": -4.59, "country": "RU", "timezone": "UTC+03:00", "name": "Moscow"}
{"coord": {"lon": -87.65, "lat": 41.85}, "feels_like": 0.75, "country": "US", "timezone": "UTC-06:00", "name": "Chicago"}
{"coord": {"lon": 30.2642, "lat": 59.8944}, "feels_like": -9.41, "country": "RU", "timezone": "UTC+03:00", "name": "Saint Petersburg"}