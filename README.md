# Illustrated Weather project

## Overview

A web (and eventually mobile) app that, when the site/app is visited, will ask the user for their location, take that location and use an API to get the weather for that location, and then display it for the user to see.

## Business Rules

* If weather is sunny AND warm, display sunny sky and warm city image
* If weather is sunny AND cold, display sunny sky and cold city image
* If weather is rainy AND warm, display rainy sky and warm city image
* Etc...

Mockups and images will be provided by a designer (yours truly). Until then, just worry about getting user's location and weather.

Temperatures are defined as follows (farenheit):

* **Hot**: 85*+
* **Warm**: 60 - 84.9*
* **Cool**: 35 - 59.9*
* **Cold**: 34.9* or below

## Technical Requirements

* Use the [html5 Geolocation API](http://www.w3schools.com/html/html5_geolocation.asp) (with jQuery) to ask for and get user's location
* Use any weather API of choice (with jQuery) to take user's location info and get weather info (just google "weather api" and see what looks promising... I think Yahoo has one that might be good)

## Pseudo-code step suggestions:

1. Get html/css/jquery files all set up and working (blank page to start)
2. Use javascript/jquery and the html5 geolocation api to ask for and return a location in the console by `console.log`ing (lat/long) when a user visits the page
3. Use that location and pass it to a weather api to get back some weather (using jQuery's `$.ajax` method). `console.log` that to the console (still blank webpage at this point)
4. Create a blank div in the html called `<div id="weather"></div>` or something to that effect
5. Insert the location and current temperature into that div (see mockup below)
6. Once I give you images, insert appropriate classnames into the html based on the temperature (technically you can do this before you have the images, they just won't show). Code example below.
7. Figure out what to name the app, get a domain, add it to hosting, then thow this puppy on the web. 

`<body class="sunnySky sunnyCity>`

`  <div id="weather"></div>`

`</body>`

## Mockup

Here's a lil mockup of what this could look like, including a v2 feature (what to wear). Ignore the actual background and icons, I would create new illustrations for this.

![illustrated_weather](https://cloud.githubusercontent.com/assets/223514/6180087/1598b916-b2d5-11e4-980b-6a5eb2267113.jpg)
