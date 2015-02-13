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

* Use the html5 Geolocation API (with jQuery) to ask for and get user's location
* Use any weather API of choice (with jQuery) to take user's location info and get weather info (just google "weather api" and see what looks promising... I think Yahoo has one that might be good)

## Pseudo-code step suggestions:

1) Get html/css/jquery files all set up and working (blank page to start)
2) Use javascript/jquery and the html5 geolocation api asking for and returning a location in the console by `console.log`ing (lat/long) when a user visits the page
3) Use that location and pass it to a weather api to get back some weather (using jQuery's `$.ajax` method). `console.log` that to the console (still blank webpage at this point)
4) Create a blank div in the html called `<div id="weather"></div>` or something
5) Insert the location and current temperature into that div. Example:

    89*
Las Vegas, NV

6) Once Jen gives you images, insert appropriate classnames into the html based on the temp (technically you can do this before you have the images, they just won't show). Example:

`<body class="sunnySky sunnyCity>`
`  <div id="weather"></div>`
`</body>`

