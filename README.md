# recycletracker_ng
RecycleTracker written in nodejs/javascript and angular2.

RecycleTracker
================

Copyright 2013, 2014, 2015, 2016 Kevin Dick.

RecycleTracker 

RecycleTracker is a web app designed to assist buildings in tracking their recycling rates by location using a simple scale with a serial connection (usually RS-232) and a RaspberryPi to collect scale data. Nodejs and Angular2 provide a very easy UI for the collection app, and Google Sheets provides a nice backend for the data store. A client web app provides some simple real-time statistics and can be built out as much as desired. 

The controller software ("RecycleCollector") collects the data using a barcode scanner and standard scale indicator, sending the information to Google Sheets (Google Sheets is more friendly for data analysis by non-technical clients). At the dock level, a building with a scale will connect with an app through the scale indicator. Using a barcode system, the building can track its waste and recycling on a daily basis. The dock app provides a visible data collection function, and sends the data to the front end app.

The front end of the app ("RecycleReporter") is a web page that displays on a tablet or tv and show the previous day's recycling rate, tips about how to recycle, graphs of progress over time, or other information - including a bullet chart for various recyclables, a leaderboard to show floor and/or suite rates in comparison, and a line graph for the rate of consumable recycling over time are some of the modules I've reviewed.

The app is designed to give building managers better real-time information on the recycling system to help them make improvements and get better recycling rates from tenants and visitors.


Dependencies:

For RecycleCollector

A nodejs serial library
A Google Apps Account (with OAUTH2 keys, etc.)

For RecycleReporter

see package.json