---
title: "One Place Foodie"
excerpt: "One Place to Find Where to Eat Next!<br/><img src='/images/OPFscreenshot.png'>"
collection: portfolio
---

* [One Place Foodie](http://34.71.80.132:8502/ "One Place Foodie")
* Streamlit server hosted on Google Cloud Platform VM. Should be running until June 30, 2021.

## Objective
* To find a restaurant nearby filtered by location and cuisine.

## Project Overview
* Scraped over 27,000 Restaurant Pages from a food directory platform
* Cleaned data and added geocodes
* Plotted all restaurants on map box with hover-over tooltip

## Code and Resources
**Python Version:** Python 3.8.5 Anaconda

**Packages:** pandas, numpy, matplotlib, seaborn, selenium, geopy, pickle, json, regex

## Web Scraping
* Food directory platform limited search results by page number. Suggestion was to use government food license titles to do a back search on the platform.
* The above searching method resulted in over 300,000 website links. After removing duplicates, only 27,000 results were used.

## Data Cleaning
* Data scraped had many missing values and had to be cleaned with regex.

## Production
* Streamlit was used to deploy the dataframe visualization and filtering

<img src="/images/oneplacefoodie/OPFdemo.png" alt="oneplacefoodie" title="oneplacefoodie"/>

## Futher Improvements
* Implement restaurant recommendation based on user's taste profile
* Implement dataframe filtering on mobile app

## Business Value
* Collect data on food preference of users (anonymously)
* Collect spending habits from restaurant visits
* Opportunities for Restaurants to promote thier brand

## GitHub
* [One Place Foodie](https://github.com/azwinlam/oneplacefoodie "One Place Foodie")