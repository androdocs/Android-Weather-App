# Android-Weather-App
<img  src='https://www.androdocs.com/files/uploads/original/creating-an-android-weather-app-using-kotlin-1565972769.jpg' >

<br>
<p>This project is on Creating an Android Weather App using Kotlin.
To get the weather information I used <a href="https://openweathermap.org" target="_blank">OpenWeatherMap</a> API. 
Informations like Temperature, Pressure, Humidity, Weather status, Time of Sunrise and Sunset etc. are passed from the API.</p>
<p>Visit the blog post on <a href="https://www.androdocs.com/tutorials/creating-an-android-weather-app-using-kotlin.html" target="_blank">
<b>Creating an Android Weather App using Kotlin</b>
</a>
</p>


<br><h2>Get an API key from OpenWeatherMap</h2>
<p>For retrieving data we will use <strong>OpenWeatherAPI</strong>, and we will be needing an API key for it. Before proceeding please get an API key by registering. You can either follow the attached video above or steps below.</p>
<ol>
<li>Create a New Account from <a title="Create new account" href="https://home.openweathermap.org/users/sign_up" target="_blank" rel="noopener">here</a>.</li>
<li>After login go to <a title="Get the API key" href="https://home.openweathermap.org/api_keys" target="_blank" rel="noopener">here</a> to get the API Key.</li>
</ol>

<br><h2>Getting weather information using Latitude & Longitude</h2>
<p>Suppose you want to request weather information using a <strong>Latitude</strong> &amp; <strong>Longitude</strong> of a place, then you should use:</p>
<pre>response = URL("https://api.openweathermap.org/data/2.5/weather?lat=$LAT&amp;lon=$LON&amp;units=metric&amp;appid=$API").readText(
                    Charsets.UTF_8
                )</pre>
<p>where LAT and LON will be the Latitude &amp; Longitude respectively. If you want to implement this project to display weather
information of user's current location you'll just need detect the current latitude &amp; longitude. I've already posted an article on 
<a href="https://www.androdocs.com/tutorials/getting-current-location-latitude-longitude-in-android-using-kotlin.html" target="_blank">
Getting Current Location (latitude, longitude) in Android using Kotlin
</a>
</p>

