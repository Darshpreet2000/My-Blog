---
keywords: fastai
description: "GSoC wrap-up"
title: "GSoC Journey Ended Only, Not The Open Source"
toc: false
branch: master
badges: true
comments: true
hide: false
search_exclude: true
nb_path: _notebooks/2020-09-01-GSoC-Wrap-Up.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2020-09-01-GSoC-Wrap-Up.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<table>
{% include image.html align="top" file="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/gsoc_logo.png" %}
{% include image.html align="top" file="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/librehealth.png" %}
</table><p>Hello, This blog is about my Google Summer Of Code journey with <a href="https://librehealth.io/">LibreHealth</a>, it covers everything from applying for GSoC, getting selected, community bonding to final evaluations. I hope you will enjoy reading this &amp; will find something useful in it. So, Let's get started.</p>
<h3 id="Little-Bit-About-Myself">Little Bit About Myself<a class="anchor-link" href="#Little-Bit-About-Myself"> </a></h3><p>I am Darshpreet Singh currently pursuing Bachelor Of Technology in Computer Science &amp; Engineering, I have just completed my second year of engineering. From the beginning of my second year I started learning mobile app development, I was really passionate about app development and then got into the field deeper with time, completed 2 internships, and so on my journey with open source started</p>
<h3 id="Aiming-for-GSoC-2020-&amp;-Submitting-POC,-Proposal">Aiming for GSoC 2020 &amp; Submitting POC, Proposal<a class="anchor-link" href="#Aiming-for-GSoC-2020-&amp;-Submitting-POC,-Proposal"> </a></h3><p>I heard a lot about GSoC from my college seniors and LinkedIn, I started asking a lot to people on LinkedIn how to get selected &amp; what more should I learn. I got replies from lot of people they guided me a lot. I aimed to get selected in GSoC in 2020, I contributed in some organisation before the GSoC but the projects I contributed to were not selected, I was little disappointed. Still I had some hope I kept searching in the organisation &amp; projects list to find an android related project. Finally after searching a lot I found LibreHealth, they had a lot of projects in mobile development, I aimed to submit my best to this organisation, I completed the POC(Proof Of Concept) task in just 2 days, I also did more than the required. I communicated a lot with mentors &amp; after discussing a lot I submitted my proposal.</p>
<h3 id="Getting-Selected">Getting Selected<a class="anchor-link" href="#Getting-Selected"> </a></h3><p>It was a long month for me waiting for the results, On day of result I frequently checked my mail &amp; GSoC website for result. It was 4th May at 11:30 PM, I got surprised to see that I am selected for GSoC, I was very happy, I thanked my mentors a lot for selecting me &amp; assured them that I will defintely work hard &amp; will make them feel proud of my work. Due to my excitement I was not able to sleep on time, I slept late at night but woke up early to start my GSoC journey &amp; to tell my parents &amp; friends about it.</p>
<p><img src="https://github.com/Darshpreet2000/My-Blog/blob/master/images/gsoc_selection.jpeg?raw=true" alt="download_cdm"></p>
<h3 id="About-Project">About Project<a class="anchor-link" href="#About-Project"> </a></h3><p>To make an app which can display costs of medical procedures of US hospitals &amp; a web scraper which can scrape ChargeMasters &amp; update data periodically in GitLab Repository. The app will display nearby hospitals and the user can compare hospitals, filter hospitals based on location &amp; radius. App can download nearby hospitals ChargeMaster from GitLab Repository and save it to local storage of phone in SQL database. User can view downloaded ChargeMaster, search in it, filter by price &amp; category. This App can work offline and can update downloaded ChargeMasters.</p>
<h2 id="About-My-Work">About My Work<a class="anchor-link" href="#About-My-Work"> </a></h2><h3 id="The-Community-Bonding-Period">The Community Bonding Period<a class="anchor-link" href="#The-Community-Bonding-Period"> </a></h3><p>The community period begin the next day, I introduced myself to community &amp; other selected students. I discussed a lot about project ideas such as use of API to get nearby hospitals &amp; dicussing about CI (Continous Integration) Pipeline which will scrap the chargemasters every month automatically. Searched data on internet to get chargemasters, I found some websites of US government which had good amount of data.</p>
<h3 id="First-Work-Period">First Work Period<a class="anchor-link" href="#First-Work-Period"> </a></h3><ul>
<li>Completed UI of App Screens with Dummy Data</li>
<li>Worked on Data Scraper</li>
<li>Setup GitLab CI Pipeline</li>
<li>Scraped &amp; Processed CDM of Alaska State</li>
<li>Made SQL Database class for App</li>
<li>Worked on Home Screen backend Code<ul>
<li>Used Overpass API to fetch Nearby hospitals</li>
<li>Used Google Images to get image of hospital by name</li>
</ul>
</li>
<li>Scraped &amp; Processed CDM of Indiana State</li>
<li>Learned &amp; Used Flutter BLoC (Business Logic Of Component) Architecture </li>
<li>Used Hive to store local data</li>
<li>Worked on new tab in bottom navigation which will download cdm</li>
<li>Wrote SQL queries with which we can read &amp; insert data in SQL Database in App</li>
</ul>
<h4 id="Blockers-Faced">Blockers Faced<a class="anchor-link" href="#Blockers-Faced"> </a></h4><ul>
<li>I wanted app to completely work offline after it fetched data once, So I started to store everything locally, I faced problem in saving images of hospitals, I thought it is not necessary to store images when user is offline, So, I am showing a placeholder, but whenever internet will be ON user can view images of hospitals as well </li>
</ul>
<h3 id="Second-Work-Period">Second Work Period<a class="anchor-link" href="#Second-Work-Period"> </a></h3><ul>
<li>Worked on Search Screen of App.</li>
<li>Made DAO ( Data Access Object ) class which uses SQL queries to query database.</li>
<li>Made Comparing Hospitals procedures functionality</li>
<li>Tested both IOS &amp; Android App</li>
<li>Scraped CDM of California State </li>
<li>Wrote Readme.md file for scraper</li>
<li>Separated “process.py” from “Data” Directory, so that user don’t need to clone large repository.</li>
<li>I have to setup chromedriver &amp; chromebrowser in CI Pipeline &amp; then make this project run properly</li>
<li>I worked on Showing progress indicator while downloading CDM &amp; saving to SQL database.</li>
<li>Fixed Network exceptions while downloading CDM in app.</li>
<li>Made Readme.md &amp; troubleshoot.md for web scraper</li>
<li>Fixed the blocker</li>
<li>Completed UI of compare hospitals screen</li>
<li>Fixed bugs in download CDM screen</li>
<li>Scraped Medicare Data &amp; wrote process script for that</li>
</ul>
<h4 id="Blockers-Faced">Blockers Faced<a class="anchor-link" href="#Blockers-Faced"> </a></h4><p>chromedriver &amp; chromebrowser were not working in Linux CI Pipeline, I was getting exception in pipeline, but it was working on my windows. I solved this blocker after searching too much on internet &amp; found that chromedriver &amp; chromebrowser need to be same.</p>
<h3 id="Third-Work-Period">Third Work Period<a class="anchor-link" href="#Third-Work-Period"> </a></h3><ul>
<li>Worked on Share App, About App screens.</li>
<li>Used Flutter cache Manager to download &amp; Save CDM to cache.</li>
<li>Search functionality in view CDM Screen.</li>
<li>Decreased size of data scraper repository</li>
<li>Fixed CI pipeline &amp; CDMs are saved in master branch</li>
<li><p>Wrote Unit Test of</p>
<ul>
<li>Home Screen</li>
<li>Download CDM screen,</li>
<li>Saved CDM Screen</li>
<li>View CDM</li>
<li>Search Screen</li>
<li>View CDM Statewise screen</li>
<li>Compare Hospital Screen</li>
<li>Settings Screen</li>
</ul>
</li>
<li><p>Also Wrote Unit Tests for Overpass API, GitLab API, Medicare Hospital Compare API</p>
</li>
<li>Complete Readme.md for app</li>
<li>Created App Intro Slides </li>
<li>Worked on search by price in search screen of App</li>
<li>Created Splash Screen</li>
<li>Created option in App settings to choose any location of US to try App.</li>
<li>Fixed various bugs in App [ Fixed Location permission bug, if user denies then he has to manually allow location from settings ]</li>
<li>Used Orange LH theme as suggested by Mentor Mua N. Laurent.</li>
<li>Added retry button in snackbar of Location widget</li>
</ul>
<h4 id="Blockers-Faced">Blockers Faced<a class="anchor-link" href="#Blockers-Faced"> </a></h4><p>I don't have IOS machine, So I was not able to setup splash screen for ios app properly, I have asked Mentor Mua N. Laurent for help in this. Still I will try to use a virtual macOS to setup the splash screen.</p>
<h3 id="About-Mentors">About Mentors<a class="anchor-link" href="#About-Mentors"> </a></h3><p>I had 4 mentors assigned during GSoC</p>
<ul>
<li><p><a href="https://gitlab.com/muarachmann"><strong>Mua N. Laurent</strong></a></p>
</li>
<li><p><a href="https://gitlab.com/judywawira"><strong>Judy Gichoya</strong></a></p>
</li>
<li><p><a href="https://gitlab.com/sunbiz"><strong>Saptarshi Purkayastha</strong></a></p>
</li>
<li><p><a href="https://gitlab.com/robbyoconnor"><strong>Robby O Connor</strong></a></p>
</li>
</ul>
<p>I would like to thank all of them for their valuable suggestions &amp; their involvement with me during the project.
I want to specially thank mentor <a href="https://gitlab.com/muarachmann"><strong>Mua N. Laurent</strong></a> for guiding me very closely, having frequent chat &amp; video calls with me, testing my code, suggesting improvements in it. I could not reach this level without your mentoring.</p>
<h3 id="GSoC-Journey-Ended-Only,-Not-The-Open-Source">GSoC Journey Ended Only, Not The Open Source<a class="anchor-link" href="#GSoC-Journey-Ended-Only,-Not-The-Open-Source"> </a></h3><p>It was great experience for me during the GSoC working for open source projects. GSoC journey ended only, not my open source journey, I will continue to contribute to LibreHealth. I will assist the new members who are willing to contribute for this project. I will actively take part in the discussions and I will contribute by creating, Solving issues and adding improvements to this app.</p>
<h3 id="Link-to-my-work-report">Link to my work report<a class="anchor-link" href="#Link-to-my-work-report"> </a></h3><p><a href="https://gist.github.com/Darshpreet2000/9f08ee2080163851a2b6834c1eef16ba">https://gist.github.com/Darshpreet2000/9f08ee2080163851a2b6834c1eef16ba</a></p>
<h3 id="Conclusion">Conclusion<a class="anchor-link" href="#Conclusion"> </a></h3><p>GSoC was a wonderful experience for me, It improved a lot my programming skills, i would just say that GSoC is a great opportunity, work hard, be patient &amp; enjoy your summer writing code. And also become a part of your organization after completing this program.</p>
<h3 id="Screenshots">Screenshots<a class="anchor-link" href="#Screenshots"> </a></h3><table>
<thead><tr>
<th></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/home.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/settings.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/search_procedure.png" align="top"></td>
</tr>
<tr>
<td>Home screen displaying nearby hospitals &amp; user location</td>
<td>Settings screen to filter nearby hospitals &amp; change location</td>
<td>Search screen - Searching by procedure</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/search_price.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/filter.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/drawer.png" align="top"></td>
</tr>
<tr>
<td>Search screen - Searching by price</td>
<td>Bottom sheet to filter searching in CDM</td>
<td>Navigation drawer - Navigate to different app screens.</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/compare.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/compare_screen.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/compare_screen_detail.png" align="top"></td>
</tr>
<tr>
<td>Choose any two hospitals to compare them</td>
<td>Compare screen - Comparing general information</td>
<td>Compare screen - Comparing patient experience</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/download_cdm.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/view_cdm.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/view_cdm_statewise.png" align="top"></td>
</tr>
<tr>
<td>Download CDM - Download ChargeMaster of your nearby hospitals</td>
<td>View CDM - Viewing individual CDM with search functionality.</td>
<td>View CDM Statewise - View CDM of other states of US.</td>
</tr>
<tr>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/saved_cdm.png" align="top"></td>
<td><img src="https://raw.githubusercontent.com/Darshpreet2000/My-Blog/master/gist_images/about.png" align="top"></td>
</tr>
<tr>
<td>Saved ChargeMasters - CDMs Saved in SQL database of app</td>
<td>About us page of the project in the app.</td>
</tr>
</tbody>
</table>

</div>
</div>
</div>
</div>
 
