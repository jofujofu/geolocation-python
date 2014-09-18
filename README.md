![Alt text](https://travis-ci.org/slawek87/geolocation-python.svg?branch=master)

What is Geolocation?
=====================
Geolocation is a simple and clever application which uses google maps api.
This application allows you to easily and quickly get information about given location.
Application returns such information as: 

* country, 
* city, 
* route/street, 
* street number,
* lat, 
* lng.


What do You need?
-----------------
To use this application you need to have Google API key.
    [Google Maps Documentation](https://developers.google.com/maps/documentation/geocoding/) -- Geocoding

1. Open [APIs console](https://code.google.com/apis/console).

  ![Alt text](https://github.com/slawek87/geolocation-python/blob/master/docs/images/geocode-1.png?raw=true "APIs console")

2. Turn On Geocode API.

  ![Alt text](https://github.com/slawek87/geolocation-python/blob/master/docs/images/geocode-2.png?raw=true "Geocode Api")

3. Get your API Key.

  ![Alt text](https://github.com/slawek87/geolocation-python/blob/master/docs/images/geocode-3.png?raw=true "API KEY")


How to install it?
-------------------
    pip install geolocation-python


How to use it?
-----------------------
```python
# -*- coding: utf-8 -*-

from geolocation.google_maps import GoogleMaps

address = "New York City Wall Street 12"

google_maps = GoogleMaps(api_key='your_google_maps_key')

print location.all() # returns all locations.

my_location = location.first() # returns only first location.

print my_location.city
print my_location.route
print my_location.street_number
print my_location.country
print my_location.country_shortcut
print my_location.lat
print my_location.lng
```
    
More examples you should find in https://github.com/slawek87/geolocation-python/tree/master/examples