# LocationApp-BackEnd

Api keys have been removed!

This is the backend part of the LocationApp. This accepts 2 coordinates from 2 different cities. It then searches the places inbetween and returns it as JSON data. The data is then split by 5 parts of a route and using the OpenWeatherApi the biggest temperature is taken from each part. The data is then send back to the front end. 

All dependancies this app requires, can be installed using nmp install.

It uses:
- express
- axios
- cors

Inside the app, it uses arrays to temporary store the data, and an array called Objects, to store it finaly, before sending it. It firstly gets the route from one to another location, then it checks the weather of the 2 sent locations, and then loops over all other locations. 

The Api final object response looks like this:

![alt text](https://github.com/fpv-life/LocationApp-BackEnd/blob/master/Pictures/slika%20api%20requesta.PNG)
