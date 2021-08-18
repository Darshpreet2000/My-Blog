---
keywords: fastai
description: "Working on Home Screen backend with BLoC Architecture"
title: "Coding Period: Week 3"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
nb_path: _notebooks/2020-06-19-Week-3-June-14 -To-June-19.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2020-06-19-Week-3-June-14 -To-June-19.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>This week I learned BLoC Architecture in Flutter, I understood it quickly from YouTube videos. I started implementing it in App.</p>
<p>I will try to explain first what BLOC components should do as short as possible (and as trivial as possible).</p>
<ul>
<li><p>UI screen - obviously shows data to the user</p>
</li>
<li><p>BLOC (or the ViewModel) - decides HOW to display data to the user, do we make the text bold, do we show the error, do we go to next screen.</p>
</li>
<li><p>Repo - decides WHAT data to display to the user (do we show the content from db, do we fetch it from API)</p>
</li>
</ul>
<h3 id="Working-on-Home-Screen-Backend">Working on Home Screen Backend<a class="anchor-link" href="#Working-on-Home-Screen-Backend"> </a></h3><p>I have created BLoC for home screen &amp; location services, I have done the following tasks in Home screen</p>
<ol>
<li><p>Fetched &amp; Displayed User Location using Geolocator Package
App will ask for location permission &amp; will access location of user, I have used two packages</p>
<ul>
<li><p>location - For asking GPS Permission</p>
</li>
<li><p>GeoLocator - For Getting coordinates of user location</p>
</li>
</ul>
</li>
<li><p>Fetched Nearby Hospitals using Overpass API</p>
<ul>
<li><p>Used Overpass API for Getting Nearby Hospitals, I have to pass Location Coordinates &amp; radius to get hospitals around my          Location</p>
</li>
<li><p>Then I Parsed JSoN data recieved to list of objects</p>
</li>
</ul>
</li>
<li><p>Fetching Image of each hospital from Google</p>
<ul>
<li>For fetching images, I have Used FutureBuilder Widget in flutter which executes a function which searches on Google by          Hospital name &amp; fetches the HTML Response, Then I get the link of first image &amp; pass it to another widget Cached Netwrok        Image which loads the image.</li>
</ul>
</li>
<li><p>Using Shimmer Loading Effect to load list</p>
<ul>
<li>I have use flutter shimmer package for doing this, I have created a ListTile for this, While the data is Loading I display      this.</li>
</ul>
</li>
</ol>
<h3 id="GIF-of-Home-Screen">GIF of Home Screen<a class="anchor-link" href="#GIF-of-Home-Screen"> </a></h3><p><img src="https://github.com/Darshpreet2000/My-Blog/blob/master/images/home_demo.gif?raw=true" alt="Home Demo"></p>
<h3 id="SQL-Database-Class">SQL Database Class<a class="anchor-link" href="#SQL-Database-Class"> </a></h3><p>Completed Main functionality of SQL Database class</p>
<ul>
<li>Implemented Basic Insertion in SQL Database using Flutter <strong>sqflite</strong> package, Some Other function are remaining which I will complete in upcoming weeks</li>
</ul>
<h3 id="Working-on-Web-Crawler">Working on Web Crawler<a class="anchor-link" href="#Working-on-Web-Crawler"> </a></h3><p>Scraped CDM of Indiana State</p>
<ul>
<li>I have Used Data Provided by Indiana State, It contains discharge data of Hospitals of 2018, I have scraped data using scrapy, processed data to proper column names using python.</li>
</ul>
<h3 id="What-do-I-plan-to-do-next-week">What do I plan to do next week<a class="anchor-link" href="#What-do-I-plan-to-do-next-week"> </a></h3><ol>
<li><p>I have used shared pref to store some data, I will replace it with Hive</p>
</li>
<li><p>I will use sqflite to store CDM</p>
</li>
<li><p>Working on Main Feature of this App [ Compare Prices Screen]</p>
</li>
<li><p>Scraping CDM of New York State</p>
</li>
</ol>

</div>
</div>
</div>
</div>
 
