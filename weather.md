import requests,json

api= "9adced7ddff5c6dc7f031455d3dec00e"

site_address="http://api.openweathermap.org/data/2.5/weather?"

city = input("add city:")

final_weather = site_address  + "appid=" +api+ "&q=" + city+ "&units= meteric"

response = requests.get(final_weather)

k = response.json()
k['main']['temp']
